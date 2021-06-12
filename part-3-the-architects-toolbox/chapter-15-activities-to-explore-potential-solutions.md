# Chapter 15 - [Explore] Activities to Explore Potential Solutions
In the explore mindset, we work to discover multiple design concepts and engineering approaches we think will solve specific  problems.

Exploration involves:
- considering solutions we already know
- knowledge codified in frameworks and experiences woven into our culture
- domain concepts
- elements, relations, and their responsibilities

The first two bullets above come from one of _The Four Principles of Design Thinking_ (Chapter 2), all design is redesign.

The activities in this chapter will help generate options for the architecture.
Use them to explore the structures that will become your architecture and figure out engineering approaches for making them real.

## Activity - Personify the Architecture
To _personify the architecture_ means to give it human qualities in order to explore interactions among elements.
Pretend elements in the architecture are people/animals and describe their emotions, motivations, goals, and reactions to stimuli.

> Anthropomorphism for a software system is imprecise and ambiguous.
> We are trading precision for effective communication so that the architecture is easier to explain.

### Benefits
- make the architecture more relatable
- qualify desirable and undesirable properties and situations by thinking of how elements will "react" or "feel"
- create memorable stories that help the team keep architectural concerns at the center of design conversations
- increase buy-in of design decisions by making the architecture almost feel like a teammate
- quickly try different emotions and reactions through simple story telling

### Guidelines and Hints
- it is ok to feel silly
- accompany stories with sketches to make the ideas discussed more concrete
- anthropomorphism is not a substitute for architectural views describing the system using more precise language

## Activity - Architecture Flipbook
In an _architecture flipbook_, record every step of the design journey so others can follow along afterward.
Every page of the flipbook includes a sketch and notes about incremental changes to a model.
Use this record to think through options or backtrack to an earlier discussion that might have led us astray.
Bonus: the resulting flipbook explains why the architecture looks the way it does.

Participants: alone or a small group of 2-3 people

### Benefits
- methodically think through a model
- externalize the branching and backtracking happening naturally during design
- teach others how to think about design and modeling
- remove some of the mystery as to where the ideas for a model came from

### Guidelines and Hints
- start with the obvious concepts
- watch out for implied concepts or completely new concepts not explicitly named in the problem domain
  - these hidden concepts are among the most interesting and important to get right
- make small changes with each step in the flipbook
- look for inconsistencies in the model relative to the scenario or user story to build the model

## Activity - Component Responsibility Collaborator Cards (CRC cards)
Use _Component Responsibility Collaborator Cards_, to propose architectural elements, describe their responsibilities, and show how they come together to form a view of the architecture.

This techniques also works well for modeling domain concepts.

Participants: solo or the dev team works in small groups of 3-5

### Benefits
- quickly iterate through design alternatives
- create group buy-in and shared understanding of the architecture
- create a connection between ASRs and design alternatives
- identify potential gaps in the architecture

### Guidelines and Hints
- use index cards or sticky notes to represent elements
- draw pictures too
- it is ok to informally mix structures (static, dynamic, and physical) if it helps with reasoning
- every card should have at least one responsibility by the end of the activity
  - if no responsibility, does the component belong in the architecture
  - are there cards with too many responsibilities

## Activity - Concept Map
A _concept map_ is a method for exploring domain concepts by visualizing how concepts in the domain are related to one another.
Concept maps uncover:
- specific ideas from the problem domain
- implicit ideas required to implement a solution

Great software architectures are grounded in the problem domain.
Every domain concept needs a home in the architecture.

The relationship among domain concepts can help us pick the right patterns, interaction models, and information architectures.

Participants:
- create a concept map with technical stakeholders
- work alone or as a small group of 2-3
- verify a concept map with knowledgeable stakeholders

### Benefits
- visualize domain concepts and their relationships
- try out different relationships among domain concepts
- uncover missing, hidden, or implied domain concepts required to implement a functional software system
- lay a foundation for partitioning architectural elements and for defining potential relations among elements
- provide a resource for evaluating an architecture's fitness; is it consistent with the domain model
- outline a domain rich vocabulary for the software system (ubiquitous language)

### Guidelines and Hints
- be specific when naming concepts and describing how they are related (see the _7 stages of naming_ in Chapter 8)
- label both ends of a concept relationship
- be prepared for concepts and relations to move as the map emerges

### Alternatives
Concept maps pair well with architecture flipbooks; just make it a domain flipbook instead.

Although similar, this is not context mapping from DDD, which focuses more broadly on identifying contextual model boundaries across a large system.

## Activity - Divide and Conquer
In cases where you need to cover a lot of ground, break your team into small, independent groups dedicated to exploring a single problem.
Divide the problem into smaller chunks and conquer them in parallel.
Independent groups can use any exploration method they want within their group, but we still want some oversight to ensure everyone's time is well spent.

Divide and conquer works best with a tight feedback loop in which the broader group attempts to converge thinking regularly.
The time between when the exploration space is divided and converges again can be as short as a few hours or as long as a week.

kickoff meeting -> exploration plan -> group exploration -> show-and-tell -> iterate again starting at the exploration plan

Participants:
- divide the whole team and technical stakeholders into groups of 2-4
- the architect leading the exercise may participate in a group, but it is beneficial for the lead architect to float among groups to resolve issues and offer coaching

### Benefits
- explore more of a solution space in a shorter period of time
- see a range of design ideas covering similar areas
- give designers the time needed to adequately explore solutions (not all explorations should be in a 90-minute time box)
- use a larger group effectively by exploring different areas in parallel

