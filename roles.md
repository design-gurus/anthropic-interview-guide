# How the Anthropic loop differs by role

Anthropic posts no job titled "AI Engineer". The work people mean by that phrase is divided among several real titles, and the loops differ. Every reported loop keeps the staged coding round and the values round. The Applied AI and forward deployed loops add rounds on building with Claude for a customer.

## The titles

| What you want to do | Anthropic title | What the work is |
|---|---|---|
| Build products on Claude with customers | Applied AI Engineer | Technical advisor working inside a customer's engineering team |
| The same work with more architecture ownership | Applied AI Architect | Architecture decisions across larger enterprise deployments |
| The same work, placed with one customer | Forward Deployed Engineer | Long engagements inside one customer organization |
| Train and improve the models | Research Engineer | Reinforcement learning, pretraining, interpretability, and computer use |
| Serve the models at high volume | Software Engineer, Infrastructure | Inference performance, reliability, and the platform under the API |

The standard software engineer loop is described in [Interview process](interview-process.md).

## Applied AI Engineer

Candidates report about seven rounds over three to six weeks, run remotely.

| Stage | Reported format |
|---|---|
| Recruiter screen | About 30 minutes |
| Technical screen | 90 minutes on CodeSignal, or 60 minutes live |
| Hiring manager | 45 to 60 minutes |
| System design | About 60 minutes on the architecture of an application built on a large language model (LLM) |
| Second technical round | About 60 minutes, often LLM implementation |
| Values round | About 60 minutes |
| Experiences and goals | About 60 minutes |

The postings ask for production experience with LLMs. They name advanced prompt engineering, agent development, evaluation frameworks, and strong Python. Listed deliverables include evaluation suites, sub-agents, and servers for the Model Context Protocol (MCP). MCP is an open standard for connecting a model to outside tools and data.

Reported design questions include a document assistant with permissions that differ by user, and a support agent that escalates the cases it should not handle. The graded skill is locating the failure. A wrong answer can come from the retrieval step, the instructions given to the model, or the model itself. Retrieval means finding the right documents for the model to read.

## Forward Deployed Engineer

Preparation guides describe six stages over four to six weeks. Anthropic publishes no official loop for this role, and the order is reported to vary by team.

| Stage | What is evaluated |
|---|---|
| Recruiter screen | Motivation, product use, level, and references |
| Technical use-case screen | Planning a long-running task with MCP and managing context |
| Staged coding round | Code that adapts as each stage adds a requirement |
| Hiring manager round | One past project, and when a model is the wrong tool |
| Solution design | Architecture for a customer, with security and failure modes |
| Final panel | Behavior and values |

The context window is the amount of text a model can read at once. In the use-case screen, interviewers are reported to watch how you manage it across many steps. References may be requested early, often a former manager and a close coworker. The final panel is reported as the hardest stage, and nontechnical interviewers often run it.

## Research Engineer and infrastructure roles

Sources say only that Research Engineer is a different interview with a machine learning bar.

For Software Engineer roles in infrastructure, the serving questions in [System design interview](system-design-interview.md) are reported more often than application design. Those questions cover batching, GPU utilization, and failover.

## Go deeper

- [Grokking the Anthropic Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-anthropic-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=roles): each stage of the forward deployed loop, with the Claude platform and two mock loops.
- Lesson: [Forward Deployed Engineers and Other Applied AI Roles](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/forward-deployed-engineers-and-other-applied-ai-roles?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=roles), in Grokking the Anthropic Forward Deployed Engineer Interview
- Lesson: [The Two Reported Loop Shapes](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/the-two-reported-loop-shapes?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=roles), in Grokking the Anthropic Forward Deployed Engineer Interview
- Lesson: [What the Use Case Screen Tests](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/what-the-use-case-screen-tests?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=roles), in Grokking the Anthropic Forward Deployed Engineer Interview
- Free article: [Anthropic AI Engineer Interview: Rounds, Questions, and How to Prepare](https://www.designgurus.io/blog/anthropic-ai-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=roles)
- Free guide: [Anthropic forward deployed engineer interview](https://github.com/design-gurus/forward-deployed-engineer-interview/blob/main/companies/anthropic.md), in Forward Deployed Engineer Interview
