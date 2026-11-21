# The Re-engineering Round

The re-engineering round gives the candidate several hundred lines of unfamiliar code that contain defects, and asks for the defects to be found and fixed. It is a debugging interview. The grade depends on method more than speed, because a customer trusts an engineer who can show why a fix is correct.

## What the round looks like

| Part | Commonly reported format |
|---|---|
| Material | A working-looking service or script of a few hundred lines |
| Defects | Two to four, of different kinds |
| Length | About 60 minutes |
| Starting point | A failing test, a wrong report, or a complaint in one sentence |
| Company most associated | [Palantir](../companies/palantir.md), as one of five onsite round types |

## Five steps for debugging unfamiliar code

1. **Reproduce.** Run the failing case and record the exact wrong output.
2. **Form a hypothesis.** State one cause that would produce that output.
3. **Isolate.** Find the smallest input that still shows the fault.
4. **Fix.** Change the least code that removes the cause.
5. **Verify.** Run the failing case, then the cases that passed before.

Say each step aloud. An interviewer cannot grade reasoning that stays silent.

## Common defect types

| Defect | Typical symptom | Where to look |
|---|---|---|
| Double counting | A total higher than the sum of its parts | A tally updated in two places, or a join that repeats rows |
| Boundary error | The first or last item is missing | Loop limits and date ranges |
| Missing value | A crash on some records only | Optional fields used without a check |
| Stale state | Correct on the first call, wrong on the second | A variable or cache kept between calls |
| Wrong unit or time zone | Values wrong by a fixed factor or by hours | Conversions at the edge of the system |

## A short worked example

A daily report says 1,260 claims were received, and the intake system says 1,200. The difference is 60, which is 5 percent.

- **Reproduce.** Run the report on one day's export and confirm 1,260.
- **Hypothesis.** Some claims are counted twice. A claim that is updated on the same day may appear as two rows.
- **Isolate.** Count distinct claim numbers in the export. The result is 1,200, and 60 claim numbers appear twice.
- **Fix.** Tally by claim number, not by row.
- **Verify.** The report now says 1,200. Run it on a second day, and check that the per-queue totals still sum to the overall total.

The whole chain takes about ten minutes when the steps are followed in order. A candidate who starts by reading all 300 lines from the top has usually not found the cause by then.

## What is graded

- A reproduction before any change to the code.
- One hypothesis at a time, each tested and then kept or rejected.
- A fix that removes the cause and not only the symptom. Subtracting 60 from the total is not a fix.
- Verification that includes the cases that worked before.
- A sentence on prevention, such as a test for duplicate claim numbers.

## Mistakes to avoid

- Changing several lines at once, so that no single change can be credited.
- Rewriting code that works because its style is unfamiliar.
- Stopping after the first defect. Ask whether more are expected.
- Fixing silently. The interviewer needs to hear the hypothesis before the fix.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-re-engineering-round) teaches the five-step method and has four runnable broken services to repair.
- Related round: [the learning round](learning-round.md).
- Related page: [practical coding](practical-coding.md).
- Free answer: [Strategies for debugging code in interviews](https://www.designgurus.io/answers/detail/what-are-the-strategies-for-debugging-code-in-interviews?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-re-engineering-round), general debugging methods for a live interview.
