# Chapter 7 - [Explore] Create a Foundation with Patterns
This chapter presents common architecture patterns and discusses how to adapt them to meet specific needs.

## What is an Architecture Pattern?
> An __architecture pattern__ is a reusable solution to a specific problem, showing how to promote specific quality attributes by using a specific combination of structures.

Refer to the book for more information about each pattern such as elements, relations, rules for use, strengths, and weaknesses.

## Layers Pattern [Module]
The __layers pattern__ creates decoupled, cohesive layers.
Use layers any time code modules need to be changed independently of one another.

## Ports and Adapters Pattern [Module or Component and Connector]
The __ports and adapters pattern (hexagonal architecture)__ isolates core business logic so it can be used in a variety of contexts and isolated from components providing data and events.
Pluggable adapters can be injected into the core business logic to provide access to events and data.

Use this pattern when the system must support multiple input devices or when there is a risk that input devices could change.

## Pipe-and-Filter Pattern [Component and Connector]
With the __pipe-and-filter pattern__, each component called a filter is responsible for a single transformation or data operation.
Data is piped from one filter to the next as quickly as possible, and data operations occur in parallel.

A similar pattern is the __batch sequential pattern__.

## Service-Oriented Architecture Pattern [Component and Connector]
In a __service-oriented architecture (SOA)__, independent components are implemented as services.
Services are combined at runtime to define the software system's behavior.
Service consumers must be able to locate and use services without knowing the implementation details behind the used services.

Useful to design large software systems such that departments work independently within their area of expertise.

## Publish-Subscribe Pattern [Component and Connector]
In the __publish-subscribe pattern__, producers and consumers exist independently and unaware of one another.
producers and consumers communicate indirectly via an event bus.

Choose this pattern when multiple, independent components need access to the same information.

## Shared-Data Pattern [Component and Connector]
In the __shared-data pattern__, multiple components access data through a common data store.
Data and the data source are the primary medium of interactions.

Useful when multiple components require a large amount of data.

## Multi-Tier Pattern [Component and Connector or Allocation]
In the __multi-tier pattern__, runtime structures are organized into logical groups.
These logical groups may be allocated to specific physical components such as a server or cloud platform.

The multi-tier pattern is conceptually similar to the layers pattern but at a different level of structures.

Useful when components will live on different platforms or hardware.

## Center of Competence Pattern [Allocation]
In the __center of competence (CoC) pattern__, a team of experts defines patterns, establishes best practices, develops support tools, and provides education for a subset of the architecture.
CoC teams can be organized around technologies, use cases, patterns, and high-risk areas.

The CoC is a support team, its primary goal is to increase development speed and improve the overall quality of the software system.
A CoC makes it easier for development teams to implement patterns and technologies we want in the architecture.

## Open Source Contribution Pattern [Allocation]
In the __open source contribution pattern__, teams are given responsibility for developing specific architectural components but are not expected to be the only contributing developers.
The owners will review submitted changes to a component for quality and conceptual integrity.

This pattern allows for limited centralized control across the architecture.

Use when there are experts available from multiple development teams or when there is a common dependency on specific components.