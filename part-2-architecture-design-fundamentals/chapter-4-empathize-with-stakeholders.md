# Chapter 4 - [Understand] Empathize with Stakeholders
> A __stakeholder__ is any person with an interest or concern in the software.

An architect identifies stakeholders and their needs/expectations in order to make better design decisions.
Only then can we understand the problem to solve; only then can we begin designing the architecture.

## Create a Stakeholder Map
> A __stakeholder map__ is a network diagram showing all the people involved with or affected by the proposed software system.

Stakeholder maps are ideal for visualizing relationships and interactions among people.
They also provide a snapshot of what motivates different stakeholders.
Use stakeholder maps to decide who the most important people are to talk to about their concerns.

After creating a stakeholder map, look for candidates for interviews and further research, look for areas to investigate further:
- who is paying for the software?
- who uses it?
- are there network hubs with many incoming or outgoing arrows?
- are there stakeholders with potential conflicts of interest?

Here is a partial stakeholder map purposefully kept simply by removing some stakeholders:

## Discover the Business Goals
> __Business goals__ describe what stakeholders hope to accomplish with the software; the fundamental purpose.

Business goals:
- seed conversations about quality attributes, trade-offs, and tech debt
- help us prioritze competing concerns
- are a primary architectural driver

Here is a summary of common business goal categories:
| Who wants it | What they want |
| --- | --- |
| Individuals | increase wealth, power, reputation, personal enjoyment, or knowledge |
| Organizations | increase revenue, maximize profits, grow the business, become a market leader, improve stability, enter a new market, beat a competitor |
| Employees | interesting and meaningful work, increase knowledge, help users, become recognized as an expert |
| Dev Team | improve specific quality attributes, reduce costs, add new features, implement a standard, improve time-to-market |
| Nations, Governments | security, civic welfare, social responsibility, legal compliance |

### Record Business Goal Statements
Capture business goals as simple need-based statements explaining what stakeholders will get from the software system.
Great business goal statements are measurable and have clear success criteria.

Business goal statements include:
- subject: a specific person or role
- outcome: express the stakeholder's need as a measurable outcome. How does the world change if the system is successful?
- context: context shares an insight about a stakeholder's need and helps build empathy. Ideally, cointext is insightful rather than completely obvious

Most systems have 3-5 business goals; anymore becomes confusing and hard to remember.
If working with many stakeholders, it is useful to records goals' relative importance (for example, must-have or nice-to-have).

Examples of business goals using a table:
| Stakeholder/Subject | Goal/Outcome | Context |
| --- | --- | --- |
| Mayor van Damme | Reduce procurement cost by 30% | avoid making budget cuts to education or other essential services in an election year |
| Office of Management and Business | review historical procurement data for the past 10 years | Businesses behave similarly over time and historic data gives the city a leg up when reviewing contract bids |