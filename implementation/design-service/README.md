# Design Service

Design and deliver government services that work, using GovStack tools and patterns.

Reduce the risk of building the wrong thing by understanding the service domain and user needs early, testing ideas quickly, and by iterating and improving.

## The service development phases

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

Each phase answers specific questions and produces artefacts that inform the next.

The phases:

* **Start by understanding the problem (Discovery)** before proposing solutions
* **Clarify future intent (Define the to-be)** before investing in detailed design or build
* **Test and learn** before committing to full-scale delivery
* **Align service intent with technical reality (Architecture planning)** before development
* **Build, operate, and improve (Develop)** as an ongoing cycle

Movement between phases is guided by confidence and evidence, not by completing every activity. Teams may:

* Loop back to previous activities when new insights emerge
* Run phases in parallel for different parts of a service
* Revisit earlier artefacts as assumptions change

<mark style="color:$danger;">\[Diagram emphasising the looping back]</mark>

Each phase ends with a set of deliverables that help teams decide whether they are ready to move forward, pause, or revisit earlier work.

<details>

<summary><strong>Discovery</strong></summary>

Build a shared understanding of the problem space before committing to solutions.

In this phase, teams explore:

* user needs and service context
* existing systems, actors, and dependencies
* constraints, risks, and assumptions

The aim is to agree **what problems are worth solving**, for whom, and why.

Deliverables:

* Clear problem statement(s)
* Initial user needs and priority groups
* As-is user journey(s)
* Stakeholder and ecosystem map
* Known constraints, risks, and assumptions

</details>

<details>

<summary><strong>Define the To-Be</strong></summary>

Agree what the future service should achieve and how it should work at a high level.

In this phase, teams:

* describe the intended future experience
* generate and explore service concepts
* establish shared foundations such as domain language, data concepts, and boundaries

The aim is to create enough clarity and alignment to guide delivery decisions.

Deliverables:

* To-be service vision or narrative
* High-level to-be user journey(s)
* Service principles or success measures
* Domain glossary and shared language
* Initial data concepts and boundaries

</details>

<details>

<summary><strong>Test and Learn</strong></summary>

Reduce uncertainty before full-scale development.

In this phase, teams:

* prototype and test ideas with users and stakeholders
* validate assumptions and hypotheses
* learn what works (and what does not)

The aim is to use evidence to refine direction and avoid costly mistakes later.

Deliverables:

* Prototypes (low- or high-fidelity)
* Documented assumptions and hypotheses
* Evidence from user testing or pilots
* Refined service concepts and journeys
* Clear decisions on what to proceed with (or stop)

</details>

<details>

<summary><strong>Architecture Planning</strong></summary>

Translate the intended service into a clear, feasible technical approach.

In this phase, teams align service intent with delivery realities by:

* confirming what systems and building blocks are needed
* agreeing integration and interoperability approaches
* exploring ownership, procurement, and operational responsibilities
* identifying technical risks, constraints, and dependencies early

The aim is to create shared clarity across product, design, delivery, and technical stakeholders before development begins.

Deliverables:

* High-level service architecture
* Identified GovStack building blocks and integrations
* Data flows and system boundaries
* Delivery and ownership assumptions
* Key technical risks and mitigation approaches

</details>

<details>

<summary><strong>Development</strong></summary>

Build and integrate the service in a secure, accessible, and scalable way.

In this phase, teams:

* translate service intent into working systems
* integrate GovStack building blocks and other components
* ensure quality, security, and performance

Service design continues to support decision-making as technical and operational choices are made.

Deliverables:

* Working service components
* Integrated systems and interfaces
* Accessibility, security, and quality checks
* Updated service journeys reflecting build decisions

</details>
