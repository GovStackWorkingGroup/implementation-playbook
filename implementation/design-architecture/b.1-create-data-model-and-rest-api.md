# B.1 - Create Data Model & REST API

Creating the data model and the API are activities that should be done in tandem because they inform each other well.

While defining the API, you will need knowledge about the data model (to define your REST resources and payloads), but designing the endpoints will also inspire changes to the data model.

The same is true the other way around. While defining the data model, you will discover candidates for REST resources. You also have to consider dependencies between entities, which will influence the endpoint structure.

Finally, the outputs produced in this step will accelerate the development of the service. Depending on how it is done, the results can even be used directly in the code (generating endpoints from OpenAPI, specifying the data model in source code and generating the ER-diagram).

## How to Do It

This is still primarily a process of analyzing the requirements. Therefore, the format will still consist of workshops with the product owner and the business analyst(s).

1. Analyze the user journeys & data flows and identify the entities and endpoints needed in each step. You can use the [GovStack Service Blueprint](https://www.figma.com/board/DAK1g4cpOaBYIEh86jrSaf/Service-Blueprint-Template?node-id=0-1\&p=f) for this.
   1. Watch out for edge cases and error scenarios.
   2. Watch out for interactions with external systems, especially those that might not yet have been identified. (In this case, also update the [2-start-with-the-system-context.md](2-start-with-the-system-context.md "mention").)
2. Document your findings in an ER diagram and an API specification.
3. Review and iterate as needed.

### Document the Data Model

Ideally there will already be a functional data model to guide you. While the technical data model will usually be very close to the functional data model, this activity is still necessary to make sure technical constraints are considered as well.

The data model should be described in an ER diagram. While documenting the data model, you should:

* Create separate data models for each bounded context.&#x20;
  * In case there are similar entities used in multiple contexts, DDD recommends to create a separate entity in each context's data model\
    ![](<../../.gitbook/assets/image (26).png>)
  * There are multiple patterns how to handle such shared entities. It is impossible to give a hard recommendation here, because it depends too much on the specifics
  * Documentation on Context Mapping Patterns
    * [Context Mapping in Domain-Driven Design: Visualizing and Managing Bounded Contexts](https://softwarepatternslexicon.com/java/domain-driven-design-ddd-patterns/strategic-patterns/context-mapping/)
    * [https://github.com/ddd-crew/context-mapping](https://github.com/ddd-crew/context-mapping)
    * [Domain Driven Design | Deep dive into context mapping](https://medium.com/geekculture/domain-driven-design-deep-dive-into-context-mapping-f9cd8acddd7e)<br>
  * Be wary though not to step into the trap of overengineering. Often the least complex approach will prove as the best. Only choose a more complex pattern if the added complexity actually adds a tangible value.
* Try to identify business components.
  * Usually a bounded context indicates that corresponding business component is needed.&#x20;
  * But even within a bounded context (or if no bounded contexts have been identified so far), it might be useful to divide the service even further into smaller business components
  * Often, the data will indicate potential business components. Look at the relations in the data model and try to identify areas of high cohesion and low cohesion.
* Try to identify data structures that require custom datatypes and or value objects
* Watch out for entities that require statuses or state models. These are often central to business flows and the design of endpoints.
* Watch out for use cases justifying denormalized (flattened) entities, like in a staging area or for performance reasons
* See [#data-model](architecture-best-practices-and-patterns.md#data-model "mention") for more detailed tips

This will:

* allow you to understand the data better,
* and help in later steps such as [b.2-create-container-diagram.md](b.2-create-container-diagram.md "mention") and [b.3-create-component-diagram.md](b.3-create-component-diagram.md "mention").

### Document the Internal API

Defining the api in a "API First" manner will help in later steps such as [b.2-create-container-diagram.md](b.2-create-container-diagram.md "mention") and [b.3-create-component-diagram.md](b.3-create-component-diagram.md "mention"), already providing a significant part of the functionality & structure. While documenting the api, you should

* first review your [#architecture-governance](architecture-design-overview.md#architecture-governance "mention") on api & endpoint design
* Use OpenAPI as specification format
* prefer REST + JSON if possible
* plan for a versioned API right from the start
  * the api should be as stable as possible, especially those parts for communicating with external systems. Versioning helps a lot with that.
* Divide into internal / external apis
  * Dont publish your full api to everyone, select who can access what
  * Your internal api will probably consist mostly of CRUD operations
* Have in mind that apis for different bounded contexts will probably end up in different containers / components. So keep track of which context an endpoint is serving.
* see [#api-design](architecture-best-practices-and-patterns.md#api-design "mention")  for more detailed tips

### Document the External API

Describing the external api requires a bit more care and alignment, because you control only one side of the communication. Therefor you need to align (again, in a workshop) with the owner of the external system, your system is interacting with.

It is advisable to create a separate specification for the external api, potentially even for each partnering system. For one, you dont want to expose the entirety of your internal api. In addition, the requirements and particularities of you internal and external apis might be different.

Often it is also useful to create sequence diagrams for the external communication. This will help you identify bottlenecks and (hidden) dependencies. A sequence diagram can be created easily with tools like PlantUML or diagrams.net / draw.io.

Example Sequence Diagram:

<figure><img src="../../.gitbook/assets/temp (2).png" alt=""><figcaption></figcaption></figure>
