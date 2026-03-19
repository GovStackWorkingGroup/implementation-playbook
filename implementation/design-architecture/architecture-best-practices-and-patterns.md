# Architecture Best Practices & Patterns

Below are some proven Best Practices for designing an architecture. Treat this as a pick & choose menu of recommendations. Additional best practices recommended by GovStack can be found here: [Architecture and Non-Functional Requirements](https://specs.govstack.global/architecture/6-cross-functional-requirements)

## Documentation

* This guide assumes and recommends that you use lightweight and free tools / methods to document your architecture
  * Use [C4 model](https://c4model.com)[Home | C4 model](https://c4model.com)
  * Use [PlantUML](https://plantuml.com)[Open-source tool that uses simple textual descriptions to draw beautiful UML diagrams.](https://plantuml.com)
  * Use [OpenAPI](https://www.openapis.org/what-is-openapi) [What is OpenAPI? – OpenAPI Initiative](https://www.openapis.org/what-is-openapi)
* Use ADR (Architecture Decision Records)
  * Architecture Decision Records are a lightweight way of documenting your decisions. There are a lot of templates available to choose from
  * Sources
    * [Architectural Decision Records (ADRs) | Architectural Decision Records](https://adr.github.io)
    * [9 - Architecture decisions | arc42 Documentation](https://docs.arc42.org/section-9/)

## Data Model

* Use UTC timestamps
  * Date, Time & Timezones are frequent error sources in software systems. Normalize all your timestamps and store them as UTC timestamps in your persistence layer. Only adapt them to specific timezones when displaying to the user.
* Use UUIDs for technical primary keys
  * Using technical primary keys and using UUIDs to represent those has a range of benefits.
  * Sources
    * [Primary Keys: IDs versus GUIDs](https://blog.codinghorror.com/primary-keys-ids-versus-guids/)
    * [UUID as a Primary Key in Databases: Advantages, Challenges, and Best Practices - DEV Community](https://dev.to/adityabhuyan/uuid-as-a-primary-key-in-databases-advantages-challenges-and-best-practices-3koi)
* But still keep natural business keys
  * Using UUIDs as recommended above, does not prevent you from also using natural business keys. Some systems allow to use both like Spring/Hibernate's `@Id` and `@NaturalId`.
* Use staging tables for bulk data
  * When handling bulk data (uploads, batches, interfaces with high volumes / large payload), it is best to first store it in its original form without manipulating it (or as close to that as possible). Use dedicated staging tables for that.
  * Having staging tables allows you to
    * analyze the data in its original form, in case of errors
    * distribute the load of processing the data
    * retrigger the processing of the data

## Business Components

* Use Data Transport Objects or Domain Objects
  * You should define dedicated data objects for the domain layer or access layer
  * Those object allow a representation specifiv to the bounded context / domain model
  * Avoid working directly on entities provided by the persistence layer
* Use the Data Repository per Aggregate Pattern
  * Use Repositories to access the persistence layer
  * Create one Repository per Aggregate of Entities: [Repository per Aggregate of Entities](https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/infrastructure-persistence-layer-design)&#x20;
    * A more technical description: [Aggregates and Repositories in Domain-Driven Design](https://softwarepatternslexicon.com/java/domain-driven-design-ddd-patterns/tactical-patterns/aggregates-and-repositories/)
