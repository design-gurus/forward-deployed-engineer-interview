# Forward Deployed Engineer vs Solutions Architect vs Software Engineer

A forward deployed engineer builds a working system for one customer and stays until it runs in production. A solutions architect designs and advises, usually around a sale, and someone else builds. A software engineer builds the product that all customers use. The three roles share technical skills and differ in who they serve, what they deliver, and how they are interviewed.

## The roles compared

| | Forward deployed engineer | Solutions architect | Software engineer |
|---|---|---|---|
| Serves | One customer at a time | Many customers, often before a purchase | All customers, through the product |
| Delivers | Running code in the customer's environment | An architecture, a proof of concept, and advice | Product features |
| Writes production code | Yes, daily | Sometimes, mostly demonstrations | Yes, daily |
| Time with customers | High | High | Low |
| Measured by | A customer result, such as hours saved | Technical success of deals and adoption | Product quality and delivery |
| Typical engagement | Weeks to months on site or embedded | Hours to weeks per account | Continuous work on one codebase |
| Feedback to product | A core duty | Common | Receives it |

Titles vary by company. Some companies use "deployed engineer", "customer engineer", or "solutions engineer" for work that overlaps these roles, so read the job description and not only the title.

## One request, three responses

A regional insurer says: "We bought access to a language model three months ago, and our own demo misrouted one claim in four."

| Role | Response |
|---|---|
| Solutions architect | Reviews the demo, explains why it failed, and presents a reference architecture with a test set and human review. The insurer's team of 4 engineers builds it. |
| Forward deployed engineer | Sits with the adjusters for a week, reads 300 claims, builds a prototype on 2,000 past claims, runs a pilot on two queues, and hands a production system to the insurer's team in week 6. |
| Software engineer | Receives the field report that scanned documents are read poorly and that the API lacks a per-queue confidence threshold, and builds both into the product. |

Each response is correct for its role. The FDE's work also produces the report that the software engineer acts on.

## How the interviews differ

| | FDE loop | Solutions architect loop | Software engineer loop |
|---|---|---|---|
| Signature round | [Decomposition](../rounds/decomposition.md) or a customer case | Architecture design with a customer role-play, often a presentation | Algorithms and system design |
| Coding | Practical and staged | Light or none | Algorithmic |
| Design round | One customer's process and data | Cloud architecture, migration, cost | Scale of a known product |
| Behavioral weight | High, often inside every round | High | Moderate |
| Unusual rounds | Learning, re-engineering, take-home, executive pitch | Presentation to a hiring manager | Few |

## Which role fits

| If you prefer | Consider |
|---|---|
| Building and shipping, with a customer in the room | Forward deployed engineer |
| Designing across many customers, and explaining more than building | Solutions architect |
| Depth in one codebase over years | Software engineer |

Two questions help with the choice. Do you want to write production code every day? Do you want your success to depend on one customer's result? Two yes answers point to the FDE role. A no to the first points to solutions architecture, and a no to the second points to software engineering.

## Answering "Why FDE?" in an interview

Use the comparison directly. A strong answer names what the role offers that the other two do not: owning a customer result from discovery to production. It should include one piece of evidence, such as a project where the candidate worked with users and shipped the system.

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-fde-vs-solutions-architect-vs-software-engineer) opens with a chapter on the role, including a lesson that handles one request three ways.
- Lesson: [Forward Deployed Engineers, Solutions Architects, and Software Engineers](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/forward-deployed-engineers-solutions-architects-and-software-engineers?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-fde-vs-solutions-architect-vs-software-engineer), in Grokking the Forward Deployed Engineer Interview
- Lesson: [What a Forward Deployed Engineer Does](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/what-a-forward-deployed-engineer-does?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-fde-vs-solutions-architect-vs-software-engineer), in Grokking the Forward Deployed Engineer Interview
- Lesson: [Forward Deployed Engineers and Other Applied AI Roles](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/forward-deployed-engineers-and-other-applied-ai-roles?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-fde-vs-solutions-architect-vs-software-engineer), in Grokking the Anthropic Forward Deployed Engineer Interview
- [Grokking the Solutions Architect Interview](https://www.designgurus.io/course/grokking-the-solutions-architect-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-fde-vs-solutions-architect-vs-software-engineer) covers the solutions architect loop.
- Full guide: [Forward deployed engineer vs solutions architect vs software engineer](https://www.designgurus.io/answers/detail/forward-deployed-engineer-vs-solutions-architect-vs-software-engineer-what-is-the-difference?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-fde-vs-solutions-architect-vs-software-engineer)
- Free answer: [Google forward deployed engineer vs. customer engineer](https://www.designgurus.io/answers/detail/google-forward-deployed-engineer-vs-customer-engineer-what-is-the-difference?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=cheat-sheets-fde-vs-solutions-architect-vs-software-engineer), the same comparison inside one company.

The free repository [solutions-architect-interview](https://github.com/design-gurus/solutions-architect-interview) covers that loop round by round.
