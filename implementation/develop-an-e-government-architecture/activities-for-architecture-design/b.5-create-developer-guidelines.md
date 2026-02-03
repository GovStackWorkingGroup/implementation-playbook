# B.5 - Create Developer Guidelines

Developer Guidelines should be a document that describes the rules how one specific project should be developed. Those rules will be unique for every project, but below you will find a few recommendations that should be included.

Above all, this should be a living document - continuously updated by the developers throughout the implementation phase, based on the insights and experience gained during development. Adherence to the guidelines will be a lot better, if they include the feedback and consensus of the development team.

For a starting point, the developer guidelines should include:

* Any rules derived from governance and compliance
* adherence to [#modular-design](b.2-create-container-diagram.md#modular-design "mention")and [#design-principles](b.3-create-component-diagram.md#design-principles "mention")
* Recommended patterns, like
  * [best-practices-and-patterns.md](../best-practices-and-patterns.md "mention")
  * [cfr-architecture](https://govstack.gitbook.io/cfr-architecture/5-cross-cutting-requirements)
* Validation rules
  * What kind of validation should be performed on the inputs.
  * For example, a backend should **never trust the frontend** to provide valid inputs. Instead **validation must be performed (again) on the backend.** Otherwise there might be a threat vector for malicious actors.
* Error handling
  * how errors should be handled consistently across the application
  * what information is returned via the api
  * what information is to be logged
  * usage of error codes
* Logging Guidelines, provide guidelines on
  * what information to log
    * It is useful to have a unique identifier (uuid / guid) that groups log messages belonging together. An example would be a correlation id identifying an unique REST request.
    * In addition, it has proven valuable to define a "logging context". The logging context contains information that will always be logged with every message.
  * what log level to use when doing so
  * describe a consistent way of logging error scenarios
* Design Guidelines for Components, like
  * Separation of Business Code
    * Code that implements business rules should be separated from code that implements technical details (REST communication, Persistence Access)
    * This way the code stays more flexible and is easier to debug & maintain
  * Usage of Layers
    * Layered approaches are helpful to separate the business code from technical code
    * Example:

<figure><img src="../../../.gitbook/assets/temp (3).png" alt=""><figcaption></figcaption></figure>
