# Anthropic interview question bank

This page lists 57 questions in three groups: 25 coding, 14 system design, and 18 behavioral. The reported questions come from candidate accounts, and interviewers are free to choose their own, so use the list as practice material. In the coding and design rounds, the added requirements carry most of the score.

## Coding: reported staged tasks

Each of these 8 tasks is reported to start small and then grow through new requirements. Build the first version, test it, and then extend it.

| # | Task | Related lesson |
|---|---|---|
| 1 | Build the core logic of a banking application with several transaction types, level by level | [Code That Grows With Each Requirement](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/code-that-grows-with-each-requirement?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 2 | Write a function that converts stack trace samples into a call trace | [Exercise: Turning Stack Samples Into Execution Traces](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-turning-stack-samples-into-execution-traces?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 3 | Find and remove duplicate files | [Exercise: Finding Duplicate Files](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-finding-duplicate-files?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 4 | Build an LRU cache, then extend it as constraints change (forward deployed loop) | [Exercise: An LRU Cache That Gains Constraints](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-an-lru-cache-that-gains-constraints?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 5 | Design the core logic behind an API | [How Staged Coding Rounds Work](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/how-staged-coding-rounds-work?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 6 | Parse a data set and reshape it into a new structure | [Cleaning and Joining Messy Data](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/cleaning-and-joining-messy-data?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 7 | Debug code that you did not write | [A Method for Debugging Unfamiliar Code](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/a-method-for-debugging-unfamiliar-code?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 8 | Build a small component with a clean interface, then extend it | [Design Parking System](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/design-parking-system-easy?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |

## Coding: staged practice exercises

These 3 exercises come from Grokking the Anthropic Forward Deployed Engineer Interview. They are practice builds in the same staged format, and the stages are the course's own illustration. A token is the unit of text that a model reads.

| # | Exercise | Lesson |
|---|---|---|
| 9 | Fit instructions, documents, history, and the answer into a fixed token budget | [Exercise: A Token Budget Allocator](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-a-token-budget-allocator?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 10 | Write the loop that runs a model's tool requests until it gives a final answer | [Exercise: A Tool Call Orchestrator](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-a-tool-call-orchestrator?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 11 | Limit the rate of requests sent to a model | [Exercise: A Rate Limiter for Model Requests](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-a-rate-limiter-for-model-requests?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |

## Coding: pattern practice

Sources say that data structure fluency still helps in the staged rounds. These 14 problems cover that base. They are practice problems, not reported Anthropic questions. Problems 18 and 24 are taught in Grokking 75: Top Coding Interview Questions, and the others in Grokking the Coding Interview.

| # | Problem | Pattern |
|---|---|---|
| 12 | [Contains Duplicate](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/contains-duplicate-easy?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Hash set |
| 13 | [Two Sum](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/two-sum-easy?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Hash map |
| 14 | [Group Anagrams](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/group-anagrams-medium?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Hash map |
| 15 | [Encode and Decode Strings](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/encode-and-decode-strings?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | String design |
| 16 | [Valid Parentheses](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/valid-parentheses-easy?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Stack |
| 17 | [Decode String](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/decode-string-medium?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Stack |
| 18 | [Evaluate Reverse Polish Notation](https://www.designgurus.io/course-play/grokking-75-top-coding-interview-questions/doc/evaluate-reverse-polish-notation-medium?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Stack |
| 19 | [Merge Intervals](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/merge-intervals-medium?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Merge intervals |
| 20 | [Maximum CPU Load](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/problem-challenge-2-maximum-cpu-load-hard?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Merge intervals |
| 21 | [My Calendar I](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/my-calendar-i-medium?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Ordered set |
| 22 | [Top K Frequent Numbers](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/top-k-frequent-numbers-medium?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Top K elements |
| 23 | [Topological Sort](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/topological-sort-medium?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Topological sort |
| 24 | [Course Schedule](https://www.designgurus.io/course-play/grokking-75-top-coding-interview-questions/doc/course-schedule-medium?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Topological sort |
| 25 | [Implement Trie (Prefix Tree)](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/implement-trie-prefix-tree-medium-1?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) | Trie |

## System design

Questions 26 to 33 are reported for the software engineer loop. Questions 34 to 37 are reported for Applied AI roles, and 38 and 39 for the forward deployed loop.

| # | Question | Related lesson |
|---|---|---|
| 26 | Design an inference batching system for one GPU that accepts up to 100 inputs per batch | [Serving Optimizations](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/serving-optimizations?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 27 | Extend the batching design to a fleet of GPUs, with failover in the middle of a batch | [Model Serving Basics](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/model-serving-basics?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 28 | Design a token generation service at about 100,000 requests per second | [Back of the Envelope Math for AI Systems](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/back-of-the-envelope-math-for-ai-systems?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 29 | Design distributed search over about 1 billion documents at 1 million queries per second | [Designing Twitter Search](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-twitter-search?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 30 | Design a file cache | [Caching](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/caching?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 31 | Batch queries so that GPUs are used efficiently | [Inference Economics](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/inference-economics?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 32 | Handle a very high volume of requests | [Load Balancing](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/load-balancing?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 33 | Design an agent system that adapts to new tasks | [What an Agent Actually Is](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/what-an-agent-actually-is?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 34 | Design a document assistant over a customer's knowledge base, with permissions that differ by user | [Capstone: Enterprise Document Q&A](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/capstone-enterprise-document-qa?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 35 | Design an agent that resolves support tickets and escalates the cases it should not handle | [Capstone: A Customer-Support Agent](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/capstone-a-customersupport-agent?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 36 | Design an evaluation suite that detects a quality regression before a customer does | [Evaluating LLM Systems](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/evaluating-llm-systems?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 37 | Review an existing customer architecture and state what you would change | [Critiquing a System Design](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/scenario-critique-this-architecture?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 38 | Design an API for sampling from large models, then optimize it for batches | [Designing a High Volume Model Pipeline](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/designing-a-high-volume-model-pipeline?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |
| 39 | Design security for a regulated customer, such as a government contractor | [Security and Data Handling for Regulated Customers](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/security-and-data-handling-for-regulated-customers?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank) |

## Behavioral and values

These 18 questions are reported for the culture and values round, the experiences and goals round, and the forward deployed final panel.

**Mission and motivation**

- 40. Why do you want to work at Anthropic?
- 41. Why Anthropic and not another AI lab?
- 42. What is your view on AI safety, and how does it affect how you build things?
- 43. What worries you most, and excites you most, about AI over the next five years?

**AI risk and critique**

- 44. What are the ethical risks of deploying agentic AI systems?
- 45. How would you keep user data safe inside an AI product?
- 46. Do you have any critique of Anthropic's direction?

**Values under pressure**

- 47. Tell me about a time your values were tested at work.
- 48. Describe a time you were asked to do something you were uncomfortable with.
- 49. Tell me about a time you raised a concern that was unpopular.
- 50. How did you handle pressure from an executive?

**Judgment and disagreement**

- 51. Tell me about a time you balanced speed against reliability or safety.
- 52. Describe a decision you made with incomplete information.
- 53. Tell me about a time you strongly disagreed with a colleague or with leadership.
- 54. Describe a time you changed your mind about something important.

**Ownership and humility**

- 55. Tell me about a serious mistake you made and what you did afterward.
- 56. Describe a time you worked outside your role to finish something important.
- 57. What is the most useful critical feedback you have received?

## Go deeper

- [Grokking the Anthropic Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-anthropic-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank): six staged coding exercises and worked answers for the values questions.
- Lesson: [Values Questions About Customer Work](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/values-questions-about-customer-work?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank), in Grokking the Anthropic Forward Deployed Engineer Interview
- Lesson: [Common Mistakes in Staged Rounds](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/common-mistakes-in-staged-rounds?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank), in Grokking the Anthropic Forward Deployed Engineer Interview
- Lesson: [DSA Patterns Cheat Sheet](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/coding-patterns-a-cheat-sheet?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank), in Grokking the Coding Interview
- Free answer: [Top Anthropic Behavioral Interview Questions (and How to Answer Them)](https://www.designgurus.io/answers/detail/top-anthropic-behavioral-interview-questions-and-how-to-answer-them?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=question-bank)
- Free guide: [Grokking Coding Interview](https://github.com/design-gurus/grokking-coding-interview)
