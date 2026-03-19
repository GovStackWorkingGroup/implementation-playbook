# Architecture Design Overview

This chapter describes a process to guide you in designing an architecture for a software system. This is an opinionated proposal on how to creating an architecture. You may deviate from it at any point, but if you don't know where to start, this is a good starting point.

In designing the architecture, you depend on a lot of [#inputs](architecture-design-overview.md#inputs "mention") from the previous phases and architecture governance, while creating a range of [#outputs](architecture-design-overview.md#outputs "mention").

## Before you start

Before you start you need to establish the participants for this phase and gather the inputs required for this phase:

### Roles&#x20;

A non exhaustive list includes:

* A solution architect / technical architect - responsible for the architecture design
* The product owner - responsible for the scope of the solution
* Business architects - responsible for and familiar with the functional design of the solution
* Stakeholders from partnering systems - responsible for one or more external systems

### Inputs

* Inputs from previous phases
  * Functional Requirements
    * a domain model & context map, describing one or more bounded contexts developed inactivity [2.3-establish-the-domain-foundations.md](../design-service/2-designing-the-future-service-to-be/2.3-establish-the-domain-foundations.md "mention")
    * for example a Business Process Model, a User Journey or a [GovStack Service Blueprint](https://www.figma.com/board/DAK1g4cpOaBYIEh86jrSaf/Service-Blueprint-Template?node-id=0-1\&p=f)
    * ideally a Functional Data Model (if available)
    * any design documents created during the previous phases
  * Non-Functional Requirements
  * UX Guidelines (if available)
    * for example wireframes, styleguide
    * UX Flow Guidelines (example: user should move through steps sequentially or should be allowed to jump between steps as he likes)
  * Proposed Building Blocks (optional)
* Other Inputs
  * Overarching [#governance-of-the-architecture](architecture-design-overview.md#governance-of-the-architecture "mention")
* The System Landscape Diagram (if it already exists)
  * An overview of Building Blocks already used in the organization
* GovStack Building Block Specifications
  * Additional documentation of existing instances of Building Blocks (if available)
* API specification of external systems

## Criteria for success

### Outputs

At the end of this process you will have produced a few artifacts, with the purpose of guiding the later phases, like Implementation, Operations & Maintenance. Those artifacts include:

* an (updated) System Landscape Diagram
* a Software Architecture, documented in System Context, Container & Component Diagrams
* a technical data model
* the api specification
* a technology stack
* developer guidelines

Designing an architecture is an ongoing and iterative process though, so expect to update & evolve the architecture regularly throughout the lifecycle of the software system.

## Use the C4 Model

This guide recommends to use the C4 model and uses it in its examples.

Using a model like C4 helps by providing a clear terminology. Terms like system, container or component are vague, overused and have different meaning in different contexts.

The C4 model is lightweight and easy to understand, even without a lot of training or experience. It only uses a few types of diagrams, some of which are even optional.

You can find a detailed introduction under:

* [Home | C4 model](https://c4model.com/)
* [Visualising software architecture with the C4 model - Simon Brown, Agile on the Beach 2019 - YouTube](https://www.youtube.com/watch?v=x2-rSnhpw0g\&t=1s)

### C4 Terminology

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption><p>Adapted from https://c4model.com (CC BY 4.0). Changes made.</p></figcaption></figure>

### Overview of C4 diagrams

<figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption><p>Adapted from https://c4model.com (CC BY 4.0). Changes made.</p></figcaption></figure>

### Sources

* [C4 model Home](https://c4model.com)
* [C4 Model Introduction on YouTube](https://www.youtube.com/watch?v=x2-rSnhpw0g)

## Governance of the Architecture

Architecture governance ensures that digital solutions are not developed in isolation, but are consistently aligned with the overarching Government Architecture and its strategic objectives. It provides the decision-making and control mechanisms that translate architectural principles into enforceable rules across design, implementation, and operation (see the “Government architecture” chapter for detailed guidance). In practice, architecture governance operationalises the Government Architecture by mandating the use of approved building blocks, shared standards, and common technology stacks. This includes compliance with defined APIs, data models, data formats, interoperability standards, and security requirements, ensuring coherence across application, data, and technology layers.

At the same time, architecture governance acts as a critical enabler of interoperability. By embedding legal, organisational, semantic, and technical interoperability requirements into architectural decision-making, it ensures that systems can effectively exchange data and services across institutional and jurisdictional boundaries. This aligns closely with the interoperability governance principles described in the Interoperability chapter and the layered approach of the European Interoperability Framework (see the “Interoperability chapter” for detailed guidance).

Architecture planning serves as the practical bridge between governance and implementation. Through architecture planning activities - such as capability mapping, dependency management, and standards selection - governance rules are translated into concrete architectural roadmaps. This ensures that interoperability considerations and Government Architecture principles are addressed early, reducing fragmentation, duplication, and costly rework later in the lifecycle. In most cases, referencing existing governance frameworks and architectural guidelines is sufficient. However, any deviation from agreed architectural principles or interoperability standards should be identified early and discussed with the responsible governance bodies to safeguard alignment, sustainability, and cross-government coherence.

More recommendations on [design-a-government-architecture.md](../../strategy-and-management/design-a-government-architecture.md "mention")

{% include "../../.gitbook/includes/todo-check-for-potential....md" %}

In almost all cases, the organisation’s governance framework or architectural guidelines should be followed as closely as possible. Any deviation should be flagged early and discussed with the responsible governance bodies to avoid rework later in the project.&#x20;
