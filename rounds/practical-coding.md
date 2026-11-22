# Practical Coding

FDE coding rounds test the code an engineer writes at a customer site: cleaning an export, calling an API, querying a database, and extending a small program as requirements arrive. The bar is commonly reported as reasonable and not puzzle-based. Google is the exception, where a reported round uses algorithm problems in a shared document.

## The four task types

| Task type | Example | What is graded |
|---|---|---|
| Cleaning and joining messy data | Reconcile two exports whose customer names are spelled differently | Handling of missing and duplicate values, and a stated matching rule |
| Calling and wrapping an API | Fetch every page of results from a REST API, one page at a time | Pagination, retries, rate limits, and error handling |
| SQL for customer data | A join with a count or a sum per group | Correct joins, and awareness of rows that a join repeats or drops |
| Code that grows in stages | A credit system: add and spend, then expiry dates, then spend the credits that expire first | A structure that absorbs each new stage without a rewrite |

## Staged rounds

Many FDE coding rounds arrive in three or four stages, and the later stages are not shown at the start. The round measures whether the first design survives new requirements.

A reported example is a credit system. Stage 1 adds and spends credits. Stage 2 gives each grant an expiry day. Stage 3 spends the credits that expire first.

| Design choice in stage 1 | Effect in stage 2 | Effect in stage 3 |
|---|---|---|
| One running total | Must be rewritten, because a total has no expiry | Rewritten again |
| A list of grants, each with an amount | Add one field and one filter | Sort the list by expiry day |

With grants of 100 credits expiring on day 30 and 50 expiring on day 10, spending 70 on day 5 uses all 50 of the earlier grant and 20 of the later one. The balance is 80. On day 12 the balance is still 80, because the expired grant was already used.

The general rule is to store the smallest real unit (each grant, each event, each row) and compute totals from it.

## Habits that score well

- **State assumptions about the data.** "I will assume claim numbers are unique. I will check that before the join."
- **Run early.** Print the first five rows before writing the transformation.
- **Name the failure cases.** An empty page, a timeout, a null field, a duplicate key.
- **Keep input and output at the edges.** Logic that does not touch the network is easy to test and easy to extend.
- **Finish each stage before improving it.** A working stage 2 scores higher than an elegant stage 1.

## AI tools in the coding round

Reported rules differ, so ask the recruiter.

| Company | Commonly reported rule |
|---|---|
| Palantir | No AI tools in any round |
| OpenAI | A coding assistant is sometimes enabled in the coding screen; the candidate must explain every line it writes |
| Anthropic | No AI tools in live interviews unless an interviewer says otherwise |
| Google | One candidate report says no AI tools were allowed in coding |

When a tool is allowed, the code it writes is graded as the candidate's own. If it sorts a list inside a loop of n steps, the cost is about n times n log n operations. The candidate is expected to notice that and move the sort before the loop.

## A two-week practice set

1. Three data-cleaning tasks on real public exports, 45 minutes each.
2. Two API wrappers with pagination and retries.
3. Ten SQL queries with joins and grouping.
4. Three staged problems, with a friend revealing one stage at a time.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-practical-coding) has a chapter on practical coding with runnable exercises for each of the four task types.
- Lesson: [What Practical Coding Questions Test](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/what-practical-coding-questions-test?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-practical-coding), in Grokking the Forward Deployed Engineer Interview
- Lesson: [Cleaning and Joining Messy Data](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/cleaning-and-joining-messy-data?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-practical-coding), in Grokking the Forward Deployed Engineer Interview
- Lesson: [Code That Grows With Each Requirement](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/code-that-grows-with-each-requirement?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-practical-coding), in Grokking the Forward Deployed Engineer Interview
- For the "vibe coding" format, see [Google](../companies/google.md).
- Related rounds: [learning](learning-round.md) and [re-engineering](re-engineering-round.md).
- Free answer: [What is the Google FDE vibe coding round?](https://www.designgurus.io/answers/detail/what-is-the-google-fde-vibe-coding-round-how-it-works-and-how-to-prepare?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-practical-coding), how the round works and how to prepare.
