# B.4 - Decide Technology Stack

Each project will have its own unique technology stack, so you cannot provide any hard rules. But this chapter aims at providing a few guidelines on how to select the right stack for your project.

## **Considerations & Criteria**

There are several things to consider, when deciding a technology stack and not all of them are of a technical:

1. Governance
   * check if there are any Governance Rules on permitted technology. Maybe there even is a recommended toolstack. If yes, strongly consider using it. To limit the number of technologies in an organization is a very important goal, beyond the scope of a single service or project.
2. Staffability
   * what skills are available in the team
   * what skills are easy to staff, if the team changes
3. Resources
   * how many resources (books, videos, trainings, articles, ...) are available on the technology
4. Ecosystem
   * how strong is the ecosystem for the technology
     * Frameworks & Libraries
     * Tooling (IDE's & extensions, Code Analysis, Build Tools)

* Actively Developed & Supported

To consider those, you could analyse

* capabilities in your national industry
* technology usage reports,
  * **focus on "most used" technology** while _ignoring "most popular" technology_ trends
* statistics on github

Example Sources:

* [Most used languages among software developers globally 2025| Statista](https://www.statista.com/statistics/793628/worldwide-developer-survey-most-used-languages/) _- Statista_
* [The Top Programming Languages 2025 - IEEE Spectrum](https://spectrum.ieee.org/top-programming-languages-2025) _- IEEE_
* [Most used web frameworks among developers 2025| Statista](https://www.statista.com/statistics/1124699/worldwide-developer-survey-most-used-frameworks-web/) _- Statista_
* [Most Popular Backend Frameworks 2012/2025 -](https://statisticsanddata.org/data/most-popular-backend-frameworks-2012-2025/)

## **Recommendations**

Here are some recommendations on selecting technologies:

* Use open source technologies
* Established technologies like Java, Spring, Angular, React are established for a reason
  * their strength lies in their rich ecosystems
  * Prefer programming languages with static typing, like Java & Typescript. Static typing allows you to prevent errors before they hit production and allow for really strong tools around quality & security analysis
* Use frameworks & libraries, especially for
  * Encryption
  * Security / IAM
  * Logging
  * HTTP / REST
  * An ORM mapper (like Hibernate) is almost always a good choice
* But limit use of dependencies, especially on the frontend side, to avoid "dependency hell"

## **Proof of Concept**

There will be areas where it is uncertain if it is possible to solve a problem with a chosen technology or approach. In that case it is recommended to do a PoC.

To perform the PoC, first create a narrow and specific problem statement

<details>

<summary>Example </summary>

_Is the selected tool able to process 1.000.000 requests in under one hour if the calling system parallelizes the requests._

</details>

Then it is possible to do small series of sprints, trying to solve that specific problem and come to an evaluation. Of course it might be sensible to test and compare multiple approaches, if time permits.
