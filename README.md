# Forward Deployed Engineer Interview

> The free, open companion to **Grokking the Forward Deployed Engineer Interview** by [DesignGurus.io](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=readme), created by Arslan Ahmad.

A forward deployed engineer (FDE) is a software engineer who works inside a customer's organization and makes a product work on that customer's data, systems, and rules. The interview loop therefore measures skills that a standard software engineer loop does not: turning a vague customer need into a plan, learning an unfamiliar system quickly, and earning trust in front of a customer. This repository explains each round and each company's reported loop in a short read. For worked problems, runnable exercises, and full mock loops, see the course.

[![GitHub stars](https://img.shields.io/github/stars/design-gurus/forward-deployed-engineer-interview?style=social)](https://github.com/design-gurus/forward-deployed-engineer-interview/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/design-gurus/forward-deployed-engineer-interview)](https://github.com/design-gurus/forward-deployed-engineer-interview/commits/main)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## Start here

| Your situation | Read this first |
|---|---|
| You have a recruiter call and do not know what the loop contains | [The interview loop](rounds/interview-loop.md) |
| You are a strong coder and have never done a decomposition round | [Decomposition](rounds/decomposition.md), then the [practice problems](cheat-sheets/decomposition-practice-problems.md) |
| You are interviewing at one specific company | [Loops by company](companies/README.md) |
| You are deciding between FDE, solutions architect, and software engineer roles | [The three roles compared](cheat-sheets/fde-vs-solutions-architect-vs-software-engineer.md) |
| You have about a month | [The four-week plan](cheat-sheets/four-week-plan.md) |

## What is in this repository

### Rounds

| Page | What it covers |
|---|---|
| [The interview loop](rounds/interview-loop.md) | The stages, the round types, and what each one measures |
| [Decomposition](rounds/decomposition.md) | The signature round: a vague customer need turned into a buildable plan in 60 minutes |
| [Discovery and scoping](rounds/discovery-and-scoping.md) | The questions for the first ten minutes and the one-page scope |
| [The learning round](rounds/learning-round.md) | Extending unfamiliar code from documentation, in stages |
| [The re-engineering round](rounds/re-engineering-round.md) | Finding and fixing defects in code you did not write |
| [Practical coding](rounds/practical-coding.md) | Messy data, APIs, SQL, and code that grows with each requirement |
| [Applied AI system design](rounds/applied-ai-system-design.md) | Rules, models, and people; retrieval, agents, evaluation, and cost |
| [The take-home project](rounds/take-home-project.md) | Scoping, building in stages, the write-up, and the live review |
| [The project deep dive](rounds/project-deep-dive.md) | Presenting one past project and defending each decision |
| [Behavioral questions for customer work](rounds/behavioral-for-customer-work.md) | Motivation, difficult customers, scope, failure, and field feedback |

### Companies

| Page | Reported shape of the loop |
|---|---|
| [Palantir](companies/palantir.md) | Three onsite rounds drawn from five types, with decomposition in nearly every onsite |
| [OpenAI](companies/openai.md) | A take-home case study, staged coding, and system design with models |
| [Anthropic](companies/anthropic.md) | A technical use-case screen and a final values panel |
| [Google](companies/google.md) | A coding round in a shared document, a "vibe coding" round, and a hiring committee |
| [Cognition](companies/cognition.md) | A product take-home, an executive pitch, and a simulated customer call |

### Cheat sheets

| Page | What it covers |
|---|---|
| [Question bank](cheat-sheets/question-bank.md) | About 50 questions grouped by round |
| [Decomposition practice problems](cheat-sheets/decomposition-practice-problems.md) | 14 problem statements, each with its first two clarifying questions |
| [FDE, solutions architect, and software engineer](cheat-sheets/fde-vs-solutions-architect-vs-software-engineer.md) | One customer request handled by three roles |
| [Four-week plan](cheat-sheets/four-week-plan.md) | 32 hours of preparation, weighted toward the rounds that decide the loop |
| [Common mistakes](cheat-sheets/common-mistakes.md) | The errors that reject strong engineers, and the correction for each |

## Loops by company

No company below publishes a fixed FDE loop. Every row is commonly reported by candidates and preparation guides, and loops change often, so confirm the format with your recruiter.

| Company | Signature stage | Coding style | AI tools in live rounds | Reported length |
|---|---|---|---|---|
| [Palantir](companies/palantir.md) | Decomposition | Practical coding, plus learning and re-engineering | Not allowed | About a month |
| [OpenAI](companies/openai.md) | Take-home case study | Staged, easy to medium | Sometimes enabled in the coding screen | Three to six weeks |
| [Anthropic](companies/anthropic.md) | Final values panel | Multi-stage, requirements grow | Not allowed unless an interviewer says otherwise | Four to six weeks |
| [Google](companies/google.md) | "Vibe coding" and agentic design | Algorithms in a shared document | One report says not allowed in coding | Six to eight weeks |
| [Cognition](companies/cognition.md) | Executive pitch and customer call | Little; a take-home inside the product | The take-home uses the company's own AI product | Not reliably reported |

## FAQ

### What is a forward deployed engineer?

A forward deployed engineer is an engineer who is sent to a customer to make a product deliver a measured result there. The work includes discovery with the customer's staff, building against the customer's data, running a pilot, and handing the system to the customer's own team. The engineer also carries field feedback to the product team, which is how customer needs become product features.

### What is asked in an FDE interview?

Most loops combine four kinds of rounds: a customer problem worked out loud (decomposition or a case), practical coding, a design round that now usually includes models, and behavioral questions about customer work. Some companies add a take-home project, a project deep dive, a learning round, or a re-engineering round. The [interview loop](rounds/interview-loop.md) page maps each round to the job task it tests.

### What is a decomposition interview?

A decomposition interview is a round of about 60 minutes in which the interviewer plays a customer with a vague need, and the candidate turns it into a plan that could be built in weeks. It is graded on the questions asked, the named user, the data reasoning, and the first version, and far less on architecture. See [Decomposition](rounds/decomposition.md).

### Is forward deployed engineer a software engineering role?

Yes. FDEs write production code, and every reported loop includes at least one coding stage. The difference is where the work happens and what is graded: the code serves one customer's decision, and the loop gives more weight to scoping and communication than a standard software engineer loop does.

### How is an FDE different from a solutions architect?

A solutions architect usually designs and advises before and during a sale, and the customer or a partner builds the system. An FDE builds the system and stays until it works in production. The [comparison page](cheat-sheets/fde-vs-solutions-architect-vs-software-engineer.md) shows one request handled by all three roles, and the sibling repository [solutions-architect-interview](https://github.com/design-gurus/solutions-architect-interview) covers that loop.

### How long does it take to prepare?

About 8 hours a week for four weeks, or 32 hours, is enough for an engineer who already codes comfortably. More than a third of that time should go to decomposition, because it appears in nearly every loop in some form. The [four-week plan](cheat-sheets/four-week-plan.md) gives the split.

## Go deeper

This repository is an index. The courses hold the worked material.

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=readme): the vendor-neutral course. It has a decomposition pattern bank with twelve worked problems, runnable learning-round and re-engineering exercises, and three written mock loops with rubrics.
- [Grokking the Anthropic Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-anthropic-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=readme): the Claude-specific companion, with runnable staged coding exercises and the values round.
- [Grokking the Google Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-google-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=readme): the Google-specific companion, covering the teams, the coding round, the "vibe coding" round, and the hiring committee.

Related free repositories: [grokking-ai-system-design](https://github.com/design-gurus/grokking-ai-system-design), [solutions-architect-interview](https://github.com/design-gurus/solutions-architect-interview), and [staff-engineer-interview](https://github.com/design-gurus/staff-engineer-interview).

## Contributing

Corrections and reports of how a round was run are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) first. This guide is independent and is not affiliated with any company it names.

## License

The content is licensed under [CC BY 4.0](LICENSE). See [NOTICE.md](NOTICE.md) for what the license covers and how to attribute.
