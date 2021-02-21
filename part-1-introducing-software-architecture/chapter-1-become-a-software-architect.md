# Chapter 1 - Becoming a Software Architect
Being a software architect is a way of thinking.

## What Software Architects Do
A software architect lives and operates at the intersection of everything involved in a software system.
Therefore, in addition to programming, an architect's responsibilities include:
- define the problem from an engineering perspective
- partition the system and assign responsibilities to those pieces
- keep an eye on the bigger picture
- design trade-offs among quality attributes
- manage technical debt
- grow the team's architecture skills

### Define the problem from an engineering perspective
Architecture design is a human-centered design discipline.
An architect works with all stakeholders to understand what is expected of the software.
Therefore, an architect:
- defines quality attributes for the system
- keeps an eye out for design constraints and features that might force the architecture down a specific path
- defines the problem with the architecture in mind

### Partition the system and assign responsibilities to those pieces
Doing so enables:
- developing a strategy for achieving quality attributes and other system requirements
- smaller things to reason about, easier to test, and easier to design

### Keep an eye on the bigger picture
Software lives in the context of a system; this system includes people, processes, business needs, and many other technical and nontechnical factors.

### Design trade-offs among quality attributes
Software design is a constant struggle to find the balance between the things you want and what is needed or must be accepted.
Architects identify the trade-offs and work with stakeholders to decide which compromises to make.

### Manage technical debt
> __Tech debt__ is the gap between your software system's current design and the design you need it to have so you can continue to deliver value.

The best teams use tech debt strategically to ship faster and regularly pay debt down.
Architects make tech debt visible and help stakeholders decide which actions to take to manage it.

### Grow the team's architecture skills
Architects teach design skills and architecture concepts just-in-time.
Architects include the team in the design process; architecture is a social activity.

## What is Software Architecture?
> A system's __software architecture__ is the set of significant design decisions about how the software is organized to promote desired quality attributes and other properties.

A design decision might be significant if it will be costly to change later.
Some examples are:
- represents a point of no return
- influences quality attributes, schedule, or cost
- affects many people
- forces other software systems to change

To promote a quality attribute, and/or other properties, means to encourage it to appear in the system.
Corollary: a good architecture downplays/eliminates undesirable quality attributes.

### Define the essential structures
A structure defines how a software system is arranged.
Structures are in the code you write (modules), the software you run (components & connectors), and even your collaboration with others (allocations).

To create a structure, take any _element_ and connect it to another element using a _relation_.

The following table shows the three types of elements and relations.

| Type | Example Elements | Example Relations |
| --- | :--: | :---: |
| module | class, package, layer, stored procedure, config file, database table | uses, allowed to use, depends on |
| component and connector | object, connection, thread, process, tier, filter | call, subscribe, pipe, publish, return |
| allocation | server, sensor, laptop, load balancer, team, Owen (a person), docker container | runs in or on, responsibile for, develops, stores, pays for |
| | |

_Module_ structures exist at design time.
These are interacted with when writing code.
These stick around even when the software is not running.

_Component and connector_ structures exist at runtime.
Components can create connections to other components, spawn new processes, and instantiate new objects.
These cease to exist when the system is not running.

_Allocation_ structures are created by showing how module and C&C elements correspond with each other and the physical elements that exist in real life.
These are sometimes call _mapping structures_ since they show how different elements map to one another.

Different kinds of structures are useful for thinking about different properties desired in the system.
Structure determines the shape of the system, which decides the quality attributes and other properties.

### Reason about quality attributes (and other system properties)
> A __quality attribute__ is any externally visible characteristic by which stakeholders judge a software system's goodness.

A stakeholder experiences quality attributes when interacting with the software.
Choose an architecture that promotes the quality attributes desired.

## Build Amazing Software
Ways software architecture helps create software loved by stakedholders:
1. __Software architecture turns a big problem into smaller, more manageable problems.__
Consider these responsibilities of an architect, "partition the system and assign responsibilities to those pieces" and "keep an eye on the bigger picture."
2. __Software architecture shows people how to work together.__
When you know the architecture, then you can see how people can collaborate.
3. __Software architecture provides a vocabulary for talking about complex ideas.__
4. __Software architecture looks beyond features and functionality__; it also considers quality attributes and other properties.
5. __Software architecture leads to the significant decisions that must be made__, thus helping to avoid costly mistakes.
6. __Software architecture enables agility.__
If software is water, architecture is the container holding it.
A software system's architecture provides the structure within which change is possible.