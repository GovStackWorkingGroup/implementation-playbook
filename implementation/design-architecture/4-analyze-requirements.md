# 4 Analyze Requirements

The first step in planning the architecture is to look at the requirements and other inputs (see [#inputs](architecture-design-overview.md#inputs "mention") ), which are mostly the results from the previous phase. The goal of this step is to establish full understanding of the service being developed. That will be the basis for all architectural decisions.

It will be important to have workshops with the product owner and analysts responsible for the service in the previous phases

## How to do it

### Start by reviewing the proposed end-to-end service

Walk through the service blueprint and prototypes. For each stage of the service, confirm and agree: &#x20;

1. What the user does and experiences&#x20;
2. How and where does the data flow
3. What happens behind the scenes to support that experience
4. Where decisions, handovers, or transitions occur
5. Which systems, services, or teams are involved



This helps to uncover complexity and dependencies in the service. Note down any assumptions, gaps or uncertainties.

## Non-functional requirements

Another important artifact that is often overlooked are non-functional requirements & quantities / sizing requirements. Make sure to check:

* If NFRs and quantities / sizing requirements are provided already, make sure to understand them. It is recommended to have a dedicated workshop on this with the relevant stakeholders, like owners of the partnering systems
* If they are not provided, request them to be provided.
* If neither is possible, check whether you can come up with reasonable estimates. Those estimates must then be aligned with the relevant stakeholders.
* Otherwise the missing NFRs should be raised as a risk to the project management.



<details>

<summary><strong>Examples for NFRs</strong></summary>

* Availability, SLA'
* Expected processing times / response times
* Accessibility
* Industry-specific compliance rules

</details>



<details>

<summary><strong>Examples for Quantities / Sizing Requirements</strong></summary>

* Total Number of users, Average number of users, Peak number of users
* Average message size, Maximum message size
* Number of requests per day / per hour / per second
* Size of documents / uploads

</details>



<details>

<summary><strong>Examples for relevant stakeholders</strong></summary>

* Product Owner
* Representative User from Business
* Operations Team
* Product Owner / Architect of partnering systems (sending / receiving requests to/from your system)
* Security Officer
* Data Protection Officer

</details>

## Outside Constraints

Additionally, you need to identify outside constraints. Make sure to understand the governance rules (for example GovStack Building Blocks, Guidelines for a common technology stack, mandatory use of defined apis & formats) and architecture principles. The following diagram gives a good overview of outside constraints: [Service Design](https://www.figma.com/board/9wR7PtrUde5SkpoBgan8ZV/Brainstorming-Service-Design?node-id=29-1105).
