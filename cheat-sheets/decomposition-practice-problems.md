# Decomposition Practice Problems

This page gives 14 problem statements for timed practice, each with the first two clarifying questions a strong candidate would ask. It contains no full solutions. The value of the exercise is in asking, scoping, and breaking the problem down aloud for 60 minutes, as described in [decomposition](../rounds/decomposition.md).

## How to use this page

1. Choose one problem and set a timer for 60 minutes.
2. Ask a friend to play the customer and to invent answers to your questions.
3. Spend the first 12 minutes on questions only.
4. Have the friend change one constraint at about minute 35.
5. Afterward, check the answer against the five criteria at the end of this page.

Without a partner, write your questions, invent two different answers to each, and plan for both.

## The problems

The pattern column names the shape of the problem. Recognizing the shape gives the first breakdown.

| # | Problem statement | Pattern | First two clarifying questions |
|---|---|---|---|
| 1 | "Improve traffic in our city." | Monitoring and alerts | Who would act on the output, and what can they change? What data exists per intersection today? |
| 2 | "Keep our two employee record systems in sync." | Syncing two systems of record | Which system is correct when they disagree? How often does each one change, and who changes it? |
| 3 | "Let five research teams use one dataset without seeing the raw records." | Sharing data without exposing records | What questions do the teams need to ask of the data? Which fields identify a person? |
| 4 | "We think we are losing money to hospital billing errors." | Automating a review queue | Who reviews bills today, and how many per day? Is there a set of past bills with known errors? |
| 5 | "Our warehouse keeps running out of popular items." | Pipeline with a decision screen | Who decides when to reorder, and how often? How current is the stock count? |
| 6 | "Inspectors in the field record findings on paper." | Pipeline with a decision screen | What happens to a finding after it is recorded? Do inspectors have a network connection on site? |
| 7 | "Customers wait too long for support answers." | Assistant over documents | What share of tickets repeat a known question? Where are the correct answers written down? |
| 8 | "Our lawyers spend days reviewing supplier contracts." | Assistant over documents | Which clauses do they look for, and what do they do on finding one? How many contracts per month, and how long is each? |
| 9 | "Trucks in our fleet break down without warning." | Monitoring and alerts | What does the mechanic need to know, and how early? Which vehicles report sensor data? |
| 10 | "School bus routes take too long." | Forecasting and planning | Who sets routes, and how often do they change? What limits apply, such as ride time or bus capacity? |
| 11 | "Tell building managers when energy use is abnormal." | Monitoring and alerts | What would a manager do after an alert? How many false alerts per week are acceptable? |
| 12 | "Reviewing grant applications takes our staff three months." | Automating a review queue | What are the review criteria, and are they written down? Which decisions must remain with a person? |
| 13 | "Route incoming insurance claims to the right team." | Automating a review queue | How many claims arrive per day, and how many queues exist? Are there past claims with a known correct queue? |
| 14 | "Catalog species while exploring an unfamiliar environment." | Pipeline with a decision screen | Who uses the catalog afterward, and for what decision? Is there a network connection in the field? |

## Constraint changes to try

Have the customer introduce one of these at minute 35:

- "We only have that data for a third of the sites."
- "The regulator requires a record of every automated decision."
- "The team that owns that system will not give us write access."
- "We need something visible in two weeks, not eight."

Change the plan, and state what the change costs. Defending the earlier plan loses the iteration criterion.

## Check the answer

| Criterion | Evidence in a strong answer |
|---|---|
| Structured breakdown | Four to six named parts, each with an input and an output |
| A named user | One role and one decision, stated in the first 15 minutes |
| Data reasoning | What exists, who owns it, and how complete it is |
| A first version in weeks | A part of the problem handled completely, with one measure |
| Iteration | A stated next version, and a changed plan after the new constraint |

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-decomposition-practice-problems) works twelve problems of this kind in full, each with a weak and a strong answer, after teaching the seven patterns.
- Lesson: [How to Use the Problem Bank](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/how-to-use-the-problem-bank?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-decomposition-practice-problems), in Grokking the Forward Deployed Engineer Interview
- Lesson: [Reducing Hospital Billing Errors](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/reducing-hospital-billing-errors?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-decomposition-practice-problems), in Grokking the Forward Deployed Engineer Interview
- Lesson: [Preventing Warehouse Stockouts](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/preventing-warehouse-stockouts?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-decomposition-practice-problems), in Grokking the Forward Deployed Engineer Interview
- Full guide: [What is the Palantir decomposition interview, and how does the round work?](https://www.designgurus.io/answers/detail/what-is-the-palantir-decomposition-interview-how-the-fde-round-works?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-decomposition-practice-problems)
