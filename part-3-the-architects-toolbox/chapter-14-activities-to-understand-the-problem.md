# Chapter 14 - [Understand] Activities to Understand the Problem
In the understand mindset we actively seek information from stakeholders and work to define (or redefine) the problem.
This involves:
- figuring out who our stakeholders are
- identifying business goals for the system
- specifying requirements with an eye toward the architecture

Recall from Chapter 5, _Dig for Architecturally Significant Requirements_, that there are four kinds of ASRs, with quality attributes having the most influence.
- __constraints__ unchangeable design decisions, usually given but sometimes chosen
- __quality attributes__ externally visible properties characterizing how the system operates in a specific context
- __influential functional requirements__ features and functions requiring special attention in the architecture
- __other influencers__ time, knowledge, experience, skills, office politics, geeky biases, and everything else swaying decision making

## Activity - Choose One Thing
Discuss priorities with stakeholders by asking "if you only get one thing, what will it be?"
This activity can help stakeholders make decisions when facing difficult trade-offs.

Participants: all stakeholders

### Benefits
- Clearly communicates, _this is more important than that_.
- Starts a conversation about why a certain choice was made and what would need to change for stakeholders to change their mind.
- Makes it obvious when stakeholders disagree.

### Guidelines and Hints
- Do this before things get too difficult.
This conversation is easier when it is hypothetical than when it is real
- Quality attributes in tension with one another should be pitted against one another
- Use this to prioritize influential functional requirements
- This technique works well as an informal conversation to help get better understanding of stakeholders' true need

## Activity - Empathy Map
Brainstorm and record a particular stakeholder's responsibilities, thoughts, and feelings to help the team develop a greater sense of empathy with stakeholders' goals.

Participants: software architect, dev team; small groups of 3-5 or as a solo exercise

### Benefits
- Discover your audience's needs before developing an architecture description
- Help decide what information to include or exclude
- Create a rubric for evaluating the effectiveness of an architecture description

### Guidelines and Hints
- Be specific.
Pick a person to empathize with, not a general role
- Validate the findings from your empathy map with stakeholders
- Mention quality attributes, risks, or other concerns this person may find relevant
- Adapt this method for understanding application end users, external systems (for interface design), or for use with proxy stakeholders to understand quality attributes

## Activity - Goal-Question-Metric (GQM) Workshop
An approach for identifying metrics and response measures so we can connect data with business goals.
The goal of GQM is to identify measures usable to determine whether a goal is satisfied.

- goal: defines a conceptual requirement that must be met.
Goals can describe quality attribute scenarios, general software quality, business goals, or other topics.
- questions: illustrate the means by which we can characterize one or more goals
- metrics: defines the measures needed to answer one or more questions

Participants: Solo or in a small group of 2-5 people; any mix of stakeholders

### Benefits
- emphasizes using stakeholder goals as the basis for measures
- shows clear lineage from data to stakeholder goals by way of the questions that must be answered to decide whether a goal is satisfied
- flexible approach that can help teams think about metrics in a variety of situations

### Guidelines and Hints
- Ensure there is plenty of space for drawing the GQM tree
- Look for opportunities for reuse.
Metrics can be used to answer more than one question.
Likewise, the same data might help compute multiple metrics
- Data sources and data are likely to influence the architecture, but also look for opportunities to gather data outside of the architecture
- Record results to validate with stakeholders later.
The identified metrics are revisited throughout the life of the software system

## Activity - Interview Stakeholders
Learn about stakeholders' business goals by asking.
When we _interview stakeholders_ we:
- ask about their plans for the software
- uncover the problem context
- get a feeling for looming risks
- and dig for details about quality attributes and other requirements

Participants
- one-on-one or in small stakeholder groups
- led by the architect
- others may observe the interview, but no more than one or two active interviewers

### Benefits
- focus on general info gathering
- format allows for open back-and-forth discussion
- provides background info usable to prepare for other workshops or activities
- quickly validate quality attribute scenarios and other ASRs
- creates a direct connection between stakeholders and architects

### Guidelines and Hints
- Avoid interviewing stakeholders about architectural concerns too early.
There is often a significant amount of general design work that must happen before diving into architectural concerns
- Phrase questions so the subject can share their true thoughts; avoid leading questions
- When possible, use the subject's words when summarizing ideas
- Talk to real users and primary stakeholders of the system being designed
- Use data to help jump start conversations, such as _Response Measure Straw Man_
- Record the session or have a designated note taker so the interviewer can devote full attention to the subject

## Activity - List Assumptions
Assumptions are truths about the system taken for granted.
Hidden assumptions kill projects, or at least cause significant pain.

_List Assumptions_ takes assumptions out of the shadows by writing down as many assumptions as we can.
Use this info to plan further design work, prioritize next steps, improve ASRs, and improve the team's shared knowledge about the architecture.

Participants:
- whole team working in pairs or small groups (no more than 3-5)
- if done solo, share your assumptions list

### Benefits
- head off misunderstanding about the true goals and requirements
- great for ad hoc analysis; does not require a formal workshop or agenda
- avoid missing important requirements

