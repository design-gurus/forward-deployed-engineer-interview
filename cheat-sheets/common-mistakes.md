# Common Mistakes in the FDE Interview

Most candidates who fail an FDE loop are capable engineers who answered as if it were a software engineer loop. The mistakes below are the ones commonly reported, grouped by round, each with its correction. Almost all of them come from the same cause: starting to build before knowing who the work is for.

## In customer rounds

| Mistake | Why it costs the round | Correction |
|---|---|---|
| Proposing an architecture in the first two minutes | Questions and scope are graded before design | Spend the first 12 minutes of 60 on questions |
| No named user | Empathy for a user is a stated criterion | Name one role and one decision, and ask the interviewer to confirm |
| Assuming the data exists | Data reasoning is graded | Ask what is recorded, who owns it, and how complete it is |
| A first version that takes a year | The criterion is a version buildable in weeks | Handle part of the problem completely |
| Defending the plan after a constraint changes | Iteration is graded | Change the plan and state what the change costs |
| Never saying what is out of scope | Leaving something out is a decision | Name it, with a reason |

## In coding rounds

| Mistake | Correction |
|---|---|
| Treating a practical task as a puzzle and optimizing early | Make it work on real input first, then improve |
| Storing a running total in stage 1 | Store the smallest unit (each grant, each event) and compute totals |
| Ignoring empty pages, null fields, and duplicates | Name the failure cases before coding |
| Using an AI tool where it is not allowed | Ask the recruiter for the rule in each round |
| Accepting AI-written code without reading it | Explain every line, including its running time |
| Reading unfamiliar code from the top | Follow one request from entry to exit |
| Fixing before reproducing | Run the failing case and record the wrong output first |

## In design rounds with models

| Mistake | Correction |
|---|---|
| Giving every step to the model | Say which steps are fixed code, which are the model's, and which are a person's |
| Letting a model decide who may read a record | Keep permission checks in fixed code, before retrieval |
| No measure of quality | Bring a test set with known answers and one number |
| Putting all the documents into one request | Size the task in tokens, then process one item per step |
| An agent with no limits | Add a step budget, repeat detection, a timeout, and a handoff to a person |
| No cost estimate | Multiply requests per day by tokens per request, and show the calculation |

## In take-homes and deep dives

| Mistake | Correction |
|---|---|
| Building for six days and writing for one hour | Give about a quarter of the time to the write-up and the video |
| Opening with the architecture | Open with the customer's result and the number |
| Hiding the limits | State them; reviewers find them, and a stated limit reads as judgment |
| Saying "we" for every decision | Say what you personally decided |
| Reaching the impact at minute 30 of a 45-minute talk | State it in the first five minutes |

## In behavioral and values rounds

| Mistake | Correction |
|---|---|
| One answer for "Why FDE?" and "Why this company?" | Prepare two different answers |
| Vague verbs such as "aligned" and "managed" | Quote what you said |
| A failure story with no cost | Give the cost as a number, and the change you made |
| Agreeing with everything the company publishes | Name one real point of disagreement and what would change your mind |
| A feature list in an executive pitch | Give a business outcome with arithmetic, and propose a pilot that measures it |
| Promising a result to a simulated customer | Promise a measurement |

## The three that matter most

If time allows only three corrections, choose these:

1. **Ask before designing.** Twelve minutes of questions in a 60-minute round.
2. **Scope down aloud.** Say what the first version leaves out and why.
3. **Bring a number.** Every design, take-home, and story ends in one.

A quick self-test: record yourself on one [practice problem](decomposition-practice-problems.md), and note the minute at which you first propose a component. Before minute 10 is too early.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-common-mistakes) pairs a weak and a strong answer for each round, so the difference is visible, and ends with three mock loops scored against rubrics.
- Start with [the interview loop](../rounds/interview-loop.md) if you have not read it.
