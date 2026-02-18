# B.2 - Create Container Diagram

The container diagram is a "zoomed-in" version of the [#system-context-diagram](2-start-with-the-system-context.md#system-context-diagram "mention") and shows a high-level overview of the software architecture and how responsibilities are distributed across it. Similar to the system context it defines how break down the system into different parts and how they interact with each other.

At a later step [b.4-decide-technology-stack.md](b.4-decide-technology-stack.md "mention"), you should amend the container diagram with the technology stack you decided upon.

## Container Diagram

<figure><img src="../../.gitbook/assets/image (79).png" alt=""><figcaption><p>Adapted from https://c4model.com (CC BY 4.0). Changes made.</p></figcaption></figure>

## How to do it

Most systems will follow a classical setup with

* one or more frontends
* one or more backends
* some kind of persistence, like a database

With that in mind you should review all incoming & outgoing connections from / to external systems. This will inform you about containers like frontends, adaptors, proxies, batches or else. You should also check whether async communication should be buffered via a queue component (a queue can be as simple as a database table).

On top of that check for any use cases requiring additional and / or special components, like

* Components for bounded contexts, as identified during the service design phase and documented in the context map
  * Note: depending on the size and scope of a bounded context, it might be mapped either as a container or as a component within a container
* Service-specific data or rules
* Key data stores and data they hold
* Bespoke integrations

### Identify internal GovStack Building Blocks

When documenting this, identify what "internal" building blocks can be introduced as part of the solution (Scheduler, Workflow, ...). A first check would be check if any proposals / recommendations have been made during the service design phase.

Another source to check for potential building blocks is the context map, if available. If the context map contains "generic contexts", this generally means that there should be a building block offering this functionality. \
\[TODO: Add image that show example context map. Reuse from Service Design Chapter if possible]

{% content-ref url="/broken/pages/lj87QjMctjqqlNj7C8D2" %}
[Broken link](/broken/pages/lj87QjMctjqqlNj7C8D2)
{% endcontent-ref %}



## Modular Design

There is a lot to be said about Architecture Principles, but the following things are some of the most important and common to almost any software architecture:

* **Modularity**: You should aim for a modular software architecture. There are many names for this design principle (Component-Based Architecture, SOA, Modulith, Subsysteme, Microservices), but the all share that they are striving to break down a system into modular components.
* **Separation of Concerns**: When breaking down a system, "Separation of Concerns", meaning that each part should have a well-defined & clear-cut responsibility, should always be the guideline.

This makes the system easier to implement, test & maintain. Even if you are never going to replace a single module, this approach has great benefits to the project.

**Development vs Deployment** Keep in mind that these principles do not necessarily restrict your deployment options. It is possible and common even to deploy multiple modules in a monolithic way (Deployment Monolith)
