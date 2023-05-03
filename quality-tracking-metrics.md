The current metric of measuring quality data onboarding / potential abuse consists of:

- Data stored in deals where the CID is shared across client DataCap applications (n-1*size of CID) - If two clients use the same dataset, if preparation is diff., then CID diff.
- Data stored in deals where the CID has been stored more than 2 times with the same SP ID (n-1*size of CID)
- All data stored by a client address where the client address has used between 10% and 90% of their DataCap allocation, has not made any deals in the last 6 weeks, and has stored everything in unique CIDs
