# Overview
How to use these rubrics: 
- Once a prospective Notary has filed an issue to apply, their application will be publicly graded on the below criteria. 
- First, the applicant will be checked to see none of the criteria for [Automatic Disqualification](/notaries/templates#automatic-disqualification).
- Next, the applicant will be ranked based on their merits as a Notary. Note, per row the applicant can get a score 1-5. If an applicant does not provide evidence, they will get a 0 for that row. Definitions for terms used in the criteria can be found below the rubrics. 
- Once the applicant has been ranked as a Notary, the outputs are fed into the [Allocation Rubric](/notaries/templates#notary-allocation-plan-rubric). This considers the merits of the applicant as a Notary along with their previous track record, and the robustness of their plan to determine the [final allocation amount](/notaries/templates#final-allocation-amount).

All scoring decisions should happen in public on the issue as filed, and iteration (e.g. improvements to an allocation plan) may be made within the issue. Editors of the repo will be able to assign the final score based on the merits of the application. On a regular cadence, review of open applications can occur where scoring decisions can be reviewed. When a final score is determined, a label will be set such that Root Key Holders can be made aware action is required. 

## Notary Rubric

| Category | Combination Logic | L1 | L2 | L3 | L4 | L5 | 
|-|-|-|-|-|-|-|
| **Long Term Network Alignment** | Max(Time Commitment, Stake Exposure)|
|Time Commitment| |Substantial, sustained contributions to Filecoin min. 6 mos |	Substantial, sustained contributions to Filecoin min. 1 year | Substantial, sustained contributions to Filecoin min. 2 years | Substantial, sustained contributions to Filecoin min. 3 years | Substantial, sustained contributions to Filecoin min. 4 years |
|Stake Exposure||100k tokens at stake|100-500k tokens at stake|1MM tokens at stake|5MM tokens at stake|10MM tokens at stake|
|**Industry Reputation**| Max(In-protocol Reputation, In-protocol Security, Organization Reputation, Individual Reputation)|
|In-protocol Reputation|| Reputable leader in Filecoin Ecosystem for > 6 mos |Reputable leader in Filecoin Ecosystem for 2 years |Reputable leader in Filecoin Ecosystem for 3 years |Reputable leader in Filecoin Ecosystem for 4 years|Reputable leader in Filecoin Ecosystem for 4+ years|
|In-protocol Security|| Contributions in identifying, responsibly disclosing, and fixing security vulnerabilities in protocols or services in the Filecoin community | Sustained contributions for 2+ years in identifying, responsibly disclosing, and fixing **serious** protocol or service vulnerabilities, in the Filecoin community | Sustained contributions for 2+ years in identifying, responsibly disclosing, and fixing **major** protocol or service vulnerabilities, in the Filecoin community | Sustained contributions for 3+ years in identifying, responsibly disclosing, and fixing **major** protocol or service vulnerabilities, in the Filecoin community | Sustained contributions for 4+ years in identifying, responsibly disclosing, and fixing **major** protocol or service vulnerabilities, in the Filecoin community|
|Organization Reputation|| Community Members | Reputable entities in Filecoin-adjacent communities with substantially adopted services / products (e.g. Supranational, Pinata, Infura) | Major organizations in Web3 (e.g. Polychain, Consensys) | Major organizations in Web2 and Web3 (e.g. Ethereum Foundation, Vimeo) | Household names / Publicly traded Institutions (e.g. Andreseen Horowitz, Netflix) | 
|Individual Reputation||Has access to 2+ social media accounts which individually have audiences > 500 where they will post publicly about their status as a notary if approved|Has access to 2+ social media accounts which individually have audiences > 1000 where they will post publicly about their status as a notary if approved|Has access to 2+ accounts on social media accounts which individually have audiences > 10000 about their status as a notary if approved|-|-| 
|**Diversity and Decentralization**| 0.7*(Geographic Distribution) + 0.3*(Use Case Diversity)|
|Geographic Distribution||>=4 existing Notaries or >=30% global DataCap has been allocated to the Region|3 existing Notaries or 20-30% global DataCap has been allocated to the Region|2 existing Notaries or 10-20% global DataCap has been allocated to the Region|1 existing Notary or <10% global DataCap has been allocated to the Region|Unrepresented geography|
|Use Case Diversity||Highly represented use case (4+ existing)|Highly represented use case (3 existing)|Somewhat represented use case (2 existing)|Under-represented use case (1 existing)|Unrepresented use case|

### Definitions
**Stake**: Stake, or tokens at stake, is defined as the sum of all locked, unvested, and liquid tokens at the time of application and should be roughly maintained over the course of the applicant's position as a Notary. 

**Substantial, sustained contributions**: Participation as a miner, active work as a developer (building ecosystem tooling, client applications, protocol improvements, etc) with significant impact, or active community advocate substantially increasing the reach and adoption of Filecoin. 

**Reputable leader**: Contributions to the Filecoin protocol and/or spec, creating and maintaining widely adopted services inside the commmunity, and cultivating the success of other members in the Filecoin ecosystem.

**Registered Organization**: A registered organization must be a government recognized entity with a minimum of the following: 
- Website
- Named officers
- Social media presence

**Geographies**: [North America, South America, Europe, Africa, Greater China, Asia-GCN, Oceania]

**Sample Use cases**: 
- Professional Services (Hosting Reseller, Digital Preservation, Long-term Backups, Long-term Log Storage)
- Developer Tools (Package Managers, Automatic Notaries)
- Web 3.0 / Decentralized Applications
- Web 2.0 Applications
- User Content (Personal Storage, User Generated Media)
- Scientific Data (Satellite Imagery, Geological Data, Computer Vision, Autonomous Driving) 
- Media & Entertainment
- Other

**Individual Reputation Note**
To qualify for this, the prospective Notary must post: 
- A statement about being accepted as a Notary
- A link to explain what a Notary is / Filecoin Plus
- A link to where they will be accepting incoming requests from clients

## Notary Allocation Plan Rubric
| Category | Combination Logic | L1 = Eligible up to 10TB | L2 = Eligible up to 100TB | L3 = Eligible up to 1PB | L4 = Eligible up to 10PB | L5 = Eligible up to 50PB | 
|-|-|-|-|-|-|-|
|**Weighted Notary Level**| Floor(0.3*(Long Term Network Alignment) + 0.4*(Industry Reputation) + 0.3*(Diversity and Decentralization))|
|**Concreteness of Allocation Plan**|Floor(0.4*(Allocation Strategy)+0.4*(Client Due Diligence) + 0.2*(Bookkeeping Plan))|
|Allocation Strategy||Minimal specificity in allocation strategy but demonstrates how allocation will reflect the Principles|Moderate specificity in allocation strategy in alignment with the Principles|Detailed plan, including tooling, to successfully allocate DataCap in a way that reflects the goals and values of the Principles|Detailed and convincing plan, including tooling, to successfully allocate DataCap in a way that reflects the goals and values of the Principles|L4 Requirements|
|Client Due Diligence||Minimal due diligence protecting against abuse and vetting clients|Base due diligence protecting against abuse and vetting clients |Robust due diligence for protecting against abuse and vetting clients|Robust due diligence for protecting against abuse and vetting clients|L4 Requirements|
|Bookkeeping Plan||Minimal plan to document DataCap allocation decision and ready to provide justification when challenged or dispute|Base plan to document DataCap allocation decision and ready to provide justification when challenged or dispute|Detailed plan, with tooling, to document DataCap allocation decision and ready to provide justification when challenged or dispute|Detailed plan, with tooling and defined audit processes, to document DataCap allocation decision and ready to provide justification when challenged or dispute|L4 Requirements|
|**Track Record**| Max(Past Allocations)|
|Past Allocations||No previous track record | Successful allocation <100TB of DataCap. Justifications and audit trail can be produced when challenged|Successful allocation of 100TB of DataCap. Convincing justifications and audit trail can be produced when challenged|Successful allocation of 1PB of DataCap. Convincing justifications and audit trail can be produced when challenged|Successful allocation of 10PB of DataCap. Convincing justifications and audit trail can be produced when challenged|
|**Scale of Allocation**|Max(DataCap Requested)|
| DataCap Requested || <10TB | 10-100TB	| 100TB- 1PB	| 1-10PB | 10PB+ |

#### Final Allocation Amount
Final Allocation Amount = Min(Round(0.5*(Track Record) + 0.3*(Weighted Notary Leveling) + 0.2*(Concretness of Allocation Plan)), Scale of Allocation)

## Automatic Disqualification
The following criteria are grounds for automatic disqualification as a Notary:
- Being found to be in violation of Filecoin's [Code of Conduct](https://github.com/filecoin-project/community/blob/master/CODE_OF_CONDUCT.md). 
- Severe or consistent acts of impropriety and abuse of one's role as Notary or as a Root Key Holder. Impropriety is defined as violating the Principles of this Mechanism, acting outside the remit of one's role (both as defined in this repository and as self-attested in the application process), or generally abusing the power entrusted to the role. Accusations of impropriety are expected to be filed via the [Disputes Mechanism](/README.md#dispute--audit-framework), where the accused will have an opportuntity to respond and justify their actions to the community. 
