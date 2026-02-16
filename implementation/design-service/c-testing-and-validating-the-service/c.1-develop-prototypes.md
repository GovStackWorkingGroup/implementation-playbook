# C.1 Develop Prototypes\*

## Build prototypes

Once the [wireframe and/or voice command flow](https://govstack.gitbook.io/implementation-playbook/govstack-implementation-playbook/design-and-delivery/wireframes) is approved, we are ready to start developing functional prototypes for the service.

The prototype is iteratively developed. Each successive iteration adds new functionalities and refines the prototype based on user feedback. This results in a service that meets the desired level of functionality and usability.

### Levels of prototyping <a href="#levels-of-prototyping" id="levels-of-prototyping"></a>

Teams typically move through different levels of fidelity as confidence increases. Not all services or teams need to use every level.

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

A simple rule of thumb:

* Testing ideas or logic → low fidelity
* Testing flow or understanding → mid fidelity
* Testing interaction or readiness → high fidelity

Good prototyping practice:

* Be explicit about what each prototype is testing
* Expect prototypes to change or be discarded
* Avoid polishing designs before learning from users
* Treat prototypes as learning tools, not commitments to build

<details>

<summary><strong>How to do it</strong></summary>

#### 1. Choose what to prototype <a href="#id-1.-choose-what-to-prototype" id="id-1.-choose-what-to-prototype"></a>

Agree what part of the service they are prototyping and why. This is informed by:

* the service blueprint
* agreed hypotheses or assumptions to test
* relevant service patterns used in the journey

You do not need to prototype the whole service at once. It could be:

* a critical user task or decision point
* a risky or unclear part of the journey
* a flow that depends on multiple patterns or roles

#### 2. Get early feedback with a low-fidelity prototype <a href="#id-2.-get-early-feedback-with-a-low-fidelity-prototype" id="id-2.-get-early-feedback-with-a-low-fidelity-prototype"></a>

Support internal alignment and early validation of ideas, logic, and assumptions.

<figure><img src="../../../.gitbook/assets/Prototype - Low-fi.png" alt=""><figcaption></figcaption></figure>

**This looks like**

* Hand-drawn sketches or paper screens
* Whiteboard flows or storyboards
* Simple diagrams or annotated journeys
* Wireframe flows

**What to learn**

* Are we solving the right problem?
* Does the overall flow make sense?
* Are key steps missing or unnecessary?

#### 3. Test the content with a mid-fidelity prototype <a href="#id-3.-test-the-content-with-a-mid-fidelity-prototype" id="id-3.-test-the-content-with-a-mid-fidelity-prototype"></a>

Test structure, content, and end-to-end flow in more detail.

<figure><img src="../../../.gitbook/assets/Prototype (1).png" alt=""><figcaption></figcaption></figure>

**What it looks like**

* Clickable wireframes
* Draft screen flows using design tools
* Content presented in realistic layouts

**What to learn**

* Do users understand what to do at each step?
* Is the content clear and usable?
* Does the journey work end-to-end?

**When to use**

* Once a general direction is agreed
* When testing flow, comprehension, or sequencing
* For both internal testing and early user testing

#### 4. Define functionality with high-fidelity prototyping <a href="#id-4.-define-functionality-with-high-fidelity-prototyping" id="id-4.-define-functionality-with-high-fidelity-prototyping"></a>

Reduce delivery risk by validating detailed interactions and readiness.

**What it looks like**

* Near-realistic user interfaces
* Prototypes using representative content and data
* Validation and unhappy paths defined
* Limited technical proofs of concept, where needed

**What to learn**

* Are detailed interactions usable and accessible?
* Are there risks that could affect delivery?
* Is the service ready to move toward implementation?

**When to use**

* Close to delivery decisions
* For complex or high-impact services
* When accessibility or interaction detail matters

</details>

<details>

<summary><strong>Outputs</strong></summary>

* prototypes at an appropriate level of fidelity
* iterations demonstrating how ideas evolved

</details>

<details>

<summary><strong>Tools and templates</strong></summary>

You can run these activity using:

* a wireframing kit (for example, a shared Figma kit)
* sandbox or prototyping platforms
* simple wireframes or clickable flows
* content experiments or sketches

GovStack recommends capturing:

* the prototype flow being tested
* assumptions or questions being explored

</details>

## Reuse existing styles and patterns

Create visual and interaction consistency, building trust with users by reusing existing styles and patterns wherever possible.

Focuses on:

* identifying and reusing established UI styles and components
* reducing unnecessary design variation
* improving usability, accessibility, and delivery efficienc

<details>

<summary><strong>How to do it</strong></summary>

1. **Check for an existing style guide**\
   Identify whether a design system or style guide already exists for your organisation, programme, or platform.
2.  **Run a UI safari (if needed)**\
    If no consistent style guide exists, review existing services or products to identify common:

    * buttons and form elements
    * typography and spacing
    * colours and visual hierarchy

    Capture examples that appear frequently or work well.
3. **Agree a baseline set of styles**\
   Consolidate commonly used components and styles into a simple reference that teams can reuse.
4. **Apply styles consistently**\
   Use the agreed styles and patterns when creating wireframes, prototypes, and early designs.
5. **Document new styles**\
   Document new styles in a way thats easy for others to use, for example, using Github, Figma or StoryBook.<br>

</details>

## Consider the design of content <a href="#heading-title-text" id="heading-title-text"></a>

Design content that is clear, consistent, and easy to understand for users.

Use simple language so users can understand what is happening, what is expected of them, and what will happen next without needing specialist knowledge.

<details>

<summary><strong>How to do it</strong></summary>

1. **Identify key content moments**\
   Review where users need to read, decide, or act, such as:
   * page headings and instructions
   * form questions and help text
   * error messages and confirmations
2.  **Simplify the language**\
    \
    \[Image showing simpler content next to original legalise]\
    \
    Rewrite content so it:

    * uses familiar, everyday words
    * avoids jargon, acronyms, and legal or technical language
    * uses short sentences and clear structure

    Prefer clear explanations over formal or bureaucratic wording.
3. **Focus on the user’s task**\
   Check that content:
   * explains what the user needs to do
   * explains why information is needed (where helpful)
   * sets clear expectations about outcomes or next steps
4. **Check consistency**\
   Make sure similar actions, concepts, and messages are described using the same words across the service.
5. **Review from a user perspective**\
   \
   \[Image of highlighter testing]\
   \
   Ask: _Would someone unfamiliar with this service understand this first time?_\
   Where possible, test or review content against known user needs.\
   You can use methods like '[highlighter testing](https://userresearch.blog.gov.uk/2014/09/02/a-simple-technique-for-evaluating-content/)' to test the content with users.

</details>
