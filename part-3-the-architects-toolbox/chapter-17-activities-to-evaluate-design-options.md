# Chapter 17 - [Evaluate] Activities to Evaluate Design Options
In the evaluate mindset, we critically examine design decisions to determine how well they meet our needs.
Our goal is to make sure the architecture _satisfices_, that it is satisfactory and sufficient, good enough.

After an evaluation we should have enough information to decide which design mindset to embrace next during the do-make-check cycle.
Note that the evaluate mindset is always embraced during the _check_ step, but can be used in the _do_ step too.

Evaluation is continuous.

The activities in this chapter help teams look deeply at different facets of the architecture and glean information needed to take action.
Use them when you need:
- to check understanding
- to choose a design option
- help figuring out what to do next

## Activity - Architecture Briefing
This presentation is used to bring stakeholders up to speed about some part of the architecture.
By the end of the briefing, participants are able to provide meaningful feedback about the architecture.

Participants:
- architect present the briefing
- stakeholders and knowledgeable non-stakeholders attend

### Benefits
- quickly bring stakeholders up to speed so they can ask questions and point out issues in a design
- foster a sense of shared ownership over the architecture
- enable more stakeholders to provide feedback, ensuring a diversity of perspectives critically evaluate the design
- promote accountability in architectural decision making
- create a platform for teaching and learning architecture design

### Guidelines and Hints
- host briefings at a regular interval
- publish artifacts, like slides, and hopefully a recording
- appoint a note taker during the questions portion of the briefing
- audience question should be tough, but constructive

## Activity - Code Review
A form of peer review in which code is incrementally inspected with an eye toward architectural concerns as the code is developed.

Incrementally inspecting code as the architecture manifests helps fight architectural rot by keeping tabs on the system's evolution relative to the planned design.
They are also a great time to identify design inflection points emerging during development.

Every review presents a potential coaching opportunity.
Watch out for synchronization mismatches in mental models so they can be fixed.
Coach teammates on architectural principles as well as the specific architecture you are developing together.

### Benefits
- keep architecture design at the forefront of every developer's mind
- allow finer-grained details to emerge without losing a connection with coarser-grained architectural concerns
- manage emergent details that can cause problems in the architecture
- influence the detailed design as required
- create teachable moments to grow the team's architecture design competence

### Guidelines and Hints
- reviews are often small.
Watch out for thematic shifts in how the code evolves over time
- escalate the style of peer review to resolve issues quickly, such as using pair programming or a whiteboard jam
- it is OK for the architecture to change as the system emerges.
The primary goals of code review form the architect's perspective is to increase awareness of design decisions, monitor the implementation of the architecture, and guide change over time
- code review is not a replacement for design evaluations.
Use reviews to monitor architectural drift and learn how you can better serve your team as an architect

In the book is a fantastic code review checklist.

## Activity - Decision Matrix
A decision matrix is a visual comparison of how various alternatives stack up against one another.
Use a decision matrix to qualify design alternatives so sa decision can be made.
A decision matrix can also be used in documentation as a part of the design's rationale.

Participants:
- architect is responsible for ensuring the matrix is filled in accurately
- stakeholders validate the evaluation factors

### Benefits
- use to compare a variety of decisions such as patterns, technologies, or frameworks
- visualize relative strengths and weaknesses among decisions
- focus attention on essential factors when comparing and contrasting alternatives
- facilitate open discussion about trade-offs among alternatives

### Guidelines and Hints
- use qualitative comparisons unless you performed quantitative analysis
- consider no more than 7 factors in the same matrix
- compare up to 5 design options in the same matrix
- take good notes when filling in the matrix.
The analysis is as important as the results and can provide design rationale for decisions

## Activity - Observe Behavior
Add instrumentation to the software system to see runtime behaviors.
Use the observations to answer specific questions about quality attributes and other stakeholder concerns.

The ability to observe the system assumes that _observability_ is designed into the architecture.
Evolve the architecture as needed to promote required observability scenarios.

### Benefits
- monitor the system over time to verify design assumptions
- directly test how well quality attributes are promoted
- produce concrete metrics shareable with stakeholders

### Guidelines and Hints
- as you answer questions about the software system, think about how the data can be used in automated analysis.
Consider adding your metrics to system dashboards and alerting systems
- in theory, any runtime property of the system can be observed

