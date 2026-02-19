# Design a Government Architecture

The following content is a summary of the Public Administration Ecosystem Reference Architecture (PAERA) document and the TOGAF methodology by the Open Group. More detailed information can be found here: [https://specs.govstack.global/paera](https://specs.govstack.global/paera).

## What is government architecture?

To understand why Government Architecture is essential, it is necessary to clarify what it encompasses and what distinguishes it from traditional approaches to digitization.

**Government architecture** (often referred to as Government Enterprise Architecture, GEA) is a **whole‑of‑government approach** (see the chapter “Set Foundations for Interoperability” for detailed guidance) that **aligns policy goals, operating models, data, applications, and technology into** a **coherent, governed ecosystem** for delivering coordinated, efficient, and equitable public services. It bridges the vocabulary and priorities of governance leaders and IT professionals to sequence digitalization in a way that reduces risk, avoids waste, and builds institutional capability over time.

Hence, Government Architecture can be defined as the structured description and intentional design of how a government operates as an integrated system. It creates a shared frame of reference that connects public mandates, organizational structures, service delivery, data flows, digital systems, and enabling infrastructure. Rather than focusing on individual solutions, Government Architecture focuses on relationships and dependencies.

Crucially, Government Architecture differs from conventional IT architecture. It does not start with systems or technologies, but with public value creation. Legal obligations, societal goals, and governance constraints are treated as architectural inputs rather than external limitations. As a result, Government Architecture becomes a strategic capability that shapes how governments prioritize investments, manage risk, and coordinate transformation across the public sector.

More importantly, Government Architecture introduces a long-term perspective. Public sector systems must endure across political cycles, legal reforms, and technological change. Decisions taken today, particularly in the design of digital systems, can shape administrative capacity and citizen trust for decades. Government Architecture therefore acts as a stabilizing mechanism, ensuring that transformation efforts are cumulative, sustainable, and aligned with public interest.

**In PAERA**, **government architecture** is **positioned as** a **reference architecture** (see figure below) for the public ad-ministration ecosystem.

More specifically, a **reference architecture** is the **blueprint** used to **put the pieces of** the **organizational & systems puzzle together**. Digital teams use reference architecture to promote the reuse of common assets and identify capability gaps. It:&#x20;

* Defines a common language for consistent communication within the organization
* &#x20;Outlines all capabilities needed to achieve the best outcome&#x20;
* Provides the ability of systems or software to exchange and make use of information &#x20;
* Establishes standard systems, and a common way to exchange information

<div align="left"><figure><img src="../.gitbook/assets/Reference Architecture graphic.png" alt=""><figcaption><p>Reference Architectures and Solution Enterprise Architectures;  Source: Adapted from “IT Connect. Information technology tools and resources at the UW” (Univ. of Washington, 2020)</p></figcaption></figure></div>

In PAERA specifically, the reference architecture explains the interactions between enterprise architecture practices and the GovStack “Building Block” approach so that high‑level leaders can see dependencies across the ecosystem while technical teams understand scope, sequencing, and the constraints under which digital transformation succeeds.

### Example: Australian government architecture

The following example illustrates how the principles described above are operationalized in practice: Australia's [reference architecture document](https://www.architecture.dta.gov.au/sp_aga2?id=aga2_how_to_use) structures capabilities and technologies into an orchestrated ecosystem that enables consistent digital service design and delivery (see figure & YouTube video below).

<figure><img src="../.gitbook/assets/20230118 - DCM visual for web - 18 Jan &#x27;23-1.jpg" alt=""><figcaption><p>Source: Australian <a href="https://architecture.digital.gov.au/sites/default/files/2023-07/22-0109%20Australian%20Government%20Architecture_v11.pdf">Reference Architecture</a></p></figcaption></figure>

{% embed url="https://youtu.be/NSBtgW09mHo" %}
Australian Whole of Government Architecture &#x20;
{% endembed %}

### GovStack's perspective on government architecture

Building on this understanding of Government Architecture as a strategic and systemic discipline, the GovStack initiative offers another concrete perspective on how architectural principles can be applied in practice to design, implement, and scale digital government solutions.

GovStack is a global initiative designed to consolidate leading digital government practices derived from real-world implementations across diverse country contexts. Its core ambition is to establish a standardized reference architecture composed of interoperable digital Building Blocks that underpin a modern Digital Government operating model.

By providing open access to these Building Blocks, GovStack creates a common platform where technology providers and developers can align directly with the needs of public-sector institutions. In doing so, GovStack effectively bridges the gap between governments striving to modernize their service delivery and the market actors capable of supplying scalable, high‑quality digital components.

The GovStack methodology is grounded in a modular building‑block approach, fully aligned with the whole‑of‑government principles (see the chapter “Establish Interoperability” for detailed guidance) articulated in the SDG Digital Investment Framework. This ensures that digital transformation efforts remain coherent, sustainable, and strategically linked to development outcomes.

To operationalize this methodology, GovStack has developed the Public Administration Ecosystem Reference Architecture (PAERA) (see figure below). PAERA provides governments with a structured, practical framework to guide digital transformation in an efficient, effective, and sustainable manner, supporting end‑to‑end redesign of public services and enabling long‑term institutional capacity building.

<div align="left"><figure><img src="../.gitbook/assets/GovStack Methodology.png" alt=""><figcaption><p><em>(GovStack methodology components</em> <em>(PAERA)) (PAERA, 2025)</em></p></figcaption></figure></div>

### The role of TOGAF in government architecture

Within the GovStack and PAERA reference-architecture context, the question shifts from what needs to be designed to how architecture work can be structured and governed within public sector organisations. In this regard, established Enterprise Architecture methodologies can complement GovStack by providing structured methods for organizing architecture activities at the organizational level. One such methodology is “The Open Group Architecture Framework” (TOGAF), which is widely used to support the development, management, and evolution of enterprise architectures over time.&#x20;

Its Architecture Development Method (ADM) provides an iterative lifecycle for analysing current states, defining target architectures, and planning transition paths in a controlled manner (see figure below):

<div align="left"><figure><img src="../.gitbook/assets/TOGAF Framework.png" alt=""><figcaption><p><em>The TOGAF Framework (The Open Group, 2025)</em></p></figcaption></figure></div>

More specifically, when using TOGAF as a supporting enterprise architecture method, organizations can structure their architecture as follows:

* **Establish architecture governance (Preliminary & A):** Assign clear ownership and define a shared architecture vision aligned with laws, policies, and public value.
* **Model mandates and processes (B):** Describe business capabilities and processes based on legal responsibilities, not organizational silos.
* **Define data and services (C):** Clarify data ownership, information flows, and reusable digital services across the organization.
* **Set technology standards (D):** Align infrastructure and security choices with national digital infrastructure.
* **Plan incremental change (E–F):** Prioritize architectures into feasible initiatives that fit budget cycles and organizational capacity.
* **Control execution and evolution (G–H):** Ensure compliance with the architecture and continuously adapt it as laws, services, and technologies change.

In digital government contexts, TOGAF is particularly relevant because it emphasizes governance, stakeholder alignment, and incremental change-characteristics that align well with the realities of public administration.&#x20;

However, TOGAF is a generic enterprise architecture method and is not specific to the public sector or to Digital Public Infrastructure.

Within GovStack implementations, TOGAF should therefore be understood as a complementary methodology, not as a reference architecture. It can be used by government organisations to structure architecture activities, define governance processes, and manage transitions between architectural states. PAERA, in contrast, provides the public-administration-specific reference architecture, including dependency models, architectural viewpoints, and implementation sequencing tailored to digital government.

In practice, this means that governments may use TOGAF to organise how architecture work is carried out, while PAERA defines what needs to be considered and which architectural conditions must be in place to enable sustainable digital government transformation.

### Four different points of view

Beyond methodological considerations, Government Architecture requires a structured way to describe the public administration as a system, which is commonly achieved through four complementary architectural points of view. These viewpoints should be developed iteratively and kept synchronized through governance:

<details>

<summary><strong>1.Business architecture:</strong></summary>

* **What it covers:** Business Architecture describes how the organization delivers value and how it is structured to achieve its mission. It looks beyond the customer service relationship to include:
  * Public services and service delivery models
  * Business processes and workflows
  * Laws, regulations, and administrative rules
  * Organizational roles and responsibilities
  * Performance indicators and policy outcomes&#x20;
* **Purpose:** It shows what the organization does, why it does it, and under what constraints. This understanding is crucial for designing services that are lawful, feasible, and aligned with public mandates.
* **Associated Building Block:** A Business Architecture Building Block is a set of recommended legal, organizational, and governance arrangements required to support specific public services.&#x20;

</details>

<details>

<summary><strong>2.Application architecture:</strong></summary>

* **What it covers:** Application Architecture describes the software landscape that supports business processes. It identifies:
  * All applications used across departments
  * Their functions, dependencies, and integration points
  * How applications support service delivery and internal processes&#x20;
* **Purpose:** It clarifies which systems enable which processes, prevents duplication, and highlights integration needs – particularly important in large public administrations with heterogeneous software portfolios.
* **Associated Building Block:** An Application Architecture Building Block is a separately deployable software component defined by:
  * A clear API/interface
  * A specific functional scope
  * Reusable capabilities that can be invoked by multiple services

</details>

<details>

<summary><strong>3.Data architecture:</strong></summary>

* **What it covers:** Data Architecture defines the organization’s information assets, including:
  * Data models and classifications
  * Registries and core datasets
  * Data flows across institutions
  * Rules for storing, sharing, securing, and using data
  * Metadata, definitions, and documentation &#x20;
* **Purpose:** It ensures the organization understands the data it collects and uses. This is essential for:
  * Evidence‑based decisions
  * Performance management
  * Personalization of services
  * Automation and interoperability&#x20;
* **Associated Building Block:** A Data Architecture Building Block specifies:
  * Required state registries and information repositories
  * The business capabilities these datasets enable (e.g., identification, licensing, taxation)

</details>

<details>

<summary><strong>4.Technology architecture:</strong></summary>

* **What it covers:** Technology Architecture describes the technical infrastructure that enables the use of digital services, including:
  * Computing platforms (servers, cloud infrastructure)
  * Networking and connectivity
  * Storage systems
  * Security mechanisms and protocols
  * Tools for system operations, monitoring, and scaling&#x20;
* **Purpose:** It defines the technical foundation needed to run mission‑critical government services securely, reliably, and at national scale.
* **Associated Building Block:** A Technology Architecture Building Block is an implementation pattern recommended for providing secure, scalable, and resilient ICT infrastructure services.

</details>



## Core components of a digital government

While architectural viewpoints describe what needs to be considered, effective Government Architecture also requires clarity on where different types of decisions are made. Digital government therefore operates across multiple, interconnected levels, each with distinct responsibilities and dependencies.

In fact, digital governance can be understood through the metaphor of a building. While buildings may differ across cultures, the underlying construction principles remain consistent. Any structure starts with a solid foundation. In Digital Governance, this foundation consists of cross-cutting governance, policy, and legislative elements. These elements support higher-order structures, following a clear causal logic in which foundational inputs enable subsequent governance capabilities. These inputs are referred to as the underlying conditions for Digital Governance (see figure below).

<figure><img src="../.gitbook/assets/Updated Interoperability house.png" alt=""><figcaption><p><em>(Public Administration Ecosystem Reference Architecture (PAERA)), (Source: Ivar Tallo &#x26; Aare Lapõnin)(PAERA, 2025)</em></p></figcaption></figure>

More specifically, within the GovStack framework, attention is placed on the Foundational, Na-tional, and Organizational Layers. The Foundational and National layers together form the Digital Governance Infrastructure, providing the underlying conditions for digital government. The Or-ganizational layer builds on this infrastructure by enabling institutions to operationalize and sus-tain digital transformation. The following sections examine these layers in depth and describe their role in enabling sustainable digital government implementations.

### Foundational level

At the base of the system lies the foundational level. This level consists of horizontal prerequisites that apply across all digital initiatives, including legal frameworks, governance arrangements, policy coordination mechanisms, and common standards. Without these foundations, digital solutions remain isolated and difficult to scale. Foundational components provide legitimacy, accountability, and coordination, ensuring that digital transformation is anchored in law and policy rather than driven solely by technical feasibility.

### National level

Building on the foundation, the national level focuses on Digital Infrastructure pillars that enable system-wide interoperability. These include connectivity, digital identity, digital data, and interoperability mechanisms. The pillars should be understood as shared public capabilities comparable to foundational state infrastructure with the purpose of reducing coordination effort across government. While service development can begin before all pillars are fully in place, failure to address them early creates structural bottlenecks that are costly and complex to resolve later.

### Organizational level

At the organisational level, digital government shifts from infrastructure to institutional capability: While national digital infrastructure enables interoperability, individual ministries and agencies determine whether it produces real public value. Each organisation must therefore develop managerial ownership of digitalisation, maintain an enterprise architecture, redesign services rather than merely digitise existing processes, and embed data into decision-making. This also requires legal recognition of digital procedures, appropriate governance and procurement models, as well as collaboration with external actors such as citizens and private providers. Because public administrations operate under legislation, political mandates, and rigid responsibilities, transformation demands coordinated change across roles, skills, culture, and communication, often led by a dedicated digital leadership function (see more in-depth information [here](https://paera.govstack.global/4.-organisation-level)). Different types of public bodies – policy-making, regulatory, and service-delivery organisations – implement these capabilities differently, but all rely on the same shared infrastructure; consequently, the organisational level ultimately determines whether national digital foundations translate into effective public services.



## Change management

Building on the foundational, national, and organizational layers outlined above, effective digital transformation requires a structured change management approach across all levels of government. Change management is often associated with modernization initiatives at the organizational level; however, government-wide transformation must be addressed as well. Such initiatives are typically implemented as reforms driven by political priorities. Digital transformation, as a core reform, needs to be aligned with the government’s vision, policy agenda, and supporting legal framework.

More specifically, the GovStack approach can only be implemented within a systematic practice of change management across government and organizational levels:

* National digital infrastructure capabilities should be planned and developed across central, regional, and municipal levels in line with policy objectives.
* Organizational capabilities should be developed within ministries, departments, and agencies (MDAs) across the public sector.
* A practice should be initiated that supports the implementation of projects from legal and administrative perspectives
* Government internal IT capabilities should be established to manage the sustainable delivery of software solutions for digital services.

### Quality attributes of the process

After addressing the importance of change management in guiding institutions through digital reform, the next step is to clarify the standards that should shape the transformation process itself. GovStack stresses that digital transformation will produce a new Digital Public Infrastructure (DPI) (see the chapter “Build a Digital Public Infrastructure” for detailed guidance), and its development must be guided by well‑defined outcomes and a process rooted in public needs. To achieve this, the process must meet several essential quality attributes, illustrated below:

<figure><img src="../.gitbook/assets/Updated attributes graphic.png" alt=""><figcaption><p><em>(Requirements for Digital transformation process</em> <em>(PAERA)) (PAERA, 2025)</em></p></figcaption></figure>

Together, these attributes ensure that digital transformation efforts create sustainable public value rather than short-term efficiency gains.

* **Purpose and Directionality:** Within a common-good framework, clear direction-setting and effective orchestration are critical capabilities. There is increasing demand for explicit directionality in the development of shared digital infrastructure. As DPI is not neutral and directly shapes downstream solutions, its intended direction must be made explicit and appropriately prioritized.
* **Co-creation and participation:** A common-good approach emphasizes collaboration, coordination, and co-investment among multiple stakeholders. Co-creation and participation should therefore be embedded in governance processes and supported by formal institutional mechanisms. Participation is more challenging in environments dominated by proprietary technologies.
* **Collective learning and knowledge-sharing:** Systematic learning from successes and failures, combined with structured knowledge sharing, is essential for collective value creation. Institutionalized learning strengthens long-term state capabilities and can be enabled through innovative institutional arrangements.
* **Access for all and reward-sharing:** Universal access and equitable benefit sharing are core to the common-good principle. Infrastructure that creates societal value must be accessible to all, with benefits broadly shared. Governments therefore prioritize access and inclusion over market-based pricing or rent extraction. Where digital access is not yet universal, analogue channels remain essential to avoid excluding citizens.
* **Transparency and accountability:** Transparency and accountability are critical for building trust in DPI initiatives. While decentralized architectures increase accountability complexity across government entities, they also create opportunities to enhance transparency when governed effectively.



## How to implement the Government Architecture

Having established the conceptual and structural foundations, the final question is how Govern-ment Architecture can be implemented in practice.

### Capability assessment

Implementation begins with a realistic assessment of existing capabilities. Governments must understand their current maturity across leadership, architecture practices, service delivery, data governance, and digital skills. Capability assessment provides a baseline that informs sequencing and prevents overambitious implementation plans.

GovStack supports a staged maturity model that structures transformation as a progressive journey, ensuring that capabilities are internalized before more advanced initiatives are pursued (see figure. below):

<figure><img src="../.gitbook/assets/Capability Assessment.png" alt=""><figcaption><p><em>(Public Administration Ecosystem Reference Architecture (PAERA)) (Source: Aare Lapõnin) (PAERA,2025)</em></p></figcaption></figure>

To translate the model into practice, the following sections walk through each stage of the ma-turity journey and describe how organizations evolve across levels.

<details>

<summary>Ground Floor</summary>

If an organization has never implemented any automation project, we can say that it is on the ground floor. The **ground floor, in terms of capabilities, means**:

* The management did not plan for IT systems to deliver services or support activities.
* There is no organizational architecture document that describes the business, data, application, and technology used by an organization.
* An organization does not deliver digital services to external customers.
* Management is not using its operational data systematically to make decisions regarding strategic options for the organization.
* The organization has never procured IT system development and management services from a market.



Once you are **on the ground floor, you should**:

* Make sure there is connectivity for your organization and your customers.
* Start with small projects, which should have a small budget and delivery timeline, at most 6-9 months.
* Prepare plans for how users will be trained to use the new system, what administrative procedures you need to support a new way of working, and how the latest IT system will be supported.
* Start cultivating a digital culture in an organization&#x20;



The following **important rules should be considered:**

* A New IT system is a liability, and you have to plan maintenance costs for the entire lifecycle of the planned solution.
* There will be digital data, and you should have procedures for managing the lifecycle of the digital data.
* There should be a unit in charge of digital transformation that is able to report and escalate to the management of the organization.
* It is important to note that if the staff has experience in digital transformation from other organizations but has yet to deliver any project as a team, then this organization starts from the ground floor.

</details>

<details>

<summary>1st Level - Tust of Data</summary>

An organization is considered to have reached the **first level once a foundational level of trust in digital systems and data** has been established. At this stage, the following capabilities are in place:

* **Management and Culture:** Management conducts regular planning cycles to assess, prioritize, and commit to IT investments aimed at improving operations. A digital culture is actively promoted across the organization.
* **Architecture Management:** A formal architecture management process exists to document business services, processes, data, applications, integrations, and technology components. This process aligns business and IT stakeholders and supports structured decision-making.
* **Digital Service Delivery:** Digital services are delivered to external users through established IT development, maintenance, and IT service management capabilities aligned with ITIL principles. The design and operation of digital services are carried out collaboratively by business owners and IT teams.
* **Data-Driven Decision-Making:** Organizational data, including operational logs and monitoring metrics, is consolidated in a reliable enterprise data warehouse. Management dashboards and reports support both operational and strategic decisions, while self-service analytics are available to analysts. Data semantics are defined through metadata, supported by a data quality management process, enabling growing trust in data and increased data-driven decision-making.
* **Digital Co-creation:** The organization is able to procure specialized services from the market to ensure high-quality digital service delivery and has established channels to collect customer feedback on digital services.



To **further progress beyond the first level**, **organizations should focus** **on** the **following** **actions**:

* Continue implementing small to medium-sized initiatives with controlled budgets and delivery timelines of up to 12 months.
* Develop a comprehensive roadmap for the full digitalization of organizational activities, typically articulated through an IT strategy covering a 3–5 year horizon.
* Establish a centralized enterprise architecture repository to support detailed planning of modernization initiatives.
* Introduce a dedicated enterprise architecture management team to ensure sustained alignment between business and IT.

</details>

<details>

<summary>2nd Level - Process Management</summary>

An **organization** is considered to have **reached the second level** **once** **all first-level capabilities** are **fully established** **and** the **following** additional **conditions** are **met**:

* **Management and Strategic Control:** Service level agreements (SLAs) are defined for all business services delivered to external users and are regularly reviewed by management, with corrective actions taken where deviations occur. Key performance indicators (KPIs) are established for all internal business processes and continuously monitored. A structured strategic management process systematically analyzes changes in the internal and external environment and proactively informs improvement initiatives for service quality and process efficiency. This process is fully aligned internally with IT management and externally with the government budget cycle. A senior executive with clear accountability for digital transformation is in place.
* **Architecture Management:** The organization has in-house capabilities to plan and optimize service delivery for improved efficiency. Enterprise architecture enables end-to-end traceability of operational and IT risks, supported by defined mitigation plans. A continuous rationalization process reduces application complexity and technical debt across the application and technology landscape.
* **Digital Service Delivery:** All core and support processes are fully digitalized, following a digital-first-by-design approach. Digital literacy is a mandatory competency across all roles.
* **Data-Driven Decision-Making:** Data product development and usage are mature and systematic. Data architecture is designed to meet both current and long-term organizational needs, with reliability and quality as top priorities. Application architecture is aligned with data architecture, ensuring architectural stability. All decisions are based on high-quality digital data.
* **Digital Co-creation:** Digital services are increasingly integrated into customers’ existing digital environments to enable seamless and efficient information exchange.



**To progress beyond** the **second level**, **organizations** **should focus** on the **following actions:**

* Deliver well-scoped initiatives with limited budgets, clear objectives, and delivery timelines of up to 18–24 months.
* Strengthen the resilience of digital service delivery, including the implementation of comprehensive business continuity management.
* Improve integration of business process ownership and product management with architecture management processes.
* Introduce program management disciplines to systematically manage long-term transformation objectives.
* Ensure procurement processes are sufficiently flexible to address complex initiatives where outcomes cannot be fully specified upfront.

</details>

<details>

<summary>3rd Level - Change Management</summary>

An organization is considered to have **reached the third maturity level once all second-level capabilities** are fully **established** and the following **additional conditions** **are** **met**:

* **Management and Change Enablement:** The organization has the capability to assess the impact of relevant policy changes and to develop and execute comprehensive change management plans through appropriate organizational units. This enables the organization to absorb and implement frequent policy changes in a structured and timely manner.
* **Architecture Agility:** Enterprise architecture is proactively designed to enable rapid and flexible implementation of changes driven by policy shifts or external environmental developments.
* **Digital Service Resilience:** A mature business continuity management framework ensures the sustained resilience and reliability of digital service delivery.
* **Policy-Driven, Data-Supported Decisions:** Data capabilities proactively support policy impact analysis and requirements definition.
* **Digital Co-creation and Sustainability:** Long-term sustainability of IT systems is ensured through the consistent design and implementation of solutions based on GovStack architectural Building Blocks.



**To continue progressing** at this level, **organizations** **should** **focus** **on** the **following actions:**

* Deliver small, well-defined initiatives with limited budgets, clear objectives, and delivery timelines of up to 18–24 months, structured as part of broader programs targeting strategic outcomes.
* Systematically monitor the external environment, international best practices, and technological developments, and regularly update organizational strategies to incorporate relevant innovations.

</details>

<details>

<summary>4th Level - Compliance Management</summary>

An **organization** is **considered** to **have reached** the **fourth maturity level once all third-level capabilities** are fully **established** **and** the **following additional conditions** are **met**:

* **Management and Policy Leadership:** The organization is able to proactively propose policy changes to improve outcomes within its mandated domain.
* **Strategic Architecture Management:** Architecture management is fully embedded within the organization’s strategic management processes, enabling continuous alignment between strategy, policy, and execution.
* **Digital Service Ecosystem Integration:** The organization can seamlessly adapt digital service delivery in line with strategic priorities. Its digital platform operates as an integrated component of the national digital ecosystem.
* **Advanced Data-Driven Value Creation:** Data products are proactively delivered to internal and external stakeholders. Structured feedback loops with data consumers are in place and systematically used to inform data product management and improvement.
* **Digital Co-creation and Platform Governance:** The organization manages its digital platform as a two-sided market, open to product providers and users. Formal governance processes ensure quality control, onboarding, and lifecycle management of platform-based products.

At this level of maturity, continuous monitoring of the external environment, international best practices, and technological advancements remains essential. Organizational strategy should be regularly updated to incorporate relevant innovations and sustain long-term impact.

</details>

### Key underlying principles&#x20;

Throughout implementation, Government Architecture must remain anchored in fundamental governance principles. These include – the rule of law, whole-of-government coordination, transparency and accountability, human-centric service design, and security and privacy by design – and ensure that architecture serves democratic governance and public trust.

Regulations and policies should adhere to the following principles:

<details>

<summary>Rule of Law and Human Rights Orientation:</summary>

Regulations must be grounded in the rule of law, with explicit priority given to human rights and the United Nations Sustainable Development Goals (SDGs). The rule of law im-plies that individuals, institutions, and governments are equally subject to and accounta-ble under a coherent system of international and domestic law, rather than arbitrary deci-sion-making. In a digital context, legal frameworks should promote a human-centric state, safeguard digital-era human rights, prevent technology-driven barriers, and minimize the risk of state abuse, such as excessive data collection, discrimination, or rights violations. Human-centered digital regulation strengthens public trust, increases civic engagement, and ensures that technology serves societal well-being.

</details>

<details>

<summary>Whole-of-Government:</summary>

Government entities should operate in a coordinated and integrated manner across min-istries, agencies, and levels of government to achieve shared objectives. Digital systems and services should be interoperable by design to enable seamless, end-to-end service de-livery across institutional boundaries.

</details>

<details>

<summary>Digital by Default:</summary>

Digital channels should be the primary mode of public service delivery, while traditional channels remain available to ensure inclusiveness.

</details>

<details>

<summary>No Legacy:</summary>

Processes should be fundamentally rethought and redesigned to fully leverage digital technologies, rather than replicating legacy workflows in digital form.

</details>

<details>

<summary>Once-Only Principle:</summary>

Citizens and businesses should provide information to the government only once. Data should be reusable across public institutions, supported by proactive information sharing and transparent processes and decision-making.

</details>

<details>

<summary>User-Centric Government:</summary>

Public services should be designed around user needs and experiences, adopting an out-side-in perspective.

</details>

<details>

<summary>Natural Digital Environment:</summary>

Public administrations should aim to deliver digital services directly within users’ existing digital environments.

</details>

<details>

<summary>Public-Private Co-creation:</summary>

Governments should actively engage the private sector in the co-creation of digital public services, based on mutually beneficial collaboration models.

</details>

<details>

<summary>Cross-Border by Default:</summary>

Public services should be designed to serve users regardless of geographic location.

</details>

<details>

<summary>Intrinsic Security and Privacy: </summary>

Security and privacy must be embedded into systems by design and by default, rather than added retrospectively.

</details>

### Recommended roadmap

With the principles, layers, and capabilities defined, the focus now shifts to implementation. The recommended roadmap translates the Government Architecture into a practical, phased sequence of actions that progressively establishes governance, infrastructure, and organizational capacity while enabling interoperable services to scale over time (see figure below).

The roadmap serves as a practical guide for sequencing government digital transformation, illustrating how capabilities and GovStack Building Blocks should be introduced step by step across the four implementation phases. The four phases are: &#x20;

_Suggested phasing for implementation of BBs_

<figure><img src="../.gitbook/assets/Updated Implementation PAERA graph.png" alt=""><figcaption><p><em>(PAERA, 2025)</em></p></figcaption></figure>

**Phase 1: Inception**

* Assess national digital capabilities and establish governance, legal alignment, and change-management structures.
* Launch proof-of-concept services using core Building Blocks (e.g., identity, payments, low/no-code) to demonstrate value quickly.

**Phase 2: High-Priority Use Cases**

* Select and rapidly prototype priority services, then implement them with local integrators and a common portal/front-end.
* Train ministries and agencies on the GovStack approach to build awareness and adoption across government.&#x20;

**Phase 3: Initial transformation**

* Industrialise digitalisation in key sectors: deploy digital wallet/portal, digitise registries, and automate priority administrative processes.
* Align legislation and institutional processes to support scalable service delivery.

**Phase 4: Mass-Scale transformation**

* Expand to full end-to-end digital services across government using all Building Blocks and shared infrastructure.
* Enable data-driven government operations, cross-sector integration, and nationwide service availability.

A more detailed description of the phases can be found in the PAERA report ([https://paera.govstack.global/5.-implementation-framework](https://paera.govstack.global/5.-implementation-framework)).

{% tabs %}
{% tab title="Summarised activities" %}
To operationalize the Government Ecosystem Reference Architecture, governments should carry out a structured set of activities focused on reuse, standardization, and long-term sustainability:

* ﻿﻿**Develop a national systems, software, and platform catalog** to identify reusable software components/building blocks that support service digitization.
* ﻿﻿**Identify additional critical building blocks required** to establish a coherent national digital stack enabling prioritized citizen-centric services.
* ﻿﻿**Define** a **clear process** **for introducing new** or **updated building blocks** - through procurement, in-house development, or reuse of existing components (e.g., digital public goods such as those referenced in GovMarket).
* ﻿﻿**Establish governance** and **maintenance mechanisms** ensuring the architecture evolves continuously rather than remaining a static document.
* ﻿﻿**Facilitate co-design workshops** and working groups to align business, policy, and technical stakeholders around shared architectural decisions.
{% endtab %}

{% tab title="Key roles" %}
Successful implementation requires clear ownership across different professional roles:

**Chief Government Architects:**

* ﻿﻿Coordinate and steward the reference architecture across government
* ﻿﻿Ensure alignment with national digital strategy and interoperability frameworks
* Oversee governance and architectural decision-making

**Solution Architects (from government entities):**

* Co-design architecture components and building blocks
* Participate in reference architecture working groups
* ﻿﻿Contribute implementation knowledge and technical constraints
* ﻿﻿Support adoption across ministries and agencies
* Actively participate in the development of the training program

**Service Designers:**

* ﻿﻿Participate in co-design sessions to ensure services remain user-centric
* ﻿﻿Align architecture decisions with real service journeys
* ﻿﻿Help translate architecture into implementable service delivery models
* Participate in reference architecture working groups
* Actively participate in the development of the training program
{% endtab %}

{% tab title="Summarised deliverables" %}
* **Government Enterprise Architecture** **documentation**
* ﻿﻿**Implementation and adoption guidelines** for public institutions and ICT\
  providers
* ﻿﻿**Training and e-learning material** for stakeholders (e.g. public servants and ICT service providers)
* **Governance procedures** for maintaining and evolving the architecture



_**Examples of Reference Architectures:**_

* In Australia, their [reference architecture document](https://www.architecture.dta.gov.au/sp_aga2?id=aga2_how_to_use) provides digital teams the guidance they need to align current and emerging tech into a sound orchestration of solutions to enable digital government service design and delivery

<figure><img src="../.gitbook/assets/20230118 - DCM visual for web - 18 Jan &#x27;23-1.jpg" alt=""><figcaption><p>Source: Australian <a href="https://architecture.digital.gov.au/sites/default/files/2023-07/22-0109%20Australian%20Government%20Architecture_v11.pdf">Reference Architecture</a></p></figcaption></figure>

{% embed url="https://youtu.be/NSBtgW09mHo" %}
Australian Whole of Government Architecture &#x20;
{% endembed %}

* [GovStack Architecture and non-functional requirements](https://specs.govstack.global/architecture)
{% endtab %}
{% endtabs %}
