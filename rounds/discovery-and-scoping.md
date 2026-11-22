# Discovery and Scoping

Discovery is the work of finding out who the user is, what decision that user makes, and what data exists. Scoping is the choice of the smallest version that delivers a measured result. Together they fill the first third of every customer round, and interviewers score them directly, because a correct design for the wrong problem has no value to a customer.

## Five things to establish

| Item | Question to ask | A usable answer |
|---|---|---|
| The user | "Who does this work today?" | "Claims adjusters, about 20 of them" |
| The decision | "What do they decide, and how often?" | "Which of six queues each claim goes to, 1,200 times a day" |
| The data | "What is recorded, where, and how complete is it?" | "A form and photos for every claim, a scanned report for some" |
| The cost today | "How long does it take, and what goes wrong?" | "About 5 minutes a claim, and 2 days to reach the right queue" |
| Success | "What number would make this worth paying for?" | "Most claims routed within an hour at the adjusters' accuracy" |

## Questions for the first ten minutes

Ask in this order. Each answer narrows the next question.

1. Who would use this, and what do they do today without it?
2. What decision does it support, and what happens after the decision?
3. How many times a day or a week does that decision occur?
4. Which systems hold the data, and who owns each one?
5. How would we know in one month that it works?
6. What is not allowed: regulation, privacy, or systems that cannot be changed?
7. Who has to agree before this goes live?

Seven questions at about one minute each leave time to restate the answers before scoping.

## The smallest version that delivers value

A first version should cover part of the problem completely, not all of the problem partly. Three ways to reduce scope work in most cases:

- **Fewer cases.** Handle the two simplest of six categories first.
- **Fewer users.** Start with one team or one office.
- **Less automation.** Suggest a decision to a person before making it automatically.

## A worked example

A regional car insurer receives 1,200 claims a day, and adjusters route each one by hand in about 5 minutes. That is 6,000 minutes, or about 100 adjuster-hours a day. Routing all six queues automatically at once is too large for a first version. A scoped version handles glass and minor damage only, which is about half of all claims, and sends every other claim to an adjuster as before.

If the pilot routes those claims correctly, it removes about half of the 100 hours. The measure is agreement with the adjusters' own choices on a test set of past claims with a known correct queue.

## The one-page scope

State the scope in a fixed order so the interviewer can confirm it in one answer.

| Line | Example |
|---|---|
| User and decision | Adjusters deciding the queue for each new claim |
| In scope | Glass and minor damage claims |
| Out of scope, with a reason | Injury and fraud, because an error costs far more |
| Data needed | The claim form, the photos, and 2,000 past claims with the correct queue |
| Success measure | Agreement with adjusters on at least 97 percent of the test set |
| Timeline | A prototype in three weeks and a pilot in five |

Say the out-of-scope line aloud. Leaving something out is a decision, and the interviewer wants to hear the reason.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-discovery-and-scoping) has six lessons on discovery and scoping, including mapping a customer's data and writing the one-page scope.
- Lesson: [Finding the User and the Decision](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/finding-the-user-and-the-decision?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-discovery-and-scoping), in Grokking the Forward Deployed Engineer Interview
- Lesson: [Questions for the First Ten Minutes](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/questions-for-the-first-ten-minutes?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-discovery-and-scoping), in Grokking the Forward Deployed Engineer Interview
- Lesson: [Writing a One-Page Scope](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/writing-a-one-page-scope?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-discovery-and-scoping), in Grokking the Forward Deployed Engineer Interview
- Next page: [decomposition](decomposition.md), where these steps open the round.
- The same skills in a pre-sales role: [solutions-architect-interview](https://github.com/design-gurus/solutions-architect-interview).
