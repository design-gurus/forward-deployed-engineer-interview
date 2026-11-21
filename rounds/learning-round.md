# The Learning Round

The learning round measures how quickly a candidate can use something never seen before. The candidate receives documentation and unfamiliar code, then extends the code over a few short stages while the interviewer watches. It copies the first week of every customer engagement, when an FDE must work inside a system that nobody has time to explain.

## What the round looks like

| Part | Commonly reported format |
|---|---|
| Material | An unfamiliar library, API, or small service, with its documentation |
| Task | Three or four stages, each adding one requirement |
| Length | About 60 minutes |
| Questions | Allowed and expected; the interviewer answers as a coworker would |
| AI tools | Reported as not allowed at Palantir, the company most associated with this round |

## What is graded

- **Reading before writing.** The candidate finds the entry point and the data model before changing anything.
- **Precise questions.** A question is evidence. "What does this function return when the record is missing?" scores higher than "How does this work?"
- **Small verified steps.** Each change is run and checked before the next one.
- **Stating what is still unknown.** A candidate who says "I have not read the retry logic, so I will not touch it" shows judgment.

## A method for the first ten minutes

| Minutes | Action | Output |
|---|---|---|
| 0 to 3 | Read the task and the table of contents of the documentation | The two or three sections that matter |
| 3 to 6 | Find where a request enters the code and follow one path to the end | A one-line description of the flow |
| 6 to 8 | Read the main data structure and one existing test | The shape of the data |
| 8 to 10 | Say the plan for stage 1 aloud and ask one precise question | An agreed first step |

Ten minutes of reading in a 60-minute round feels long. It is cheaper than rewriting a stage that was built on a wrong guess.

## Weak and strong questions

| Weak question | Strong question |
|---|---|
| "Can you explain this file?" | "This handler calls `validate` twice. Is the second call intended?" |
| "What should I do next?" | "Stage 2 needs the claim's region. Is it on the claim record, or must I join it from the policy table?" |
| "Is this right?" | "My change returns an empty list for an unknown queue. Would you prefer an error?" |

A strong question names what the candidate already found, then asks for the one fact that cannot be read from the code.

## A short worked example

The material is a small claims service of about 300 lines. Stage 1 asks for a new field in the response. Stage 2 asks for a filter by date. Stage 3 asks that the filter also work for claims with no date recorded.

A candidate who read the data model first already knows that the date field is optional in 1 record of every 10 in the sample data. That candidate handles the missing value in stage 2 and finishes stage 3 in two minutes. A candidate who skipped the reading discovers the missing dates as a crash in stage 3, with eight minutes left.

## How to practice

Choose a library never used before. Set a timer for 45 minutes and build one small feature using only its documentation. Afterward, write down every question that arose and rewrite each one in the strong form above. Four sessions of this kind change the habit.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-learning-round) has two method lessons and four runnable staged exercises on a small claims service.
- Related round: [re-engineering](re-engineering-round.md), where the unfamiliar code is also broken.
- Company page: [Palantir](../companies/palantir.md).
