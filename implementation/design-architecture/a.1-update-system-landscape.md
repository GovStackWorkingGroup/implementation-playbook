# A.1 - Update System Landscape

## Purpose

The System Landscape Diagram

* describes
  * the IT architecture of your organization (or a department of that)
  * the services provided by the organization
  * the systems required to provide those services
* gives an overview of what systems exist in an organization and how they interact with each other
* informs about
  * dependencies & bottlenecks
  * reuse within the organization
    * usage / adoption of building blocks (for example a central Identity component)
  * redundancies & duplication

## Scope

A single diagram can usually only hold the information on a subset of systems. In the context of this playbook, the System Landscape should describe

* a single organization
* all software systems of that organization that
  * are necessary to provide the e-government services of that organization
  * follow the same or similar governance (for example all systems using GovStack)
* all interfaces between those systems
* all outside interfaces of those systems
* should be grouped into clusters representing the services provided by the organization (one cluster - one service / Fachverfahren)

## How to do it

* If the System Landscape Diagram already exists, just update it, by adding the information from the System Context diagram.
* If it does not exist, it can easily be created from System Context
  * It might be useful to add additional boxes to create groups of systems, where suitable
* Optionally: if you want to further complete the System Landscape, go back to the previous step and create System Context for further systems. This way you will document the Government Architecture step-by-step.

Example System Landscape Diagram:&#x20;

<figure><img src="../../.gitbook/assets/image (25).png" alt=""><figcaption><p>Adapted from https://c4model.com (CC BY 4.0). Changes made.</p></figcaption></figure>

