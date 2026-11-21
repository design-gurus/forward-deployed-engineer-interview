# Anthropic Forward Deployed Engineer Interview

The Anthropic forward deployed engineer loop is commonly reported to have six stages over four to six weeks, ending in a final panel on behavior and values that can decide the result by itself. Candidates call that panel the hardest stage. Anthropic does not publish an official loop for this role, and the order of stages varies by team, so confirm it with your recruiter.

## The stages

| Stage | Reported format | What it tests |
|---|---|---|
| Recruiter screen | About 30 minutes | Motivation, use of the company's products, level, references |
| Technical use-case screen | A practical task, sometimes with live access to Claude | Planning a long-running task, managing context, consistent output |
| Coding round | Multi-stage, often on an online coding platform | Code that adapts as each stage adds a requirement |
| Hiring manager round | A deep dive on one past project | Decisions, scaling, and when a model fits |
| Solution design | Architecture for a customer | Enterprise design, security, and failure modes |
| Final panel | Behavioral and values interviews | Mission fit, ethics, and self-awareness |

AI tools may be used to prepare. They are reported as not allowed during live interviews unless an interviewer says otherwise.

## The recruiter screen and references

The recruiter asks why you want this role and how you use the company's products today. Name one task you do with the product every week and one thing you would change. References may be requested early, usually a former manager and a close coworker, so contact both before the screen.

## The technical use-case screen

This screen tests whether you can plan a task that a model performs over many steps. The amount of text a model can read at once is its **context window**, and interviewers watch how you manage it.

Suppose a customer wants the renewal date and notice period from 400 supplier contracts of about 6,000 words each. A **token**, the unit a model reads, is about three quarters of a word, so one contract is about 8,000 tokens and all 400 are about 3.2 million. A plan that works has four parts:

- One contract per step.
- A fixed output format with the same three fields each time.
- A check in fixed code, with one retry and then a person.
- Results written to a table outside the context, with a short progress note.

State the size of the task in tokens before presenting the plan.

## The coding round

Each stage adds a requirement that forces a change to earlier code. One reported example is an LRU cache extended as constraints change. An **LRU cache** keeps the most recently used items and drops the least recently used one when it is full. Keeping the removal logic in one function means a new limit changes only that function. See [practical coding](../rounds/practical-coding.md).

## Hiring manager and solution design

The hiring manager round centers on one project: why you chose your approach, where it would break at scale, and when a model is the wrong tool. See [the project deep dive](../rounds/project-deep-dive.md).

Solution design asks for a system for a customer. It is framed around AI, although the work is often mostly infrastructure. Reported examples include an API for requesting outputs from large models and security for a regulated customer. Name failure modes before the interviewer asks.

## The final values panel

Reported topics include "Why Anthropic?", a moral conflict, a time you were wrong, and pressure from an executive. Read the company's published views on AI safety and form your own position.

A strong answer to "Where do you disagree with us?" names one specific point, gives a reason from your own experience, and says what evidence would change your mind. "I agree with everything you publish" is a weak answer, because it shows no independent judgment.

## Go deeper

- [Grokking the Anthropic Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-anthropic-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=companies-anthropic) is the company-specific course: the Claude platform, six runnable staged coding exercises, the values round, and mock loops.
- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=companies-anthropic) covers discovery, decomposition, and general applied AI.
- Full guide: [What is the Anthropic forward deployed engineer interview like, round by round?](https://www.designgurus.io/answers/detail/what-is-the-anthropic-forward-deployed-engineer-interview-like-round-by-round?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=companies-anthropic)
