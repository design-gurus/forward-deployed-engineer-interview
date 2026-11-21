# Palantir Forward Deployed Software Engineer Interview

The Palantir onsite is commonly reported to draw three rounds from a pool of five types, and decomposition appears in nearly every onsite. Palantir calls the role forward deployed software engineer (FDSE). Palantir does not publish a fixed loop, so every fact below comes from candidate reports and preparation guides. Confirm the current format with your recruiter.

## The stages

| Stage | Reported length | What it tests |
|---|---|---|
| Recruiter call | About 30 minutes | Background, motivation, and fit for customer work |
| Technical screen | 45 to 60 minutes live, or a timed online test | Practical coding framed around an end user |
| Onsite | Three rounds of about 60 minutes, drawn from five types | Decomposition, learning, coding, re-engineering, system design |
| Hiring manager | 30 to 60 minutes | Ownership, motivation, and the weakest area from the onsite |

Reports differ on the number of onsite rounds, from three to five. Plan for three rounds and about a month in total.

## Two rules for the whole loop

1. **AI tools are reported as not allowed in any round.** Practice coding without them.
2. **Behavioral questions appear inside nearly every round.** They are reported to take about 15 to 20 minutes of each technical round.

## The five onsite round types

| Round | What happens | Page |
|---|---|---|
| Decomposition | The interviewer plays a customer with a vague need, and you produce a buildable plan | [Decomposition](../rounds/decomposition.md) |
| Learning | You extend unfamiliar code from its documentation, in stages | [Learning round](../rounds/learning-round.md) |
| Coding | A practical problem, not a puzzle | [Practical coding](../rounds/practical-coding.md) |
| Re-engineering | You find and fix defects in several hundred lines of code | [Re-engineering round](../rounds/re-engineering-round.md) |
| System design | Often a data pipeline | [Applied AI system design](../rounds/applied-ai-system-design.md) |

Decomposition is most often paired with the learning round and the coding round. With decomposition fixed, the other two rounds come from four types, which gives 6 possible pairs. The second and third rounds cannot be predicted, so prepare all four.

## The screen

The recruiter call is reported to be a real filter. Prepare a specific reason for wanting customer work, and an honest view on government and defense customers.

The technical screen is either live coding or an online test. Reported tasks include fetching paginated data from a REST API one page at a time, and a SQL join with a count or a sum.

## The decomposition round

Reported questions include improving traffic in a large city, syncing two employee record systems, and letting several teams query a shared dataset without seeing raw records. The reported grading has five parts: a structured breakdown, empathy for a named user, explicit data reasoning, a first version buildable in weeks, and a path to the next version.

A workable split of the 60 minutes is 12 for clarifying, 5 for scoping, 18 for decomposing, 17 for the design, and 8 for the next version.

## The hiring manager interview

The hiring manager is commonly reported to return to the weakest onsite area. A candidate whose decomposition answer said little about data should expect questions about data. The conversation also covers motivation, ambiguity, and difficult stakeholders.

## What the loop weights

| Skill | Weight |
|---|---|
| Turning a vague problem into a plan | Highest: nearly every onsite |
| Learning an unfamiliar system | High: often paired with decomposition |
| Practical coding | Medium: a reasonable bar |
| Trust in front of a customer | Present in every round |
| Distributed system design | Lower for this role |

This table is a reading of the reported facts, not a published rubric.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=companies-palantir) covers every Palantir round type and includes a full written Palantir-style mock onsite with interviewer notes.
- Full guide: [What is the Palantir decomposition interview, and how does the round work?](https://www.designgurus.io/answers/detail/what-is-the-palantir-decomposition-interview-how-the-fde-round-works?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=companies-palantir)
- Practice: [decomposition practice problems](../cheat-sheets/decomposition-practice-problems.md).
