# Overview
Notaries are selected to act as [fiduciaries](https://www.merriam-webster.com/dictionary/fiduciary) for the Filecoin network. Notaries are entrusted to uphold the [Principles](https://github.com/filecoin-project/FIPs/blob/fip-0003/FIPS/fip-0003.md/#principles) of the program - responsibly allocating DataCap to help foster legitimate use cases on Filecoin. This document aims to provide additional specificity to the role/responsibility of Notaries, define the application and selection process, and the process for making changes. 

## Current active notaries

| Region         | Organization                    | Notary Name                       | Link to application                                              | Approved allocation amount | Existing Notary |
|----------------|---------------------------------|-----------------------------------|------------------------------------------------------------------|----------------------------|-----------------|
| Asia minus GCN | 12ships Foundation              | Irene Young                       | https://github.com/filecoin-project/notary-governance/issues/456 | 1PiB                      | Yes             |
| Asia minus GCN | Bitrise Capital                 | Suki                              | https://github.com/filecoin-project/notary-governance/issues/443 | 1PiB                       | No, new notary  |
| Asia minus GCN | BlockChain World                | Sounghwan Park                    | https://github.com/filecoin-project/notary-governance/issues/408 | 1PiB                       | No, new notary  |
| Asia minus GCN | BlockMaker                      | BlockMaker                        | https://github.com/filecoin-project/notary-governance/issues/454 | 1PiB                       | No, new notary  |
| Asia minus GCN | Define Platform                 | Alex Kim                          | https://github.com/filecoin-project/notary-governance/issues/463 | 1PiB                       | No, new notary  |
| Asia minus GCN | FBG Capital                     | Gary Gao                          | https://github.com/filecoin-project/notary-governance/issues/458 | 1PiB                      | No, new notary  |
| Asia minus GCN | Firefly (YuanHe Tech)           | embedsky                          | https://github.com/filecoin-project/notary-governance/issues/465 | 500TiB                     | No, new notary  |
| Asia minus GCN | Force Web3 Community            | Tim Guo (柏礼）                   | https://github.com/filecoin-project/notary-governance/issues/426 | 100TiB                     | No, new notary  |
| Asia minus GCN | IPFS Japan Consortium           | Masaaki Nawatani                  | https://github.com/filecoin-project/notary-governance/issues/410 | 1PiB                       | Yes             |
| Asia minus GCN | ND Labs                         | Leo                               | https://github.com/filecoin-project/notary-governance/issues/449 | 1PiB                       | No, new notary  |
| Asia minus GCN | Pluskit                         | Pluskit                           | https://github.com/filecoin-project/notary-governance/issues/448 | 1PiB                       | No, new notary  |
| Asia minus GCN | Tenet Data Systems * *Pending dispute resolution*              | Tenet Data Systems                | https://github.com/filecoin-project/notary-governance/issues/464 | 1PiB                       | No, new notary  |
| Europe         | 4Everland                       | Deon Erda                         | https://github.com/filecoin-project/notary-governance/issues/450 | 1PiB                       | No, new notary  |
| Europe         | Filecoin Foundation             | Filecoin Foundation               | https://github.com/filecoin-project/notary-governance/issues/469 | 1PiB                       | Yes             |
| Europe         | Speedium                        | Wijnand Schouten                  | https://github.com/filecoin-project/notary-governance/issues/414 | 1PiB                       | Yes             |
| Europe         | TechHedge (Reiers)              | Nicklas Reiersen                  | https://github.com/filecoin-project/notary-governance/issues/471 | 100TiB                     | Yes             |
| Europe         | Twinquasar                      | Julien NOEL                       | https://github.com/filecoin-project/notary-governance/issues/468 | 100TiB                     | Yes             |
| Greater China  |                            1475 | Simon                             | https://github.com/filecoin-project/notary-governance/issues/423 | 1PiB                      | Yes             |
| Greater China  | BingHe Web3.0 Lab               | BingHe Web3.0 Lab                 | https://github.com/filecoin-project/notary-governance/issues/441 | 1PiB                      | Yes             |
| Greater China  | ByteBase                        | Eric                              | https://github.com/filecoin-project/notary-governance/issues/419 | 1PiB                       | No, new notary  |
| Greater China  | Cabrina Huang                   | Cabrina Huang                     | https://github.com/filecoin-project/notary-governance/issues/440 | 1PiB                       | No, new notary  |
| Greater China  | Coffee Cloud                    | Coffee Cloud                      | https://github.com/filecoin-project/notary-governance/issues/386 | 1PiB                       | No, new notary  |
| Greater China  | DeFil                           | Eden                              | https://github.com/filecoin-project/notary-governance/issues/446 | 1PiB                       | No, new notary  |
| Greater China  | Fenbushi Capital                | Fenbushi Capital                  | https://github.com/filecoin-project/notary-governance/issues/418 | 1PiB                      | Yes             |
| Greater China  | Genesis                         | Anne                              | https://github.com/filecoin-project/notary-governance/issues/411 | 1PiB                       | No, new notary  |
| Greater China  | Guazi Dynamic                   | Fatman13                          | https://github.com/filecoin-project/notary-governance/issues/424 | 10TiB                      | No, new notary  |
| Greater China  | IPFS Metaverse Community        | Nic                               | https://github.com/filecoin-project/notary-governance/issues/434 | 100TiB                     | No, new notary  |
| Greater China  | IPFSForce                       | Steven Li                         | https://github.com/filecoin-project/notary-governance/issues/412 | 1PiB                       | Yes             |
| Greater China  | IPFSMain                        | Neo Ge                            | https://github.com/filecoin-project/notary-governance/issues/413 | 1PiB                       | Yes             |
| Greater China  | MatrixStorage                   | Matrix Storage                    | https://github.com/filecoin-project/notary-governance/issues/436 | 1PiB                      | No, new notary  |
| Greater China  | New Web Group                   | New Web HK Group Holdings Limited | https://github.com/filecoin-project/notary-governance/issues/422 | 1PiB                       | No, new notary  |
| Greater China  | NonEntropy Tech                 | Junyao Ren                        | https://github.com/filecoin-project/notary-governance/issues/445 | 300TiB                     | No, new notary  |
| Greater China  | POW Power                       | ZHIHUI                            | https://github.com/filecoin-project/notary-governance/issues/447 | 1PiB                       | No, new notary  |
| Greater China  | STCloud                         | Barry                             | https://github.com/filecoin-project/notary-governance/issues/429 | 1PiB                       | No, new notary  |
| Greater China  | Tianji Studio                   | Bailey-li                         | https://github.com/filecoin-project/notary-governance/issues/453 | 1PiB                       | No, new notary  |
| Greater China  | Union Labs (formally IPFSUnion) | Jackie Mo                         | https://github.com/filecoin-project/notary-governance/issues/416 | 1PiB                       | Yes             |
| Greater China  | Venus Team - IPFSForce          | Joss Hua                          | https://github.com/filecoin-project/notary-governance/issues/431 | 100TiB                      | No, new notary  |
| Greater China  | Waterdrop Lab                   | Waterdrop Lab                     | https://github.com/filecoin-project/notary-governance/issues/432 | 1PiB                       | No, new notary  |
| North America  | Banyan                          | Claudia Richoux                   | https://github.com/filecoin-project/notary-governance/issues/459 | 100TiB                     | No, new notary  |
| North America  | Filswan                         | Charles Cao                       | https://github.com/filecoin-project/notary-governance/issues/433 | 100TiB                     | Yes             |
| North America  | Gate.io                         | Fafa                              | https://github.com/filecoin-project/notary-governance/issues/461 | 1PiB                       | No, new notary  |
| North America  | Infinite Scroll // Glif         | Glif Verifier                     | https://github.com/filecoin-project/notary-governance/issues/467 | 100TiB                     | Yes             |
| North America  | IPOLLO                          | M                                 | https://github.com/filecoin-project/notary-governance/issues/439 | 1PiB                       | No, new notary  |
| North America  | Kernelogic                      | Fei Yan                           | https://github.com/filecoin-project/notary-governance/issues/409 | 1PiB                       | No, new notary  |
| North America  | NFTStar                         | Vito                              | https://github.com/filecoin-project/notary-governance/issues/444 | 1PiB                       | No, new notary  |
| North America  | Origin Storage                  | ORIGIN Storage                    | https://github.com/filecoin-project/notary-governance/issues/452 | 1PiB                       | No, new notary  |
| North America  | Performive * *Pending dispute resolution*                     | Tim Williams                      | https://github.com/filecoin-project/notary-governance/issues/420 | 1PiB                       | Yes             |
| North America  | PiKNiK                          | James Hoang                       | https://github.com/filecoin-project/notary-governance/issues/438 | 100TiB                     | No, new notary  |
| North America  | Tech Greedy                     | Xinan Xu                          | https://github.com/filecoin-project/notary-governance/issues/421 | 1PiB                       | No, new notary  |
| North America  | Textile                         | Andrew Hill                       | https://github.com/filecoin-project/notary-governance/issues/472 | 100TiB                     | Yes             |
| North America  | Tinfra                          | Tinfra LLC                        | https://github.com/filecoin-project/notary-governance/issues/470 | 1PiB                       | No, new notary  |
| Oceania        | Holon Innovations               | Holon Innovations                 | https://github.com/filecoin-project/notary-governance/issues/460 | 100TiB                     | Yes             |
| Oceania        | MetaWave                        | Jazz Hsiao                        | https://github.com/filecoin-project/notary-governance/issues/457 | 100TiB                     | No, new notary  |
| Oceania        | West Labs                       | West Labs Venture                 | https://github.com/filecoin-project/notary-governance/issues/430 | 100TiB                     | No, new notary  |


### Regional Counts of active notaries
| Region         | Number of notaries | Total DataCap allocated to region |
|----------------|--------------------|-----------------------------------|
| Asia minus GCN |                 12 | 10.5 PiB                          |
| Europe         |                  5 | 3.2 PiB                            |
| Greater China  |                 21 | 10.5 PiB                          |
| North America  |                 13 | 8.5 PiB                          |
| Oceania        |                  3 | 300 TiB                            |

## Roles & Responsibilities
The base responsibilities of the Notaries are as follows: 
- Allocate DataCap to clients in order to subsidize reliable and useful storage on the network.
- Verify that clients receive a DataCap commensurate with the level of trust that is warranted based on information provided. 
- Ensure that in the allocation of the DataCap no party is given excessive trust in any form that might jeopardize the network.
- Follow operational guidelines, keep record of decision flow, and respond to any requests for audits of their allocation decisions.

**Note:** Notaries are given autonomy in their decision making process and encouraged to allocate DataCap based on their best judgement. However, Notaries should expect to answer any questions about previous allocation decisions before receiving future DataCap to distribute. Guidelines for reasonable allocation strategies are supplied in this repository (both a [recommended scoring mechanism for prospective Clients](/notaries/templates/client-evaluation.md), as well as a [sample set of questions to ask of Clients](/notaries/templates/sample-client-application.md)). While not mandatory to use, these documents represent the expected baseline for well-behaved Notaries.

## Operational Guidelines
As stated above, Notaries are given a high degree of autonomy in their decision making power. In order to build trust in the stability of this mechanism, below outlined are some basic criteria by which all Notaries are expected to adhere. In the future these restrictions may be reduced or removed, upon approval by the community (going through the standard PR process). 

* **Upfront Disclosures**: Prior to being confirmed as a Notary, Notaries are expected to disclose all relevant addresses which they control, have a financial stake in, or are strongly connected to by other means. For the disclosure, the Notary should state the relevant addresses and the nature of the relationship. 

* **Promoting Client Best Practices**: Notaries agree to educate approved clients about the best practices for using their DataCap (e.g. how to request additonal services from miners, storing data redundantly across many miners, etc). Some reference information can be found [here](https://github.com/filecoin-project/notary-governance/issues/9).

* **Commitment to effeciently serving the Network**: Notaries agree to serve as fiduciaries of the Network, striving to work towards bringing useful data onto Filecoin and improving the experience for clients to do so. Notaries should generally be able to respond to Client applications and updates within 3 days, and should be comfortable communicating with Clients and Notaries if an application needs to be redirected.

* **No Self Dealing**: To prevent conflicts of interest, Notaries should not allocate DataCap to Clients over which they control the private keys, or to a Client who intends to specifically spend the allocated DataCap with an address affiliated with the Notary. When in doubt, Notaries should bias towards transparency (i.e. public disclosure) or to getting a different Notary to handle the individual request. 

* **Operating in Good Faith**: Notaries hold a position of trust in the network, and as such it is expected that they operate keeping the Principles of this mechanism in mind. While each form of abuse cannot be exhaustively defined, Notaries are expected to bias towards caution and act in a way that promotes transparency. Notaries should expect to potentially recieve requests or questions for allocation decisions (within reason) - and should make decisions with this in mind.

* **Community Governance Participation**: It is expected that Notaries regularly attend the scheduled Governance calls. As these calls are a forum to shape this process, it is important to ensure Notaries are present to provide their context, learnings, and input. 

## Application / Selection Process
For those interested in providing this service to the Filecoin network, they may apply to this role by filing an Issue [here](https://github.com/filecoin-project/notary-governance/issues/new/choose). Applications for this third round closed in March, and we anticipate opening the fourth round of notary applications in Q4 of 2022.

Please note, applications are reviewed during the [community governance call](/README.md#governance-and-iteration-process) - and will be graded according to this community defined [criteria](/notaries/templates#overview). Edits to the criteria, will follow the same process as any proposed change to this repository, defined [here](/README.md#process-for-modifications).

Notaries were selected by regions based on the issue proposed [here](https://github.com/filecoin-project/notary-governance/issues/479).

Prospective Notaries will be ranked based on the rounded score used to determine their DataCap allocation. 





## Removal Process
Notaries that have consistent and substantive issues raised against them and have been found to be legitimately abusing their power will be made ineligible for DataCap allocations. The process for raising and resolving disputes can be found [here](/README.md#dispute--audit-framework). 
