# The Forward Deployed Engineer Interview Loop

An FDE loop usually has a recruiter call, one early technical stage, and an onsite of three to six interviews. The rounds are built from the tasks of the job, so the fastest way to understand a loop is to map each round to the task it copies. No company publishes a fixed loop, and the details below are commonly reported, not official.

## The stages

| Stage | Commonly reported format | What it measures |
|---|---|---|
| Recruiter call | About 30 minutes | Motivation for customer work, background, communication |
| Early technical stage | A live coding screen of 45 to 60 minutes, a timed online test, or a take-home of about a week | Practical coding and, for a take-home, customer framing |
| Onsite | Three to six interviews of about 60 minutes each | The round types in the next table |
| Final conversation | A hiring manager interview, a values panel, or a hiring committee review | Ownership, judgment, and the weakest area from the onsite |

The whole process is commonly reported to take three to eight weeks, depending on the company.

## Job tasks and the rounds that test them

| Task on the job | Round that tests it |
|---|---|
| Sit with a customer and find the real problem | [Decomposition](decomposition.md), [discovery and scoping](discovery-and-scoping.md), simulated customer call |
| Start work in a codebase nobody explained | [Learning round](learning-round.md) |
| Repair a system that is failing in production | [Re-engineering round](re-engineering-round.md) |
| Write code against messy exports and third-party APIs | [Practical coding](practical-coding.md) |
| Decide where a model belongs in the customer's process | [Applied AI system design](applied-ai-system-design.md) |
| Deliver a working first version alone | [Take-home project](take-home-project.md) |
| Explain a finished project to the customer's leaders | [Project deep dive](project-deep-dive.md), executive pitch |
| Decline a request, admit a failure, keep trust | [Behavioral questions](behavioral-for-customer-work.md) |

## How it differs from a software engineer loop

| | Software engineer loop | FDE loop |
|---|---|---|
| Hardest round | Algorithms or distributed system design | A customer problem worked out loud |
| Coding questions | Often puzzles with one best answer | Practical tasks that grow in stages |
| Design round | Scale and storage for a known product | One customer's process, data, and constraints |
| Behavioral questions | One dedicated round | Often inside every round as well |
| Grading of questions | Clarifying questions help | Clarifying questions are a scored part of the answer |

## Three rules that apply to most loops

1. **Ask which rounds allow AI tools.** Reported rules differ by company and by round. Some loops forbid them, and one enables a coding assistant and then asks the candidate to explain every line.
2. **Expect a constraint to change mid-round.** Interviewers commonly change one fact to see whether the candidate adapts the plan and states the cost of the change.
3. **Prepare the weakest area again.** A hiring manager is commonly reported to return to the round that went worst.

## A worked example of weighting

A candidate with 32 hours to prepare for a loop with decomposition, learning, and coding rounds should not divide the time equally. Decomposition is the round that most often rejects strong coders, so it receives 12 hours. Learning and re-engineering receive 8 hours, practical coding receives 8, and stories and motivation receive 4. The [four-week plan](../cheat-sheets/four-week-plan.md) lays this out by week.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-interview-loop) has a lesson that maps every job task to its round, then a chapter for each round.
- Lesson: [How FDE Interview Loops Test the Job](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/how-fde-interview-loops-test-the-job?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-interview-loop), in Grokking the Forward Deployed Engineer Interview
- Lesson: [What a Forward Deployed Engineer Does](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/what-a-forward-deployed-engineer-does?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-interview-loop), in Grokking the Forward Deployed Engineer Interview
- Full guide: [What is the forward deployed engineer interview process like, round by round?](https://www.designgurus.io/answers/detail/what-is-the-forward-deployed-engineer-interview-process-like-round-by-round?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-interview-loop)
- Company details: [loops by company](../companies/README.md).
- Free answer: [Forward deployed engineer vs. solutions architect vs. software engineer](https://www.designgurus.io/answers/detail/forward-deployed-engineer-vs-solutions-architect-vs-software-engineer-what-is-the-difference?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-interview-loop), how the three roles and their interviews differ.
