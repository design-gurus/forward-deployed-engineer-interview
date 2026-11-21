# The Project Deep Dive

In a project deep dive, the candidate presents one past project and defends the decisions in it. Interviewers ask what the candidate personally owned, why each approach was chosen, and where the system would fail under load. For an FDE, the round also tests a job skill directly: explaining finished work to a customer's leaders.

## Where it appears

| Company | Commonly reported form |
|---|---|
| [OpenAI](../companies/openai.md) | Present and defend a past system as one onsite interview |
| [Anthropic](../companies/anthropic.md) | The hiring manager round centers on one project |
| [Cognition](../companies/cognition.md) | A presentation of about 45 minutes to a panel, in which some panelists may play a customer |

## Choosing the project

Score each candidate project from 0 to 2 on five criteria, and present the one with the highest total.

| Criterion | 2 points when |
|---|---|
| A real user | A named group used it, outside the engineering team |
| Decisions that were yours | At least three choices were made by you, not inherited |
| A measured result | One number changed, with a before and an after |
| Something that went wrong | A real problem occurred, and you can describe the correction |
| Recent enough to recall | You can answer questions three levels deep |

A project from a customer or stakeholder setting scores above a larger internal one, because the loop is hiring for customer work.

## Structure for a 45-minute presentation

| Minutes | Part | Content |
|---|---|---|
| 0 to 5 | Impact | The user, the problem, and the result as a number |
| 5 to 15 | Context and constraints | What was fixed: deadline, data, team size, rules |
| 15 to 30 | Decisions | Three decisions, each with the alternative rejected |
| 30 to 35 | What went wrong | One problem, its cost, and the change made |
| 35 to 45 | Questions | Kept free; do not fill this time with slides |

State the impact within the first five minutes. A presentation that reaches the result at minute 30 has lost the listeners who needed it first.

## An opening that works

> "Claims adjusters at a regional insurer were routing 1,200 claims a day by hand, and a claim took two days to reach the right queue. In six weeks we moved 70 percent of claims to automatic routing, and those claims now reach their queue in under an hour. I will cover the three decisions that mattered and the one that I got wrong at first."

The opening names the user, gives a before and an after, and promises a mistake. Each of those is something the panel is listening for.

## Follow-up questions to prepare

Prepare each decision three levels deep: the alternative, the numbers, and the second-order effect.

| Level | Question | Example answer |
|---|---|---|
| 1 | "Why not route all six queues from the start?" | "An error on an injury claim costs far more than one on a glass claim." |
| 2 | "How did you know the accuracy was sufficient?" | "On 2,000 past claims with a known queue, it matched the adjusters on 97 percent." |
| 3 | "What happened to the other 3 percent?" | "They fell below the confidence threshold and went to an adjuster with a suggestion." |

Also prepare these three, which are commonly reported at AI companies:

- Which part would fail first at ten times the load?
- Where was a model the wrong tool, and what replaced it?
- What would you do differently with the same six weeks?

## When a panelist plays a customer

A panelist may act less technical or impatient. Answer in the customer's terms: hours saved, errors avoided, and what staff do differently. Offer the technical detail only when asked.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-project-deep-dive) has four lessons on deep dives and presentations, including presenting to executives.
- The staff-level version of this round is in [staff-engineer-interview](https://github.com/design-gurus/staff-engineer-interview).
- Related round: [the take-home project](take-home-project.md).
