# B.3 - Create Component Diagram

The container diagram is a even further "zoomed-in" version of the [#container-diagram](b.2-create-container-diagram.md#container-diagram "mention") and shows the software architecture within a single container. You dont have to create this diagram for every container, usually it is done for containers that need to be custom-coded. This most prominently includes the frontend and backend containers as well as special components, like a batch component or an complicated adapter. A bounded context might also be implemented as its own component, if it isn't big enough to justify its own container.

Example Component Diagram:

<figure><img src="../../.gitbook/assets/image (80).png" alt=""><figcaption><p>Adapted from https://c4model.com (CC BY 4.0). Changes made.</p></figcaption></figure>

Example Template:

<figure><img src="../../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure>

## Design Principles

* Modularity
  * Expanding on the ideas presented in [#modular-design](b.2-create-container-diagram.md#modular-design "mention"), a modular approach is also recommended within a container
  * Try to identify components and especially business components / domain components that encapsulate a specific area of concern
    * the data model is usually a good starting point informing you of areas of high cohesion
*   Some commonly used design patterns for dealing with external systems include Adapter, Proxy & Facade (see [Software design pattern - Wikipedia](https://en.wikipedia.org/wiki/Software_design_pattern)).\
    <br>

    <figure><img src="../../.gitbook/assets/image (82).png" alt="" width="375"><figcaption><p>Adapted from a CC0 1.0 public-domain diagram (Wikimedia Commons). Changes were made.</p></figcaption></figure>