### Guidelines and Hints
- Start by asking, _what do we think we know about x_?
- Write down everything mentioned, even if seemingly common knowledge
- Pause to discuss assumptions that are surprising or generate a reaction from any participants
- Record the assumptions

## Activity - Quality Attribute Web
The _quality attribute web_ is a brainstorming and visualization activity to help elicit, categorize, refine, and prioritize stakeholder concerns and raw quality attribute scenarios.

Participants: Any stakeholders, including the team

### Benefits
- guide stakeholders to think about quality attributes instead of features
- provide a visualization showing how one system is different from another based on highly desirable properties
- help stakeholders prioritize quality attribute scenarios before refining them

### Guidelines and Hints
- Some stakeholders will need help getting started; help them phrase their concerns initially
- Use dot voting to prioritize concerns on the web
- Don't worry about getting perfect scenarios; a general thought, worry, response measure, or partial scenario is a great start
- Combine with the _Mini-Quality Attribute Workshop_ for a more comprehensive workshop

## Activity - Mini-Quality Attribute Workshop (mini-QAW)
The _mini-quality attribute workshop_ is a lean, facilitated workshop designed to help you talk about quality attributes with stakeholders early in a system's life.
You collaborate as a group to quickly identify, develop, and clarify quality attributes with the help of a quality attribute taxonomy.
By the end, you will have a prioritized list of quality attribute scenarios and a wealth of contextual info about the system to be designed.

Participants
- a facilitator, usually the architect
- small group of stakeholder participants
- best in small groups of 3-5, with a maximum of 10 participants
- host multiple workshops if necessary to keep the group size down

### Benefits
- walk through the essential steps of a traditional quality attribute workshop in only a few hours
- quickly identify raw quality attributes and prioritize them before refining into full scenarios
- provide opportunities for stakeholders to riff on each other's ideas
- create a forum for open discussion among stakeholders to discuss quality attribute concerns, risks, and other general concerns about the software system

### Guidelines and Hints
- keep your taxonomy small, 5-7 quality attributes max
- use the _quality attribute web_ to drive the workshop
- don't worry about creating formal scenarios during brainstorming
- ask probing questions about the stimulus, response, environment
- pay attention when stakeholders sound worried about something; their worries are often the source of a possible scenario
- watch out for features and functional requirements (we are looking for quality attributes)

## Activity - Point-of-View Mad Lib
Summarize business goals and other stakeholder needs.
Here's a basic template to use, or create your own: [stakeholder] needs to [stakeholder's need] because [context].
- stakeholder: specific person or role
- stakeholder's need: measurable task
- context: insightful

The format is similar to agile stories, but the emphasis is on stakeholders' needs and how the overall system with provide value rather than specific features or functionality.

Participants
- any stakeholders
- can be done alone or as a small group of 2-3
- if it is a large group, divide it into subgroups of 2-3

### Benefits
- develop empathy for stakeholders' needs
- articulate business goals in a user-focused way
- start the conversation about business goals

### Guidelines and Hints
- getting the ideas out is more important than the phrasing at first
- the impact of each mad lib should be outcome focused.
Try the 5 Why's technique to help reach the stakeholders' real needs

## Activity - Response Measure Straw Man
The goal of a _response measure straw man_ is to give stakeholders something to beat up until they arrive at their own answers.
Do this by inventing a reasonable response measure for some ASR as a way to kickstart discussions.

Participants: architects often create these on their own and validate with stakeholders later

### Benefits
- provide an example of a measurable response and response measure
- jump-starts thinking about ASRs and quality attribute scenarios
- overcomes blank-page syndrome by providing something to edit instead of creating response measures from scratch

### Guidelines and Hints
- use a straw man to understand the boundaries around acceptable behavior
- responses should be correct for the scenario; the point is to zero in on an accurate and reasonable response measure
- listen to your stakeholders once you get them talking.
When presented with a wrong answer, many stakeholders will react with useful information
- keep an eye out for anchoring (cognitive bias)
- the straw man should be a reasonable estimate or so outrageous it will be rejected outright; be cautious if your outrageous estimate is accepted

## Activity - Stakeholder Map
A stakeholder map is a network diagram of the people involved with or impacted by the software system.
Use this method to visualize the relationships, hierarchies, and interactions between all the people who have an interest in the software system to be built.

Participants:
- whole team, known stakeholders
- no limit on the number of participants

### Benefits
- identify more stakeholders than just the usual suspects
- determine who to talk to about requirements
- help the team empathize with people and not just focus on technology
- create a snapshot of the system context and who's involved
- use as a document to bring new teammates up to speed or to assist with architecture validation

### Guidelines and Hints
- use simple icons to represent individual people; use multiple icons to represent groups
- be specific when naming stakeholders (role or person)
- use speech bubbles to represent stakeholders' needs or thoughts
- connect people using arrows tos how relationships and influence.
Label connections to describe relationships
- encourage participants to look beyond the obvious stakeholders if they stall out during the activity