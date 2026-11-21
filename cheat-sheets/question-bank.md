# Forward Deployed Engineer Interview Question Bank

This page lists 52 questions grouped by round. Some are commonly reported by candidates, and the rest are written in the same style for practice. Each group starts with one line on what the interviewer is measuring. Answer them aloud with a timer, because every FDE round is a spoken one.

## Motivation and the recruiter screen

Measured: a specific reason for customer work, and evidence of hands-on building.

1. Why forward deployed work and not a product engineering team?
2. Why this company?
3. What have you built with language models, and how did you measure it?
4. Describe a time you worked directly with a customer or an internal user.
5. How do you feel about travel and time at a customer site?
6. Which of our products do you use, and what would you change in it?

## Decomposition and customer cases

Measured: questions, a named user, data reasoning, and a first version buildable in weeks. See [decomposition](../rounds/decomposition.md).

7. Design a system to improve traffic in a large city.
8. Design a sync between two employee record systems.
9. Let several teams query a shared dataset without seeing the raw records.
10. Design an app to catalog species while exploring an unfamiliar environment.
11. A hospital believes it is losing money to billing errors. Where do you start?
12. A warehouse runs out of its 50 best-selling items every week. What do you build?
13. A support team answers the same 30 questions every day. What would you propose?
14. The customer has just said that half of the data you planned to use does not exist. What changes?

## Discovery and scoping

Measured: finding the decision behind the request, and choosing what to leave out. See [discovery and scoping](../rounds/discovery-and-scoping.md).

15. What are the first five questions you ask a new customer?
16. How do you define success before building anything?
17. The customer asks for everything in the first version. What do you say?
18. How do you find out what data a customer actually has?
19. Who needs to agree before a system goes live, and how do you find them?

## Learning and re-engineering

Measured: method with unfamiliar code. See [the learning round](../rounds/learning-round.md) and [the re-engineering round](../rounds/re-engineering-round.md).

20. Here is a library and its documentation. Add a filter by date to this service.
21. This report shows 5 percent more claims than the source system. Find out why.
22. This function is correct on the first call and wrong on the second. Fix it.
23. Describe your first hour in a codebase that nobody can explain to you.
24. Tell me about a tool or system you had to learn in under a week.

## Practical coding

Measured: working code for real data, and a design that survives new stages. See [practical coding](../rounds/practical-coding.md).

25. Fetch every page of results from this REST API and handle failures.
26. Reconcile two exports whose customer names are spelled differently.
27. Write a SQL query for the number of orders per customer, including customers with none.
28. Build a credit system with add and spend. Now add expiry dates. Now spend the credits that expire first.
29. Implement an LRU cache. Now give each item a size and limit the total size.
30. Parse this messy export and reconcile it against a second source. Now handle a burst of input.
31. The coding assistant wrote this function. Explain its running time and improve it.

## Applied AI system design

Measured: the division between models, fixed code, and people, with proof that it works. See [applied AI system design](../rounds/applied-ai-system-design.md).

32. Design retrieval over a customer's private knowledge base.
33. Design an assistant that extracts two fields from 400 long contracts.
34. Which steps in your design should never be given to a model?
35. What stops your agent from looping without finishing?
36. How would you show a customer that the system is accurate enough to deploy?
37. What does one request cost, and what changes at ten times the volume?
38. Design security for a deployment at a regulated customer.
39. When is a model the wrong tool?

## Take-home and project deep dive

Measured: ownership, reasons, and limits. See [the take-home project](../rounds/take-home-project.md) and [the project deep dive](../rounds/project-deep-dive.md).

40. Present your take-home in three minutes for a customer.
41. Which of your failed test cases concerns you most?
42. How would the system change if the customer's needs shifted?
43. What did you personally own in this project?
44. Which part would fail first at ten times the load?
45. What would you do differently with the same time?

## Behavioral and values

Measured: trust, judgment, and honesty. See [behavioral questions for customer work](../rounds/behavioral-for-customer-work.md).

46. Tell me about a stakeholder who disagreed with your plan.
47. Describe a time you said no to a customer or a manager.
48. Tell me about something you shipped that broke in production.
49. When did feedback from a customer change what a product team built?
50. Tell me about a time you were wrong.
51. Describe pressure from a senior person to do something you thought was a mistake.
52. Where do you disagree with us?

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-question-bank) answers these question types with weak and strong examples and has a question bank for every chapter.
- [Grokking Modern Behavioral Interview](https://www.designgurus.io/course/grokking-behavioral-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-question-bank) covers the behavioral families in full.
- Free answer: [What is the forward deployed engineer interview process like, round by round?](https://www.designgurus.io/answers/detail/what-is-the-forward-deployed-engineer-interview-process-like-round-by-round?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-question-bank), where each question family appears in the loop.
