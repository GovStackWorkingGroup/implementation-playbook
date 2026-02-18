# 5 Start with the System Context

It is always advisable to start with the system context, as it provides a good first overview of how technical requirements emerge from the functional requirements. The system context defines the boundaries of the solution, the actors who interact with it, and the external systems and building blocks on which it depends.

Having the system context early already informs you about many of the components that will appear later in step [5-b.3-create-component-diagram.md](5-b.3-create-component-diagram.md "mention").

## System Context Diagram

<figure><img src="../../.gitbook/assets/image (23).png" alt=""><figcaption><p>Adapted from https://c4model.com (CC BY 4.0). Changes made.</p></figcaption></figure>

## How to do it

### Identify users & actors

Understanding who interacts with the system and how is the foundation of the system context. Identify all user types, their responsibilities, and their interaction channels.

* Identify all types of users, like
  * end users, power users,
  * back‑office staff, support users
  * administrators and supervisors
  * external partners or agents
    * technical users, system users
* Understand roles & privileges
  * required roles, permissions, and access levels
  * separation of duties (e.g., requester vs approver)
  * needs for authentication, authorization, or delegated access
* Identify interaction channels
  * Check whether different user groups require different channels or frontends. For example:
    * A citizen uses a mobile or web interface
    * A case worker uses an internal operational interface
    * An administrator uses a monitoring or configuration interface
  * Users do not always interact through a typical UI. Consider:
    * API calls from partner systems
    * File uploads (documents, spreadsheets, scanned forms)
    * Batch jobs or scheduled tasks
    * Emails or text & chat messages triggering processes

### Identify external systems

Identify all external systems your service needs to interact with and understand the flow of information between all systems and actors. This includes the data formats and communication technologies being used (like REST + JSON). The system being designed might only be a single step in a series of steps.

### Identify external GovStack Building Blocks

When documenting this, identify what "external" building blocks can be introduced as part of the solution (IAM, Messaging, Payment, Information Mediator, ...). A first check would be check if any proposals / recommendations have deen made during the service design phase. You should aim to reuse & share existing instances of those building blocks when possible.

Another source to check for potential building blocks is the context map, if available. If the context map contains "generic contexts", this generally means that there should be a building block offering this functionality. \
\[TODO: Add image that show example context map. Reuse from Service Design Chapter if possible]



{% content-ref url="/broken/pages/lj87QjMctjqqlNj7C8D2" %}
[Broken link](/broken/pages/lj87QjMctjqqlNj7C8D2)
{% endcontent-ref %}

## Next Step: System Landscape or System Architecture

After completing this step, you need to decide whether you want to continue with the System Landscape, for an overview or with the System Architecture, for getting into the details of the technical design.

{% columns %}
{% column %}
{% content-ref url="5-a-system-landscape.md" %}
[5-a-system-landscape.md](5-a-system-landscape.md)
{% endcontent-ref %}


{% endcolumn %}

{% column %}
{% content-ref url="5-b-system-architecture.md" %}
[5-b-system-architecture.md](5-b-system-architecture.md)
{% endcontent-ref %}


{% endcolumn %}
{% endcolumns %}
