# Overview
Notaries are selected to act as [fiduciaries](https://www.merriam-webster.com/dictionary/fiduciary) for the Filecoin network. Notaries are entrusted to uphold the [Principles](https://github.com/filecoin-project/FIPs/blob/fip-0003/FIPS/fip-0003.md/#principles) of the program - responsibly allocating DataCap to help foster legitimate use cases on Filecoin. This document aims to provide additional specificity to the role/responsibility of Notaries, define the application and selection process, and the process for making changes. 

## Current active notaries

|region                    |Github Link                                                     |Organization                                |(POC) Name                    |
|--------------------------|----------------------------------------------------------------|--------------------------------------------|------------------------------|
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/648|BlockchainWorld                             |Sounghwan Park                |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/657|Define Platform                             |Alex Kim                      |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/659|Greaterheat Pte.Ltd.                        |Neo                           |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/668|Force Community                             |Tim Guo (柏礼）                  |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/669|CoinSummer Labs                             |Max                           |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/677|12Ships Foundation                          |Irene Young                   |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/682|Protocan                                    |AnthonySmith                  |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/683|Antalpha Digital Pte. Ltd.                  |Xin Jin                       |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/692|Bit Engine Pte Ltd                          |Reeta                         |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/694|Pluskit                                     |Pluskit                       |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/695|Blockmaker                                  |Blockmaker                    |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/696|IPFS Japan Consortium                       |Masaaki Nawatani              |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/697|ND LABS                                     |Leo                           |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/703|BigData Exchange                            |CB Tan                        |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/707|EMO capital                                 |Bruce                         |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/709|METAVERSE DATA MINING PTE.LTD.              |MDM                           |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/716|Bitrise capital                             |Kivi                          |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/722|FBG Capital                                 |Gary Gao                      |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/745|Starboard                                   |Sylvan Zhang                  |
|Asia minus GCR            |https://github.com/filecoin-project/notary-governance/issues/788|YuanHe Tech ( Firefly )                     |FireflyHZ                     |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/637|CoffeeCloud                                 |CoffeCloud                    |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/643|ZC LABS                                     |zhongchuang                   |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/644|FILWallet                                   |a1991car                      |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/645|Venus Team                                  |Joss Hua                      |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/647|N.A.                                        |Fenbushi Capital              |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/663|StorSwift                                   |StorSwift                     |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/665|mkccstorage                                 |Hunter                        |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/667|IPFS Force                                  |Steven Li                     |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/670|Guazi Dynamic                               |@Fatman13                     |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/672|IPFSMain                                    |Neo Ge                        |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/674|Hangzhou Niutong Information Technology Co. | Ltd.                         |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/680|SXX Future Data                             |Darleen                       |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/684|FileDrive Labs                              |Laura Ren                     |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/687|Tianji Studio                               |Bailey-li                     |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/689|ByteBase                                    |Eric                          |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/699|BingHe Web3.0 Lab                           |MRJAVAZHAO                    |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/700|NonEntropy Tech.                            |Junyao Ren                    |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/713|New Web Group                               |Yuan                          |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/719|MS Cloud                                    |Tracy                         |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/720|DeFIL                                       |Eden                          |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/732|Genesis                                     |Anne                          |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/734|IPFS.CN                                     |Nic                           |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/736|TAKI Chain                                  |Smart Dong                    |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/740|Ewesion                                     |Ewesion                       |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/746|Tokencan                                    |Tokencan                      |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/752|Chengdu Codoon Health Technology Co.        | LTD                          |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/763|N/A                                         |Cabrina Huang                 |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/764|STCould                                     |LISA                          |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/765|POW POWER                                   |Jackson                       |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/768|Interstellar Storage                        |Interstellar Storage（ShenZhen）|
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/770|1475                                        |Simon                         |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/772|FogMeta                                     |FogMeta                       |
|Greater China Region (GCR)|https://github.com/filecoin-project/notary-governance/issues/775|Pangod                                      |Casey                         |
|North America             |https://github.com/filecoin-project/notary-governance/issues/658|Kernelogic                                  |Fei Yan                       |
|North America             |https://github.com/filecoin-project/notary-governance/issues/664|Tech Greedy                                 |Xinan Xu                      |
|North America             |https://github.com/filecoin-project/notary-governance/issues/675|TopBlocks                                   |Harry Ma                      |
|North America             |https://github.com/filecoin-project/notary-governance/issues/693|NFTSTAR                                     |Vivian                        |
|North America             |https://github.com/filecoin-project/notary-governance/issues/698|Aifabot                                     |Benny                         |
|North America             |https://github.com/filecoin-project/notary-governance/issues/704|Gate.io                                     |Fafa                          |
|North America             |https://github.com/filecoin-project/notary-governance/issues/708|New Huo Pool                                |New Huo Pool                  |
|North America             |https://github.com/filecoin-project/notary-governance/issues/710|ORIGIN Storage                              |ORIGIN Storage                |
|North America             |https://github.com/filecoin-project/notary-governance/issues/721|Ipollo                                      |Mona                          |
|North America             |https://github.com/filecoin-project/notary-governance/issues/729|Top Value Limited                           |Top Value Finance             |
|North America             |https://github.com/filecoin-project/notary-governance/issues/730|LendMi team                                 |LendMi                        |
|North America             |https://github.com/filecoin-project/notary-governance/issues/742|Banyan                                      |Claudia Richoux               |
|North America             |https://github.com/filecoin-project/notary-governance/issues/743|Acrontech Inc.                              |Gendin Han                    |
|North America             |https://github.com/filecoin-project/notary-governance/issues/744|Saukibit                                    | Inc. (DBA Canza Finance)     |
|North America             |https://github.com/filecoin-project/notary-governance/issues/747|XnMatrix                                    |XnMatrix                      |
|North America             |https://github.com/filecoin-project/notary-governance/issues/750|Filecoin Foundation                         |Danny O'Brien                 |
|North America             |https://github.com/filecoin-project/notary-governance/issues/754|Koda Inc.                                   |Emma Russell                  |
|North America             |https://github.com/filecoin-project/notary-governance/issues/756|SECUREXPERTS Inc.                           |Darnell Washington            |
|North America             |https://github.com/filecoin-project/notary-governance/issues/760|Ghost Byte Inc                              |Trevor K Smith                |
|North America             |https://github.com/filecoin-project/notary-governance/issues/776|PiKNiK                                      |James Hoang                   |
|North America             |https://github.com/filecoin-project/notary-governance/issues/777|Nebula Block Data                           |Boqian Wang                   |
|North America             |https://github.com/filecoin-project/notary-governance/issues/778|FilSwan                                     |FilSwan                       |
|North America             |https://github.com/filecoin-project/notary-governance/issues/779|N/A                                         |Nick Merrick                  |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/600|Fungi Project                               |Andress Sarria                |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/638|ZhongYiGuoLian                              |Patapon                       |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/661|RawTech Ventures                            |RawTech Ventures              |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/676|N/A.                                        |Carohere/Carolina             |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/678|Speedium / DCENT BV.                        |Wijnand Schouten              |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/717|Direction Technology Co.                    | LTD                          |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/739|Twinquasar                                  |Julien NOEL                   |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/769|N/A                                         |Bobby Choi                    |
|Europe                    |https://github.com/filecoin-project/notary-governance/issues/774|N/A                                         |Olivier Molenkamp             |
|Africa.                   |https://github.com/filecoin-project/notary-governance/issues/681|Meibuy Cloud                                |Meibuy                        |
|Oceania                   |https://github.com/filecoin-project/notary-governance/issues/673|OPENGATE TECHNOLOGY INVESTMENT GROUP PTY LTD|TAO YANG                      |
|Oceania                   |https://github.com/filecoin-project/notary-governance/issues/748|Holon Global Investments PTY Ltd            |Holon Innovations             |



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
