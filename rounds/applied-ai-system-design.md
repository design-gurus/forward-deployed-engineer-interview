# Applied AI System Design

The FDE design round asks for a system that solves one customer's problem, and at AI companies that system usually contains a language model. The round is less about scale than a classic system design interview. It measures whether the candidate can decide which steps belong to a model, which belong to fixed code, and which belong to a person, and can then show that the result works.

## Rules, models, and people

| Step type | Give it to | Reason |
|---|---|---|
| One correct answer that can be computed | Fixed code | A permission check or a price filter must never be approximate |
| Judgment over unstructured text or images | A model | Reading a claim description, summarizing a contract |
| High cost of error, or low model confidence | A person, with the model's suggestion | Injury claims, possible fraud |

State this division early. It is the sentence interviewers at AI companies are commonly reported to wait for.

## Six steps for the round

| Step | Question to answer |
|---|---|
| 1. Goal | Which user, which decision, and which number defines success? |
| 2. Integrations | Which customer systems hold the data, and how is each one reached? |
| 3. Smallest version | What ships first, and what is left to a person? |
| 4. Guards | What stops a wrong output from reaching the customer? |
| 5. Proof | What test set and measure show that it works? |
| 6. Growth | What changes at ten times the volume, in cost and in latency? |

## Terms to define when using them

- **Retrieval** is finding the right documents for the model to read before it answers.
- **An embedding** is a list of numbers that represents the meaning of a piece of text, so that similar texts can be found quickly.
- **An agent** is a model that chooses and calls tools over several steps.
- **Evaluation** is measuring how often the system's outputs are correct against cases with known answers.
- **A guardrail** is a check in fixed code that blocks or redirects an output.
- **The context window** is the amount of text a model can read at once.

## A worked example with numbers

A customer wants semantic search over 2,000 products. A design that can be defended has four parts: load the products, index an embedding for each one, expose one search endpoint that returns the top 5, and build a test set of 40 questions with a known correct product.

If the correct product is in the top 5 for 34 of the 40 questions, the hit rate is 85 percent. Report the number together with the 6 failures and their causes. When the customer then asks for a price filter, apply it in fixed code before the search.

A second example concerns the context window. Extracting two fields from 400 contracts of about 8,000 tokens each is about 3.2 million tokens, which no single request can hold. The plan processes one contract per step, checks each result in fixed code, and stores results in a table outside the context.

## Questions to expect about agents

| Question | A sound answer includes |
|---|---|
| "What stops the agent from looping forever?" | A step budget, detection of repeated actions, a timeout, and a handoff to a person |
| "Which tools may it call?" | Read-only tools by default, and writes kept as drafts for review |
| "How do you know it is safe to deploy?" | A test set from the customer's real cases, and a pilot on low-risk cases first |
| "What does it cost?" | Requests per day times tokens per request, with the calculation shown |

## Go deeper

- [Grokking the Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-applied-ai-system-design) has seven lessons on applied AI for customers, including guardrails, cost, and compliance for regulated customers.
- [Grokking the AI System Design Interview](https://www.designgurus.io/course/grokking-the-ai-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-applied-ai-system-design) goes deeper on retrieval, agents, and serving.
- [Grokking LLM Evals](https://www.designgurus.io/course/grokking-llm-evals?utm_source=github&utm_medium=repo&utm_campaign=forward-deployed-engineer-interview&utm_content=rounds-applied-ai-system-design) covers building test sets and measuring quality.

The free repository [grokking-ai-system-design](https://github.com/design-gurus/grokking-ai-system-design) indexes the building blocks.
