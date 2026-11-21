# The Decomposition Interview

A decomposition interview gives the candidate a short, vague customer need and about 60 minutes to turn it into a plan that could be built in weeks. The interviewer plays the customer. The round is graded on questions, scope, and data reasoning before it is graded on any design, which is why it is commonly reported to reject more strong coders than any other FDE round.

## What the questions look like

Reported questions are one sentence long and deliberately open:

- Design a system to improve traffic in a large city.
- Design a sync between two employee record systems.
- Let several teams query a shared dataset without seeing the raw records.
- Design an app to catalog species while exploring an unfamiliar environment.

More statements to practice on are in the [decomposition practice problems](../cheat-sheets/decomposition-practice-problems.md).

## A time budget for 60 minutes

| Minutes | Step | Output |
|---|---|---|
| 0 to 12 | Clarify | The user, the decision that user makes, and the data that exists |
| 12 to 17 | Scope | One sentence of scope, confirmed by the interviewer |
| 17 to 35 | Decompose | Four to six parts, each with an input and an output |
| 35 to 52 | Design the first version | The parts needed for a version that ships in weeks |
| 52 to 60 | Plan the next version | What is added second, and the measure that triggers it |

## What is graded

Preparation guides commonly report five criteria:

1. **A structured breakdown.** The problem is divided into named parts, not described as one large system.
2. **Empathy for a named user.** The plan serves one person with one decision, such as "a traffic planner who chooses where to change signal timing".
3. **Explicit data reasoning.** The candidate asks what data exists, who owns it, and how complete it is.
4. **A first version buildable in weeks.** It covers a part of the problem and delivers a measured result.
5. **Iteration.** The candidate names what comes next and adapts when a constraint changes.

## Seven patterns that cover most questions

Most decomposition questions are one of a small number of shapes. Recognizing the shape gives the first breakdown quickly.

| Pattern | Example |
|---|---|
| Automating a human review queue | Routing insurance claims |
| Syncing two systems of record | Two employee record systems |
| A data pipeline with a decision screen | Warehouse stockouts |
| An assistant over documents | Contract review |
| Monitoring events and raising alerts | Energy usage alerts |
| Sharing data without exposing records | A shared research dataset |
| Forecasting and planning tools | School bus routing |

## A short worked example

The question is the traffic one. A weak opening proposes sensors, a stream processor, and a machine learning model within two minutes. A strong opening sounds like this:

> "Before I design anything, I would like to know who uses this. I will assume a city traffic planner who decides where to change signal timing. Which data does the city have today: signal logs, road sensors, or accident reports?"

Suppose the interviewer answers that only 200 intersections have sensors. The first version then covers those 200 and supports one decision there: which 10 intersections should have their timing changed this month. The success measure is average delay at those 10 after four weeks. The next version estimates delay at intersections without sensors.

When the interviewer changes a constraint, change the plan and say what the change costs. A candidate who defends the old plan loses the iteration criterion.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-decomposition) teaches the seven patterns and works twelve problems in full, each with a weak and a strong answer.
- Full guide: [What is the Palantir decomposition interview, and how does the round work?](https://www.designgurus.io/answers/detail/what-is-the-palantir-decomposition-interview-how-the-fde-round-works?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-decomposition)
- Next page: [discovery and scoping](discovery-and-scoping.md), the first 17 minutes in detail.
