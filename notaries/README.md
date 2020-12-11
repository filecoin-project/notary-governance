# Overview
Notaries are selected to act as [fiduciaries](https://www.merriam-webster.com/dictionary/fiduciary) for the Filecoin network. Notaries are entrusted to uphold the [Principles](https://github.com/filecoin-project/FIPs/blob/fip-0003/FIPS/fip-0003.md/#principles) of the program - responsibly allocating DataCap to help foster legitimate use cases on Filecoin. This document aims to provide additional specificity to the role/responsibility of Notaries, define the application and selection process, and the process for making changes. 

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

* **No Self Dealing**: To prevent conflicts of interest, Notaries should not allocate DataCap to Clients over which they control the private keys, or to a Client who intends to specifically spend the allocated DataCap with an address affiliated with the Notary. When in doubt, Notaries should bias towards transparency (i.e. public disclosure) or to getting a different Notary to handle the individual request. 

* **Operating in good faith**: Notaries hold a position of trust in the network, and as such it is expected that they operate keeping the Principles of this mechanism in mind. While each form of abuse cannot be exhaustively defined, Notaries are expected to bias towards caution and act in a way that promotes transparency. Notaries should expect to potentially recieve requests or questions for allocation decisions (within reason) - and should make decisions with this in mind. 

## Application / Selection Process
For those interested in providing this service to the Filecoin network, they may apply to this role by filing an Issue [here](https://github.com/filecoin-project/notary-governance/issues/new/choose).

Please note, applications are reviewed during the [community governance call](/README.md#governance-and-iteration-process) - and will be graded according to this community defined [criteria](/notaries/templates#overview). Edits to the criteria, will follow the same process as any proposed change to this repository, defined [here](/README.md#process-for-modifications).

To begin, the first wave of Notaries to be constrained at a cap of **3 Notaries per geography** based on the highest scoring initial applicants. To start, prospective Notaries will be ranked based on the rounded score used to determine their DataCap allocation. 

### Tiebreaking
In the event more than 3 Notaries in the same geography share the same score, the unrounded score (that considers the Notary weight, allocation strategy, and track record) will be used. In the event there is still a tie, the community can decide whether to approve both Notaries OR to pick the Notary who will provide the most contributions to the ecosystem (e.g. through open source tooling that might benefit future Notaries). 

We propose this constraint to ensure any issues that arise early on in this process can be dealt with while introducing minimal impact. As this process stabalizes, we envision this constraint will be relaxed. 

## Removal Process
Notaries that have consistent and substantive issues raised against them and have been found to be legitimately abusing their power will be made ineligible for DataCap allocations. The process for raising and resolving disputes can be found [here](/README.md#dispute--audit-framework). 
