# Chapter 16 - [Make] Activities to Make the Design Tangible
In the make mindset, we turn abstract ideas into tangible things easily shareable.

Tangible things:
- facilitate communication
- can be directly tested to see how well a design addresses needs
- enables reasoning about the architecture

Even making only a part of an artifact can serve as a useful thinking exercise.

Remember to review what you make with your team and relevant stakeholders.
Chapter 17 will show how to facilitate reviews.

## Activity - Architecture Decision Records
Capture architecture design decisions as they are made using a lightweight, text-based template.
Documenting design decisions makes it easier to share and analyze them.
Retaining a history of decisions provides context for the current architecture relative to its evolution.

### Benefits
- make recording design decisions a team responsibility
- keep key decisions close to the code by storing them in the code repo
- combine with other artifacts to create a holistic description strategy
- capture history to gain perspective on the evolution of the design
- involve the whole team in the design process
- train teammates in architectural thinking by providing ADR templates
- enable peer review of design decisions using standard development tools and an existing peer review workflow

### Guidelines and Hints
- include only one decision per file
- sequentially number ADRs and keep old records.
Add references to old records when a decision is superseded or changed
- keeps ADRs short, one or 2 pages at most
- use plain language when recording decisions
- put architecture decisions through the same review process as code
- store in version control with other code artifacts
- ADRs should not be the only architecture documentation you create.
Combine with other artifacts such as views, architecture haikus, and system metaphors

## Activity - Architecture Haiku
Figure out what matters in your architecture by creating a bite-sized summary stakeholders will use.
An architecture haiku describes a view of the architecture using only a single piece of paper.

### Benefits
- think through and articulate the essential parts of the architecture
- produce an artifact easily consumed by readers.
The end result is like a flier advertising the best parts of the architecture
- create a frame of reference for other documentation

### Guidelines and Hints
- do not record everything about the architecture; focus only on what is most important
- establish a common vocabulary for architectural concepts
- set aside time to explore design options before starting
- treat the architecture haiku as a living document
- use the architecture haiku as an outline or executive summary for a longer architecture description
- not a replacement for other design artifacts

## Activity - Context Diagram
A _context diagram_ helps stakeholders understand where the software system fits in the world.
Context diagrams show the people and systems that interact with the software system you are responsible for developing.

### Benefits
- provide a high-level overview of the systems and stakeholder groups the system directly interacts with or relies on
- make the boundary between the system you are building and the outside world obvious to stakeholders
- use as a natural entry point for learning about the system's architecture
- ensure everyone is aware of and agrees with the general system scope

### Guidelines and Hints
- it is ok to use informal notations.
The most important thing is to communicate effectively
- show people and systems relevant to the system you are designing
- label arrows to tell how two things are related
- include a legend to describe the notations in the diagram

## Activity - Greatest Hits Reading List
As a software system grows, so does the documentation describing its architecture.
A _greatest hits reading list_ will help stakeholders navigate the morass of design artifacts so they can find the relevant information.
Creating a curated reading list provides new stakeholders with a starting point for learning about the architecture.

### Benefits
- highlight the most important design artifacts
- provide context for design artifacts within the scope of the whole system
- unify disparate, lightweight design artifacts to create a coherent, whole description

### Guidelines and Hints
- organize the list around stakeholder concerns
- the same artifact can be used to address different concerns.
Use the overview and caveats to help stakeholders navigate an artifact from varying perspectives
- take advantage of design artifacts from third-party sources by referencing them instead of creating your own
- include links to reference material defining important concepts in the architecture as well as design artifacts

## Activity - Inception Deck
Answer ten important questions at the start of a new project to avoid common failures and align stakeholders.
The inception deck is usually created early in a project's life, during the _inception_ phase.

Filling in the inception deck is short when you have the required information handy.
Finding the information needed for the deck could take days/weeks.