## Activity - Question-Comment-Concern
This is a  collaborative, visual activity getting the whole team talking about the architecture - what they know, what they don't know, and what keeps them up at night.
Use this activity to shine a light on knowledge gaps, articulate issues, and establish known facts about the architecture.

The inclusion of comments is meant to fast-track issue resolution.
Issues resulting from simple gaps in understanding can be resolved immediately so the team can focus on the bigger concerns.

Participants: whole team

### Benefits
- promote knowledge sharing by flushing questions into the open along with potential answers
- visualize high-risk, mysterious, or troublesome parts of the system
- identify areas in need of further research and exploration
- foster shared ownership over the architecture and the direction it takes

### Guidelines and Hints
- comments can be facts, new ideas, tidbits of knowledge, or answers to questions raised during the workshop
- concerns can be known problems, risks, or general worries
- questions can expose gaps in understanding, mismatches in expectations, or areas in need of further exploration

## Activity - Risk Storming
A collaborative, visual technique for identifying risks in the architecture.

Participants:
- small groups of 3-7 devs
- participants must be familiar with the architecture

### Benefits
- quickly identify risks in the proposed system architecture
- visualize the system by considering the level of risk
- constrain risk identification to architectural concerns
- provide a platform for all team members to elevate their concerns

### Guidelines and Hints
- place sticky notes directly on the diagrams
- leave time for team discussions; this is the most important part
- use no more than 2-3 diagrams, more than that can be overwhelming

## Activity - Sanity Check
A fast, simple exercise designed to expose issues in team communication or understanding.
Sanity checks verify everyone is indeed on the same page.
They can also identify opportunities for improving team operations, artifacts, and design methods.

When designing a sanity check, keep it as a short-burst activity forcing teammates to actively think about the architecture.
Verbal sanity checks are an efficient way to end most collaborative design sessions.

### Benefits
- reinforce architectural responsibility across the team
- identify problems caused by misunderstandings and gaps in knowledge early
- create teaching and coaching opportunities
- document knowledge the team feels is essential to the design
- pinpoint opportunities for improving artifacts and communication
- uncover the unknown unknowns

### Guidelines and Hints
- simple and short; a good sanity check can be completed in 5-10 minutes or less
- remember: sanity checks are about improving the team's knowledge.
Do not use in a punitive or rewarding way.
- share responsibility for creating sanity checks among the team
- host regular sanity checks
- be creative and use a variety of formats; this keeps it fresh and helps expose different kinds of understanding gaps

## Activity - Scenario Walkthrough
Describe step-by-step how the architecture addresses a specific quality attribute scenario.
Scenario walkthroughs can be used any time but are most applicable early in the life of the software system, before the system's behavior can be observed directly.

### Benefits
- assess the architecture design early, even while it is only on paper
- identify different concerns in the architecture
- reason about how the architecture will respond to different stimuli
- qualify the design; walkthroughs are not strict pass or fail
- quickly determine the extent to which the architecture promotes or inhibits different quality attributes

#### Guidelines and Hints
- avoid creating a witch hunt.
The point is to find potential problems while they are still cheap to fix.
Finding issues is a good thing.
- time box the time spent on each scenario
- surface issues, but avoid problem solving
- record new quality attribute scenarios raised during the walkthrough

## Activity - Sketch and Compare
Create two or more alternatives of the same design so it is easier to see the pros and cons.

Any design alternatives can be sketched and compared.
This includes current and future, ideal and reality, technology A and technology B, and many others.

Sketching the extremes can also be compared.
To do this:
- pick a quality attribute or design concept
- design the architecture for that one thing at the exclusion of all else
- then pick another high-priority quality attribute or design concept
- sketch an alternative design for comparison

### Benefits
- expose both the positive and negative aspects of a decision by comparing it to something else
- create a platform for discussion and build consensus around a design decision
- avoid _buyer's remorse_ when making a design decision by doing at least a basic comparison

### Guidelines and Hints
- avoid argumentative confrontations and encourage constructive participation.
Sometimes participants will pick sides and entrench themselves, strongly favoring one design over the other
- be ready to sketch compromises as the discussion progresses.
Some of these new ideas will become new design alternatives
- always summarize the findings so there is no confusion about the decisions made
- follow up with skeptics to win them over and drive consensus