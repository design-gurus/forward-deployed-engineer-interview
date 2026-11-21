# The Take-Home Project

A take-home project asks the candidate to build a small working system alone, usually within about a week, and then defend it in a live review. It is graded on customer framing as much as on code. The reviewer wants to see what a customer would get from each decision, so a modest build with a clear write-up and a measured result beats a large build with neither.

## What is commonly reported

| Company | Take-home format |
|---|---|
| [OpenAI](../companies/openai.md) | A case study of about one week: working code, a running app, and a recorded video, followed by a live discussion. Some teams ask for a design document instead. |
| [Cognition](../companies/cognition.md) | A hands-on exercise inside the company's own product, with little code, judged on product understanding and customer value |

One reported task is: "Build a semantic search system over product data that an assistant can query."

## Four stages

| Stage | Share of the time | Output |
|---|---|---|
| Scope | 10 percent | A half-page plan: the user, what is in, what is out, and the success measure |
| Build | 50 percent | The smallest version that runs end to end, then improvements one at a time |
| Measure | 15 percent | A test set with known answers and one number |
| Write up and record | 25 percent | A document and a video a customer could follow |

A quarter of the time on the write-up looks high. It is the part the reviewer reads first, and often the only part every reviewer reads.

## Build in stages

Make the whole path work with the simplest parts before improving any one part. For the search task, the order is:

1. Load a sample of 2,000 products.
2. Return any five products for a question, through one endpoint.
3. Replace the placeholder with a real index of embeddings. An **embedding** is a list of numbers that represents the meaning of a text.
4. Write 40 test questions, each with a known correct product.
5. Improve the weakest step, and measure again.

After step 2 there is always something that runs. A candidate who spends four days on the index and has no endpoint on day five has nothing to submit.

## The write-up

| Section | Content |
|---|---|
| Result | One sentence a customer would repeat, with the number |
| What was built | Three or four parts, each in one line |
| How it was measured | The test set, the measure, and the failures |
| Decisions | Each decision with the alternative that was rejected and the reason |
| Limits | What it does not handle |
| Next steps | What would be done with two more weeks |

A result line for the search task: "The assistant finds products by meaning. The correct product is in the top 5 for 34 of 40 test questions, which is 85 percent."

## The live review

Reviewers commonly ask how the system would change if the customer's needs shifted. Prepare three answers before the call:

- **The failures.** Which of the 6 failed questions is the most serious, and what causes it.
- **Ten times the data.** How the index is stored and updated for 200,000 products without a full rebuild.
- **A new requirement.** For example, a filter by price. Apply it in fixed code before the search, because a filter must never be approximate.

Open with the customer's result, then the test number, then the main decision. Leave the architecture until someone asks.

## Mistakes to avoid

- Starting to build before writing the scope.
- Submitting without a number.
- Hiding the limits. Reviewers find them, and a stated limit reads as judgment.
- Using an AI tool where the instructions forbid it. Read the rules for the take-home, because they differ by company.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-take-home-project) has four lessons on the take-home: scoping, building in stages, the write-up, and the live review.
- Full guide: [What is the OpenAI forward deployed engineer interview like, round by round?](https://www.designgurus.io/answers/detail/what-is-the-openai-forward-deployed-engineer-interview-like-round-by-round?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-take-home-project)
- Related round: [the project deep dive](project-deep-dive.md).
