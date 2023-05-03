The current metric of measuring quality data onboarding / potential abuse consists of:
- Data stored in deals where the CID is shared across client DataCap applications 
    - $(n-1)*\text{size of CID}$, where n is the number of duplicates
    - If two clients use the same dataset, but preparation is different, then we are counting them as different CIDs.
    - This likely means that the data is being duplicated many times and the client is storing it with the same SP
- Data stored in deals where the CID has been stored more than 2 times with the same SP ID
    - $(n-1)*\text{size of CID}$, where n is the number of duplicates
    - This likely means that the same data is being shared and stored by different clients
- All data stored by a client address where the client address has used between 10% and 90% of their DataCap allocation, has not made any deals in the last 6 weeks, and has stored everything in unique CIDs
    - This likely means that this not being duplicated at all and therefore not being distributed enough

The following is the a query specifying how we will tag deals under these three flags and its explanation:

```
CREATE OR REPLACE FUNCTION epoch_to_timestamp(epoch INTEGER)
    RETURNS INTEGER AS $$
BEGIN
    RETURN epoch * 30 + 1598306400;
END;
$$ LANGUAGE plpgsql;

CREATE OR REPLACE FUNCTION tag_over_replicated_deals()
    RETURNS VOID AS $$
BEGIN
    INSERT INTO deal_tags (deal_id, cid_overreplicated, sector_start, piece_size)
    SELECT
        cs.deal_id,
        cs.row_number > 1 AS cid_overreplicated,
        TO_TIMESTAMP(epoch_to_timestamp(cs.sector_start_epoch)),
        cs.piece_size
    FROM (
             SELECT
                 *,
                 ROW_NUMBER() OVER (
                     PARTITION BY piece_cid, provider
                     ORDER BY sector_start_epoch
                     ) AS row_number
             FROM
                 current_state
             WHERE
                     verified_deal = true
               AND sector_start_epoch > 0
         ) AS cs
    ON CONFLICT (deal_id)
        DO UPDATE SET cid_overreplicated = EXCLUDED.cid_overreplicated,
                      sector_start = EXCLUDED.sector_start, piece_size = EXCLUDED.piece_size;
END;
$$ LANGUAGE plpgsql;

CREATE OR REPLACE FUNCTION tag_cid_sharing_deals()
    RETURNS VOID AS $$
BEGIN
    WITH owner_count AS (
        SELECT
            piece_cid,
            COUNT(DISTINCT owner) AS owner_count
        FROM (
                 SELECT
                     current_state.piece_cid,
                     COALESCE(github_client_mapping.unique_id::TEXT, current_state.client) AS owner
                 FROM
                     current_state
                         LEFT JOIN github_client_mapping ON current_state.client = github_client_mapping.client_address
                 WHERE
                         verified_deal = true
                   AND sector_start_epoch > 0
             ) AS distinct_owners
        GROUP BY piece_cid
    )
    INSERT INTO deal_tags (deal_id, cid_shared, sector_start, piece_size)
    SELECT
        cs.deal_id,
        (cs.row_number > 1 AND oc.owner_count > 1) AS cid_shared,
        TO_TIMESTAMP(epoch_to_timestamp(cs.sector_start_epoch)),
        cs.piece_size
    FROM (
             SELECT
                 cs_with_owner.*,
                 ROW_NUMBER() OVER (
                     PARTITION BY piece_cid, owner
                     ORDER BY sector_start_epoch
                     ) AS row_number
             FROM (
                      SELECT
                          current_state.*,
                          COALESCE(github_client_mapping.unique_id::TEXT, current_state.client) AS owner
                      FROM
                          current_state
                              LEFT JOIN github_client_mapping ON current_state.client = github_client_mapping.client_address
                      WHERE
                              verified_deal = true
                        AND sector_start_epoch > 0
                  ) AS cs_with_owner
         ) AS cs
             JOIN owner_count oc ON cs.piece_cid = oc.piece_cid
    ON CONFLICT (deal_id)
        DO UPDATE SET cid_shared = EXCLUDED.cid_shared,
                      sector_start = EXCLUDED.sector_start, piece_size = EXCLUDED.piece_size;
END;
$$ LANGUAGE plpgsql;


CREATE OR REPLACE FUNCTION tag_cid_unique_deals()
    RETURNS VOID AS $$
BEGIN
    WITH eligible_clients AS (
        SELECT
            COALESCE(gcm.unique_id::TEXT, cs.client) AS grouped_client,
            SUM(cs.piece_size) AS total_storage,
            MAX(cs.sector_start_epoch) AS max_sector_start_epoch
        FROM
            current_state cs
                LEFT JOIN github_client_mapping gcm ON cs.client = gcm.client_address
        WHERE
                cs.verified_deal = true
          AND cs.sector_start_epoch > 0
        GROUP BY
            grouped_client
        HAVING
                SUM(cs.piece_size) > (1::BIGINT * 1024 * 1024 * 1024 * 1024)
           AND (TO_TIMESTAMP(epoch_to_timestamp(MAX(cs.sector_start_epoch))) + interval '6 weeks') <= NOW()
    ),
         unique_deals AS (
             SELECT
                 cs.*,
                 COALESCE(gcm.unique_id::TEXT, cs.client) AS grouped_client,
                 ROW_NUMBER() OVER (
                     PARTITION BY COALESCE(gcm.unique_id::TEXT, cs.client), cs.piece_cid
                     ORDER BY cs.sector_start_epoch
                     ) AS row_number
             FROM
                 current_state cs
                     LEFT JOIN github_client_mapping gcm ON cs.client = gcm.client_address
             WHERE
                     cs.verified_deal = true
               AND cs.sector_start_epoch > 0
         )
    INSERT INTO deal_tags (deal_id, cid_unique, sector_start, piece_size)
    SELECT
        ud.deal_id,
        (ud.row_number = 1 AND ec.grouped_client IS NOT NULL) AS cid_unique,
        TO_TIMESTAMP(epoch_to_timestamp(ud.sector_start_epoch)),
        ud.piece_size
    FROM
        unique_deals ud
            LEFT JOIN eligible_clients ec ON ud.grouped_client = ec.grouped_client
    ON CONFLICT (deal_id)
        DO UPDATE SET
                      cid_unique = EXCLUDED.cid_unique,
                      sector_start = EXCLUDED.sector_start,
                      piece_size = EXCLUDED.piece_size;
END;
$$ LANGUAGE plpgsql;
```
This code defines four PostgreSQL functions using PL/pgSQL, a procedural language for PostgreSQL. These functions are used to tag and process deal data related to file storage.

epoch_to_timestamp(epoch INTEGER): This function takes an integer epoch as input and returns an integer. It converts the given epoch value to a timestamp by multiplying it by 30 and then adding the constant 1598306400. The returned value represents Unix time.

tag_over_replicated_deals(): This function tags deals that are over-replicated. It does so by inserting or updating deal tags in the deal_tags table based on the calculated cid_overreplicated value, which indicates whether the deal is over-replicated or not. The function also sets sector_start and piece_size columns for the corresponding deal.

tag_cid_sharing_deals(): This function tags deals that share content identifiers (CIDs) across multiple clients. It calculates the cid_shared value, which indicates whether the deal shares a CID with other deals, and inserts or updates the deal_tags table with this value. The function also sets sector_start and piece_size columns for the corresponding deal.

tag_cid_unique_deals(): This function tags deals with unique content identifiers (CIDs) for clients that have stored more than 1 TiB of data and have not added any new storage within the last 6 weeks. It calculates the cid_unique value, which indicates whether the deal has a unique CID or not, and inserts or updates the deal_tags table with this value. The function also sets sector_start and piece_size columns for the corresponding deal.

In summary, these four functions are designed to process and tag deal data in a PostgreSQL database, which can be useful for tracking and analyzing data storage deals.
