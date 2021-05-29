# Chapter 13 - [Understand, Explore, Evaluate, Make] Empower the Architects on Your Team
Modern software architects design with their team.
They are part coach, mentor, and technical guru.
Let us learn how to grow and empower your team as you design software architectures together.

## Promote Architectural Thinking
A team that embraces the idea of _software architect_ as a way of thinking will produce better software.
Why?
- explore more design decisions faster
- documentation is leaner and conveys more knowledge
- shared ownership
- understanding of the intent behind the design
- creates force multipliers
- increased happiness

But not everyone is ready to accept more design responsibilities.
Therefore, nurture the team's design skills while simultaneously designing an architecture with them.

## Facilitate Decision Making and Foster Skills Growth
Infuse your team(s) with the knowledge and skills they need to make design decisions for themselves.
When this is going well, an architect is more like a coach/mentor than an authoritative leader making all the design decision.

| OK Software Architects | Great Software Architects |
| --- | --- |
| Select patterns and technology without input | Collaboratively select patterns and technologies with input from the team |
| Write detailed documents, release only once fully complete | Create document templates for the team to use, build and review documents with the team incrementally |
| Make or approve all design decisions | Teach the team how to decide, provide design guidance, delegate decision making, provide reviews and feedback |
| Dictate who builds specific elements | Help the group self-organize and choose work |
| Avoid changes to the architecture | Embrace the inevitability of change and make the architecture easy to change |
| Mandate technology decisions | Build consensus for technology decisions |

## Create Opportunities for Safe Practice
Teammates have to practice design to gain experience.
Here are some ways to create opportunities for safe practice:
- pair design
- create scaffolding
  - create support structures promoting and reinforcing learning (instructional scaffolding)
- introduce Architecture Guide Rails
  - an __architecture guide rail__ restricts design options to ensure detailed design stays within the bounds of the desired architecture
  - this is a form of constraint we choose for ourselves
- host information sessions
  - dive deep into specific topics
  - when doing so, teach relevant info JIT

When the team starts sharing feedback about the architecture, we can think about delegating more design authority.

## Delegate Design Authority
Give away as much design authority as possible without putting essential quality attributes at risk or endangering the architecture.
There are seven levels of authority:
- __Level 1: Tell__ You make the design decision and tell the team what will happen, usually by producing an artifact
- __Level 2: Sell__ You make the design decision and show the team why it is the right call
- __Level 3: Consult__ You ask the team for input before making the design decision; ultimately the decision is still yours
- __Level 4: Agree__ You collaborate with your team and reach consensus about the design decision as a group; everyone has an equal voice
- __Level 5: Advise__ You influence the team by sharing your opinions and insights but let someone else make the design decision
- __Level 6: Inquire__ You let the team make the design decision and ask them to show why their decision is the right one
- __Level 7: Delegate__ You leave the design decision to someone else
  - In this capacity, you might help gather information as a facilitator but someone else is responsible for the decision

Choosing the appropriate level of authority is trial-and-error and dependent on how the team likes to operate.
To choose the best level of authority, talk to the team and decide together.

## Design Architecture Together
In Chapter 1 (Build Amazing Software), we learned how software architecture improves our ability to shape software.
We also learned that architects guide the team to design an architecture.
Let's revisit the architect's key responsibilities from the perspective of the new knowledge we acquired since Chapter 1 (remember, these can become team-level as the team embraces the idea of software architect as a way of thinking):

__Define the problem from an engineering perspective.__
Architects are responsible for defining the ASRs.
Prefer to use human-centered design methods to gather these requirements so we don't lose touch with stakeholders' true needs.

__Partition the system and assign responsibilities to elements and teams.__
Architects guide the team to identify patterns that will promote desired quality attributes.
Prefer to minimally design the architecture to ensure key quality attributes are achieved, leaving all other decisions to downstream designers.

__Keep an eye on the bigger picture and ensure design consistency of the whole.__
Architects monitor the design as it emerges and shepherd the team as they implement the architecture.
Capture design decisions as accurate models using the lightest-weight documentation methods that work for the team and stakeholders.
Use these models to reason about the system, evaluate our decisions, and identify risks in our ability to achieve business goals.

__Decide trade-offs among quality attributes.__
Architects help the team reconcile trade-offs as design decisions are made and as the architecture evolves over time.
Use risk to determine how much design work is required and where to focus the team's attention.

__Manage technical debt.__
Architects deal with the reality of shipping software by identifying tech debt and devising strategies for paying it back.

__Grow the team's architecture skills.__
Architects empower their teams to take ownership of the system by ensuring the team has the knowledge and skills required to understand, explore, make, and evaluate an architecture.
Prefer to design the architecture with the team instead of for the team.