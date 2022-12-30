# Overview
Notaries are selected to act as [fiduciaries](https://www.merriam-webster.com/dictionary/fiduciary) for the Filecoin network. Notaries are entrusted to uphold the [Principles](https://github.com/filecoin-project/FIPs/blob/fip-0003/FIPS/fip-0003.md/#principles) of the program - responsibly allocating DataCap to help foster legitimate use cases on Filecoin. This document aims to provide additional specificity to the role/responsibility of Notaries, define the application and selection process, and the process for making changes. 

## Current active notaries

|region (CLEANED)          |Organization                                     |Github Link                                                      |3rd Round|4th Round|
|--------------------------|-------------------------------------------------|-----------------------------------------------------------------|---------|---------|
|Africa                    |Meibuy Cloud                                     |https://github.com/filecoin-project/notary-governance/issues/681 |         |checked  |
|Asia minus GCR            |BlockchainWorld                                  |https://github.com/filecoin-project/notary-governance/issues/648 |checked  |checked  |
|Asia minus GCR            |Define Platform                                  |https://github.com/filecoin-project/notary-governance/issues/657 |checked  |checked  |
|Asia minus GCR            |Greaterheat Pte.Ltd.                             |https://github.com/filecoin-project/notary-governance/issues/659 |         |checked  |
|Asia minus GCR            |Force Community                                  |https://github.com/filecoin-project/notary-governance/issues/668 |checked  |checked  |
|Asia minus GCR            |CoinSummer Labs                                  |https://github.com/filecoin-project/notary-governance/issues/669 |         |checked  |
|Asia minus GCR            |12Ships Foundation                               |https://github.com/filecoin-project/notary-governance/issues/677 |checked  |checked  |
|Asia minus GCR            |Bewell Technology Limited                        |https://github.com/filecoin-project/notary-governance/issues/679 |         |checked  |
|Asia minus GCR            |Protocan                                         |https://github.com/filecoin-project/notary-governance/issues/682 |         |checked  |
|Asia minus GCR            |Antalpha Digital Pte. Ltd.                       |https://github.com/filecoin-project/notary-governance/issues/683 |         |checked  |
|Asia minus GCR            |Bit Engine Pte Ltd                               |https://github.com/filecoin-project/notary-governance/issues/692 |         |checked  |
|Asia minus GCR            |Pluskit                                          |https://github.com/filecoin-project/notary-governance/issues/694 |checked  |checked  |
|Asia minus GCR            |Blockmaker                                       |https://github.com/filecoin-project/notary-governance/issues/695 |checked  |checked  |
|Asia minus GCR            |IPFS Japan Consortium                            |https://github.com/filecoin-project/notary-governance/issues/696 |checked  |checked  |
|Asia minus GCR            |ND LABS                                          |https://github.com/filecoin-project/notary-governance/issues/697 |checked  |checked  |
|Asia minus GCR            |BigData Exchange                                 |https://github.com/filecoin-project/notary-governance/issues/703 |         |checked  |
|Asia minus GCR            |EMO capital                                      |https://github.com/filecoin-project/notary-governance/issues/707 |         |checked  |
|Asia minus GCR            |METAVERSE                                        |https://github.com/filecoin-project/notary-governance/issues/709 |checked  |checked  |
|Asia minus GCR            |Bitrise capital                                  |https://github.com/filecoin-project/notary-governance/issues/716 |checked  |checked  |
|Asia minus GCR            |FBG Capital                                      |https://github.com/filecoin-project/notary-governance/issues/722 |checked  |checked  |
|Asia minus GCR            |Starboard                                        |https://github.com/filecoin-project/notary-governance/issues/745 |         |checked  |
|Asia minus GCR            |YuanHe Tech                                      |https://github.com/filecoin-project/notary-governance/issues/788 |checked  |checked  |
|Europe                    |Fungi Project                                    |https://github.com/filecoin-project/notary-governance/issues/600 |         |checked  |
|Europe                    |ZhongYiGuoLian                                   |https://github.com/filecoin-project/notary-governance/issues/638 |         |checked  |
|Europe                    |RawTech Ventures                                 |https://github.com/filecoin-project/notary-governance/issues/661 |         |checked  |
|Europe                    |Carohere/Carolina                                |https://github.com/filecoin-project/notary-governance/issues/676 |         |checked  |
|Europe                    |Speedium / DCENT BV.                             |https://github.com/filecoin-project/notary-governance/issues/678 |checked  |checked  |
|Europe                    |Direction Technology Co., LTD                    |https://github.com/filecoin-project/notary-governance/issues/717 |         |checked  |
|Europe                    |Twinquasar                                       |https://github.com/filecoin-project/notary-governance/issues/739 |checked  |checked  |
|Europe                    |Bobby Choi                                       |https://github.com/filecoin-project/notary-governance/issues/769 |         |checked  |
|Europe                    |Olivier Molenkamp                                |https://github.com/filecoin-project/notary-governance/issues/774 |         |checked  |
|Greater China Region (GCR)|Union Labs (formerly IPFSUnion)                  |https://github.com/filecoin-project/notary-governance/issues/135 |         |         |
|Greater China Region (GCR)|Wusi R&D Center                                  |https://github.com/filecoin-project/notary-governance/issues/178 |         |         |
|Greater China Region (GCR)|CoffeeCloud                                      |https://github.com/filecoin-project/notary-governance/issues/637 |checked  |checked  |
|Greater China Region (GCR)|ZC LABS                                          |https://github.com/filecoin-project/notary-governance/issues/643 |         |checked  |
|Greater China Region (GCR)|FILWallet                                        |https://github.com/filecoin-project/notary-governance/issues/644 |         |checked  |
|Greater China Region (GCR)|Venus Team                                       |https://github.com/filecoin-project/notary-governance/issues/645 |checked  |checked  |
|Greater China Region (GCR)|Fenbushi Capital                                 |https://github.com/filecoin-project/notary-governance/issues/647 |checked  |checked  |
|Greater China Region (GCR)|StorSwift                                        |https://github.com/filecoin-project/notary-governance/issues/663 |         |checked  |
|Greater China Region (GCR)|mkccstorage                                      |https://github.com/filecoin-project/notary-governance/issues/665 |         |checked  |
|Greater China Region (GCR)|IPFS Force                                       |https://github.com/filecoin-project/notary-governance/issues/667 |checked  |checked  |
|Greater China Region (GCR)|Guazi Dynamic                                    |https://github.com/filecoin-project/notary-governance/issues/670 |checked  |checked  |
|Greater China Region (GCR)|IPFSMain                                         |https://github.com/filecoin-project/notary-governance/issues/672 |checked  |checked  |
|Greater China Region (GCR)|Hangzhou Niutong Information Technology Co., Ltd.|https://github.com/filecoin-project/notary-governance/issues/674 |         |checked  |
|Greater China Region (GCR)|SXX Future Data                                  |https://github.com/filecoin-project/notary-governance/issues/680 |         |checked  |
|Greater China Region (GCR)|FileDrive Labs                                   |https://github.com/filecoin-project/notary-governance/issues/684 |         |checked  |
|Greater China Region (GCR)|Tianji Studio                                    |https://github.com/filecoin-project/notary-governance/issues/687 |checked  |checked  |
|Greater China Region (GCR)|ByteBase                                         |https://github.com/filecoin-project/notary-governance/issues/689 |checked  |checked  |
|Greater China Region (GCR)|BigFrog Technology                               |https://github.com/filecoin-project/notary-governance/issues/690 |         |checked  |
|Greater China Region (GCR)|BingHe Web3.0 Lab                                |https://github.com/filecoin-project/notary-governance/issues/699 |checked  |checked  |
|Greater China Region (GCR)|NonEntropy Tech.                                 |https://github.com/filecoin-project/notary-governance/issues/700 |checked  |checked  |
|Greater China Region (GCR)|New Web Group                                    |https://github.com/filecoin-project/notary-governance/issues/713 |checked  |checked  |
|Greater China Region (GCR)|MS Cloud                                         |https://github.com/filecoin-project/notary-governance/issues/719 |checked  |checked  |
|Greater China Region (GCR)|DeFIL                                            |https://github.com/filecoin-project/notary-governance/issues/720 |checked  |checked  |
|Greater China Region (GCR)|Genesis                                          |https://github.com/filecoin-project/notary-governance/issues/732 |checked  |checked  |
|Greater China Region (GCR)|IPFS.CN                                          |https://github.com/filecoin-project/notary-governance/issues/734 |         |checked  |
|Greater China Region (GCR)|TAKI Chain                                       |https://github.com/filecoin-project/notary-governance/issues/736 |         |checked  |
|Greater China Region (GCR)|Ewesion                                          |https://github.com/filecoin-project/notary-governance/issues/740 |         |checked  |
|Greater China Region (GCR)|Tokencan                                         |https://github.com/filecoin-project/notary-governance/issues/746 |         |checked  |
|Greater China Region (GCR)|Chengdu Codoon Health Technology Co., LTD        |https://github.com/filecoin-project/notary-governance/issues/752 |         |checked  |
|Greater China Region (GCR)|Cabrina Huang                                    |https://github.com/filecoin-project/notary-governance/issues/763#|checked  |checked  |
|Greater China Region (GCR)|STCould                                          |https://github.com/filecoin-project/notary-governance/issues/764 |checked  |checked  |
|Greater China Region (GCR)|POW POWER                                        |https://github.com/filecoin-project/notary-governance/issues/765 |checked  |checked  |
|Greater China Region (GCR)|Interstellar Storage（ShenZhen）                   |https://github.com/filecoin-project/notary-governance/issues/768 |         |checked  |
|Greater China Region (GCR)|1475                                             |https://github.com/filecoin-project/notary-governance/issues/770 |checked  |checked  |
|Greater China Region (GCR)|Fog Meta                                         |https://github.com/filecoin-project/notary-governance/issues/772 |         |checked  |
|Greater China Region (GCR)|Pangod                                           |https://github.com/filecoin-project/notary-governance/issues/775 |         |checked  |
|North America             |Textile                                          |https://github.com/filecoin-project/notary-governance/issues/53  |checked  |         |
|North America             |Glif                                             |https://github.com/filecoin-project/notary-governance/issues/467 |checked  |         |
|North America             |TinfraAC                                         |https://github.com/filecoin-project/notary-governance/issues/470 |checked  |         |
|North America             |Kernelogic                                       |https://github.com/filecoin-project/notary-governance/issues/658 |checked  |checked  |
|North America             |Tech Greedy                                      |https://github.com/filecoin-project/notary-governance/issues/664 |checked  |checked  |
|North America             |TopBlocks                                        |https://github.com/filecoin-project/notary-governance/issues/675 |         |checked  |
|North America             |NFTSTAR                                          |https://github.com/filecoin-project/notary-governance/issues/693 |checked  |checked  |
|North America             |Aifabot                                          |https://github.com/filecoin-project/notary-governance/issues/698 |         |checked  |
|North America             |Gate.io                                          |https://github.com/filecoin-project/notary-governance/issues/704 |checked  |checked  |
|North America             |New Huo Pool                                     |https://github.com/filecoin-project/notary-governance/issues/708 |         |checked  |
|North America             |ORIGIN Storage                                   |https://github.com/filecoin-project/notary-governance/issues/710 |checked  |checked  |
|North America             |Ipollo                                           |https://github.com/filecoin-project/notary-governance/issues/721 |checked  |checked  |
|North America             |Top Value Limited                                |https://github.com/filecoin-project/notary-governance/issues/729 |         |checked  |
|North America             |LendMi team                                      |https://github.com/filecoin-project/notary-governance/issues/730 |         |checked  |
|North America             |Banyan                                           |https://github.com/filecoin-project/notary-governance/issues/742 |checked  |checked  |
|North America             |Acrontech Inc.                                   |https://github.com/filecoin-project/notary-governance/issues/743 |         |checked  |
|North America             |Saukibit, Inc. (DBA Canza Finance)               |https://github.com/filecoin-project/notary-governance/issues/744 |         |checked  |
|North America             |XnMatrix                                         |https://github.com/filecoin-project/notary-governance/issues/747 |         |checked  |
|North America             |Filecoin Foundation                              |https://github.com/filecoin-project/notary-governance/issues/750 |checked  |checked  |
|North America             |Koda Inc.                                        |https://github.com/filecoin-project/notary-governance/issues/754 |         |checked  |
|North America             |SECUREXPERTS Inc.                                |https://github.com/filecoin-project/notary-governance/issues/756 |         |checked  |
|North America             |Ghost Byte Inc                                   |https://github.com/filecoin-project/notary-governance/issues/760 |         |checked  |
|North America             |PiKNiK                                           |https://github.com/filecoin-project/notary-governance/issues/776 |checked  |checked  |
|North America             |Nebula Block Data                                |https://github.com/filecoin-project/notary-governance/issues/777 |         |checked  |
|North America             |FilSwan                                          |https://github.com/filecoin-project/notary-governance/issues/778 |checked  |checked  |
|North America             |Nick Merrick                                     |https://github.com/filecoin-project/notary-governance/issues/779 |         |checked  |
|Oceania                   |West Labs                                        |https://github.com/filecoin-project/notary-governance/issues/430 |checked  |         |
|Oceania                   |OpenGate Technology                              |https://github.com/filecoin-project/notary-governance/issues/673 |         |checked  |
|Oceania                   |Holon Global Investments                         |https://github.com/filecoin-project/notary-governance/issues/748 |         |checked  |




### Regional Counts of active notaries
| Region         | Number of notaries |
|----------------|--------------------|
| Asia minus GCR |                 20 |
| Europe         |                  9 |
| Greater China  |                 33 |
| North America  |                 23 |
| Oceania        |                  2 |

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

# Notary Sets Use Cases 
  Support (1) or more the following, which can be linked to in a separate doc:
- Professional Services (Hosting Reseller, Long-term Backups, Data Warehousing)
- Developer Tools (Package Managers, Automatic Notaries, Web2 to Web3 integrations)
- Decentralized Applications
- User Content (Personal Storage)
- Public or Open Data (Scientific datasets, research data, government or historic
- Media & Entertainment (Videos, photos, NFTs)



## Removal Process
Notaries that have consistent and substantive issues raised against them and have been found to be legitimately abusing their power will be made ineligible for DataCap allocations. The process for raising and resolving disputes can be found [here](/README.md#dispute--audit-framework). 