### Guidelines and Hints
- all groups must share during the show-and-tell.
If the team completely missed their exploration goals, use it as a coachable moment to pivot or realign the group
- to maximize exploration potential, encourage people to form cross-functional groups with people they do not work with every day.
Consider occasionally mixing groups
- keep the groups small to avoid gold plating the designs and bike-shedding discussions in which the groups focuses on trivial, tangential matters
- commitments made during exploration planning should come from the group.
Some groups will need help scoping their commitments appropriately to the available exploration time
- remind groups that the exploration phase is ending so they have enough time to prepare for the show-and-tell

## Activity - Event Storming
_Event Storming_ is a collaborative brainstorming technique used to identify domain events.
Event storming can be used as a precursor to more in-depth domain modeling exercises, to assess the team's current understanding of the domain, and to identify risks and open questions in an existing domain model.

Event storming helps teams better engage with subject matter exports who are knowledgeable about the domain.
Event storming accomplishes this in two ways:
1. the format requires active engagement from all participants.
Subject matter experts have no choice but to inject their knowledge
2. event storming encourages participants to be concrete and specific.
If you have subject matter experts, encourage them to describe their jobs and expertise in detail

Participants:
- subject matter experts knowledgeable in the problem domain must participate
- a few members of the dev team
- as few as 2-3 participants to as many as a dozen or more, depending on the workspace and facilitator's experience

### Benefits
- visualize learning opportunities and facilitate a structured conversation about the domain
- uncover assumptions about how people think the system works; identify misunderstandings and missing concepts
- create a shared understanding of the problem and potential solutions
- produce a highly visual, tactile representation of business concepts and how they relate
- enable diverse viewpoints
- allow participants to quickly try out multiple domain models to see where concepts works and where they break down
- focus on concrete examples, not abstract ideas

### Guidelines and Hints
- include a diverse group of participants and ensure you have the right mix of participants
  - it is better to cancel the workshop and try again with the right mix of people than attempt the workshop without knowledgeable business experts
- try to create an unlimited modeling space
- explore real, concrete business examples.
The more specific, the better.
This helps expose new events and edge cases
- post a visual legend of the sticky notes being used
- ask clarifying questions throughout the workshop
- encourage participants to post sticky notes first, then talk about ideas
- time-box the activity to encourage the group to move forward quickly

### Alternatives
Event storming can be modified to include different experts and emphasize different modeling outcomes.
Here are some ideas:
- focus on big picture ideas and include many stakeholders when starting a new system or project
- dig into specifics required to implement event sourcing or CQRS systems by focusing more narrowly on a specific topic area
- include user experience experts and overlay a user's journey onto the event map
- use as the basis for evaluation to identify areas of the system that may need to be expanded or refactored
- run a workshop with new teammates and stakeholders to teach them about the problem domain

## Activity - Group Posters
Small groups work together to create a poster conveying their design ideas for the architecture.
This activity is well suited for summarizing outcomes from other workshops.

Participants: groups of 2-5, stakeholders who work together regularly should be in different groups

### Benefits
- produce several alternative models for comparison
- build pockets of consensus and spread knowledge within a larger group of stakeholders
- create artifacts easily shareable with people outside the group
- quickly explore and summarize architecture design ideas

### Guidelines and Hints
- remind participants to include a legend and think about which views of the architecture they are sketching - module, component and connector, or allocation
- sketching more than structures is fine, consider domain models, sequence diagrams, state diagrams, or anything else useful
- encourage jotting down open questions or risks that arise during group discussions
- during the critiques, remind participants to focus on facts and avoid "I like..." kinds of remarks

## Activity - Round-Robin Design
Quickly explore a range of ideas, and then combine them to start building consensus.
In a _round-robin design_ workshop, participants quickly generate, share, and critique sketches of the architecture to help them see a range of possibilities.
By the end of the activity, participants will have seen at least two new ideas in addition to their own.

Use this activity as a sanity check exercise or to set the stage for a follow-on activity such as creating group posters.

Participants:
- usually technical stakeholders since sketching architectural models
- at least 3 people, no more than 12

### Benefits
- give everyone a voice and opportunity to share their design ideas
- foster creativity by constraining the design environment
- create opportunities for unintended combinations
- encourage group ownership of the design
- build consensus among possibly disparate ideas
- expose differences, and similarities, in thinking across the group

### Guidelines and Hints
- hold the paper trading as a surprise, do not disclose all steps at the beginning of the activity
- informal views are fine during the sketches
- encourage participants to use any notations needed to convey an idea

## Activity - Whiteboard Jam
Collaboratively draw a series of diagrams that best capture the whole group's ideas.
We all do this.
This activity adds a smidge of structure to help the activity become more consistent and encourage better outcomes.

Participants:
- any technical stakeholder
- 3-5 seems to be a sweet spot
- allow participants to come and go throughout the session

### Benefits
- help opinionated teams get their ideas out in the open
- quickly move through design alternatives by forgoing formality and immediately improving ideas based on feedback
- create a shared cultural experience upon which further design insights can be created
- include many participants
- facilitate the activity as a participant

### Guidelines and Hints
- use during impromptu discussions to resolve confusion and capture multiple ideas under discussion
- write down important discussion points as they arise
- occasionally pause to reflect on the sketches and ask questions (_Iterate through the Create-Share-Critique Cycle_ from Chapter 9)
- it is ok to sketch while others are talking