### Benefits
- put important info in the open
- share easily with all stakeholders
- ensure all stakeholders have a common understanding of important system concerns
- discuss important information that should be covered at the start of a new project

### Guidelines and Hints
- use the ten questions as a checklist for kicking off a software project
- periodically review the inception deck as a reminder for what is important in the project
- the effort creating the inception deck should be commiserate with size and cost of the project.
For example, do not spend a week creating an inception deck for a two-week project

## Activity - Modular Decomposition Diagram
Show how the architecture is composed of varying abstractions that come together to create a coherent whole.
A _modular decomposition diagram_ is a simple tree diagram showing how varying granularities of abstraction are related to one another.

### Benefits
- uniquely name concepts at different granularities of abstraction
- map refinements in the architecture
- use to analyze organizational alignment with the system's composition
- reduce complexity without losing traceability to related elements
- promote system thinking within the architecture

### Guidelines and Hints
- use the diagram to help reason about quality attributes such as agility, maintainability, time-to-market, costs, buildability, and deployability
- break large diagrams into smaller ones to make them easier to understand.
Be careful not to lose the context between the diagrams
- leaf nodes should not be connected with other leaf nodes except by way of their parent

## Activity - Paths Not Taken
Create a list of the architectural decisions you discarded with a brief note explaining why you rejected each decision.
Recording the decisions you discarded, the paths not taken, provides context and rationale for a design decision.

### Benefits
- help downstream designers replay the thought process that went into the current design
- head of _did you consider...?_ discussions with stakeholders
- provide an additional layer of rationale for design decisions

### Guidelines and Hints
- focus on a single view or design decision.
Do not attempt to encompass all design decisions
- keep it brief; include only enough detail so stakeholders can understand the decision and why it was rejected
- combine with other methods, such as ADRs and architecture haikus, to create a more complete description of the architecture

## Activity - Prototype to Learn or Decide
Develop or use software so you can test a hypothesis, learn information needed to make a design decision, prove a quality attribute, or gain experience.

We _prototype to learn_ when we need to figure out how to do something or how something works.
We _prototype to decide_ when we need to gather information to help in choosing between multiple options.

Building a prototype to decide is like running an experiment.
The technology or pattern under investigation is hypothesized to solve a specific design prolbem.
The purpose of the prototype is to test the hypothesis.

### Benefits
- gather information through firsthand experience
- generate data to use in decision making
- allow stakeholders to experience a part of the system
- learn how something works quickly and inexpensively

### Guidelines and Hints
- look for ways to meet learning objectives without writing software
- decide up front whether the prototype is evolutionary or throw-away
- prototyping often requires trading quality for speed of delivery and completeness.
This is a challenge for many devs proud of their craft
- time-box the prototype aggressively, but allow sufficient time to complete the work
- sketch out a high-level design for the prototype with the implementers before starting development

## Activity - Sequence Diagram
Use a _sequence diagram_ to show how control or data moves through the system at runtime.
Model the flow of logic, data, or control among components.

### Benefits
- simple and flexible notation
- both graphical and text notations exist
- useful for communication and reasoning
- ample tool support, though tools are not required

### Guidelines and Hints
- reason about distributed systems, microservices, object communication, and other dynamic structures
- informal notations are fine if consistent
- use a tool that renders text-based notations so you can store the diagrams with your code
- choose a single scenario to diagram

## Activity - System Metaphor
Tell a simple story demonstrating how the system influences specific quality attributes.

### Benefits
- lightweight description technique perfect for co-located teams to use during times of fast architectural evolution
- can be combined with other description methods
- cheap to create, easy to change

### Guidelines and Hints
- tell a memorable story and have fun
- be specific and focus on what makes your system unique.
We already know that every software system ever made is _like a city_
- if a common reference point does not exist, then create a shared experience
- pop culture and food are common points of reference for many metaphors
- common architecture patterns serve the same purpose as system metaphors and can be used in the same way