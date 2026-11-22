# Anthropic Interview Guide

> A free guide to the Anthropic software engineer interview from [DesignGurus.io](https://www.designgurus.io/course/grokking-the-ai-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme), created by Arslan Ahmad.

[![GitHub stars](https://img.shields.io/github/stars/design-gurus/anthropic-interview-guide?style=social)](https://github.com/design-gurus/anthropic-interview-guide/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/design-gurus/anthropic-interview-guide)](https://github.com/design-gurus/anthropic-interview-guide/commits/main)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

The Anthropic software engineer interview differs from a standard large-company loop in four ways. A written "Why Anthropic?" answer is read before any interview is scheduled. The coding rounds are commonly reported as staged builds: you write a small working program, and each new level adds a requirement. System design, the round where you design a large software system aloud, is framed around serving AI models on graphics processors (GPUs). The culture and values round is the stage where candidates most often report being rejected.

This repository is a short, free guide to that loop. It covers each stage, the questions candidates report, and a four-week preparation plan. Each page takes about three minutes to read. This guide is independent. It is not affiliated with, endorsed by, or reviewed by Anthropic, and every process detail is a candidate report, not an official statement.

## The loop at a glance

Candidates commonly report seven to nine rounds, with two onsite loops on separate days. Not every candidate sees every stage.

| Stage | Length | What it measures | Guide |
|---|---|---|---|
| Written application | 200 to 400 words | Specific, personal motivation | [Behavioral interview](behavioral-interview.md) |
| Recruiter screen | About 30 minutes | Background, role fit, and "Why Anthropic?" | [Interview process](interview-process.md) |
| Technical screen | 60 to 90 minutes | Working code that absorbs new requirements | [Coding interview](coding-interview.md) |
| Hiring manager conversation | 45 to 60 minutes | Engineering judgment and depth of involvement | [Interview process](interview-process.md) |
| First onsite loop | 2 or 3 interviews of about 60 minutes | System design, coding, and culture and values | [System design interview](system-design-interview.md) |
| Second onsite loop | 2 or 3 interviews of about 60 minutes | Experiences and goals, and a technical project review | [Behavioral interview](behavioral-interview.md) |
| References and team matching | Calls | Fit with one team | [Interview process](interview-process.md) |

## Start here

| Your situation | Read this first |
|---|---|
| You have not submitted the application yet | [Behavioral interview](behavioral-interview.md), for the written "Why Anthropic?" answer |
| You have a recruiter call scheduled and need the outline | [Interview process](interview-process.md) |
| You are applying for an Applied AI or forward deployed role | [Roles](roles.md) |
| You have four weeks before the onsite loops | [Four-week plan](four-week-plan.md) |

## All pages

| Page | What it covers |
|---|---|
| [Interview process](interview-process.md) | Every stage from application to offer, and what each stage decides |
| [Coding interview](coding-interview.md) | The staged coding format, what is graded, and how to practice it |
| [System design interview](system-design-interview.md) | Reported questions, the inference batching problem, and what a strong answer includes |
| [Behavioral interview](behavioral-interview.md) | The values round, the "Why Anthropic?" answer, and how to prepare stories |
| [Levels and seniority](levels.md) | What the sources say about seniority, new graduates, and how the loop changes |
| [Roles](roles.md) | The real job titles, and how the loop differs for Applied AI and forward deployed roles |
| [Question bank](question-bank.md) | 57 questions grouped as coding, system design, and behavioral |
| [Four-week plan](four-week-plan.md) | A weekly plan with a finish condition for each week |
| [Common mistakes](common-mistakes.md) | Ten mistakes that are specific to this loop |

## How many rounds are in an Anthropic interview?

Candidates commonly report seven to nine rounds. The usual order is a recruiter screen, a technical screen, a hiring manager conversation, and two onsite loops of two or three interviews each. The second onsite loop is reported to be scheduled only if the first one goes well. See [Interview process](interview-process.md).

## How hard is the Anthropic interview?

Candidates describe two separate difficulties. The staged coding screen is timed, and candidates report running out of time more often than being stuck. The culture and values round is the most commonly reported reason for rejection, including for engineers who passed every technical round. See [Common mistakes](common-mistakes.md).

## How long does the Anthropic hiring process take?

Reported timelines range from about three weeks to a few months. Team matching is the stage where candidates report waits of several weeks. Anthropic is reported to send rejection emails at every stage and to give no interview feedback. See [Interview process](interview-process.md).

## What coding questions does Anthropic ask?

Most reported questions are practical builds, not algorithm puzzles. Examples include the core logic of a banking application, a function that converts stack samples into a call trace, and a tool that finds duplicate files. Python is the expected language. See [Coding interview](coding-interview.md) and [Question bank](question-bank.md).

## Does Anthropic ask system design?

Yes. The most frequently reported question is an inference batching system for one GPU that accepts up to 100 inputs per batch. You do not need to explain how the model works inside. The graded skills are queuing, batching, routing, and failure handling. See [System design interview](system-design-interview.md).

## Can you use Claude during the Anthropic interview process?

In some stages. Anthropic's published candidate guidance is reported to allow Claude for refining the written application and for preparation. It is reported as not allowed in take-home assessments or live interviews unless the instructions say otherwise. Confirm the current rule with your recruiter. See [Interview process](interview-process.md).

## Course lessons to start with

- [The Anthropic Loop](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/the-anthropic-loop?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): the reported stages in one lesson, in Grokking the Forward Deployed Engineer Interview
- [How Staged Coding Rounds Work](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/how-staged-coding-rounds-work?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): how each stage adds a requirement to working code, in Grokking the Anthropic Forward Deployed Engineer Interview
- [Exercise: Turning Stack Samples Into Execution Traces](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-turning-stack-samples-into-execution-traces?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): a runnable version of a reported coding task, in Grokking the Anthropic Forward Deployed Engineer Interview
- [Serving Optimizations](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/serving-optimizations?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): batching and the other methods that raise GPU throughput, in Grokking the AI System Design Interview
- [Back of the Envelope Math for AI Systems](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/back-of-the-envelope-math-for-ai-systems?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): throughput and cost estimates for model serving, in Grokking the AI System Design Interview
- [Anthropic's Published Positions on AI Safety](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/anthropics-published-positions-on-ai-safety?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): what to read before the values round, in Grokking the Anthropic Forward Deployed Engineer Interview
- [Forming Your Own View, Including Disagreement](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/forming-your-own-view-including-disagreement?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): how to hold a reasoned position under follow-up questions, in Grokking the Anthropic Forward Deployed Engineer Interview
- [Why Anthropic: Answers That Are Not Generic](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/why-anthropic-answers-that-are-not-generic?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): the written and spoken motivation answer, in Grokking the Anthropic Forward Deployed Engineer Interview
- [Discussing Your Own Mistakes](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/discussing-your-own-mistakes?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): how to describe a real failure and what changed, in Grokking Staff Engineer Interview

## Free reading on DesignGurus.io

- Free article: [Anthropic Interview Process: Rounds, Questions, and How to Prepare](https://www.designgurus.io/blog/anthropic-interview-process?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free article: [Anthropic AI Engineer Interview: Rounds, Questions, and How to Prepare](https://www.designgurus.io/blog/anthropic-ai-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free answer: [What Is the Anthropic Interview Process Like? (Round by Round)](https://www.designgurus.io/answers/detail/what-is-the-anthropic-interview-process-like-round-by-round?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free answer: [What to Expect in the Anthropic System Design Interview](https://www.designgurus.io/answers/detail/what-to-expect-in-the-anthropic-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free answer: [Top Anthropic Behavioral Interview Questions (and How to Answer Them)](https://www.designgurus.io/answers/detail/top-anthropic-behavioral-interview-questions-and-how-to-answer-them?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free answer: [How to Answer the "Why Anthropic?" Application Question](https://www.designgurus.io/answers/detail/how-to-answer-why-anthropic?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free answer: [Does Anthropic Use CodeSignal in Interviews?](https://www.designgurus.io/answers/detail/does-anthropic-use-codesignal-in-interviews?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free answer: [What Is the Anthropic Forward Deployed Engineer Interview Like? (Round by Round)](https://www.designgurus.io/answers/detail/what-is-the-anthropic-forward-deployed-engineer-interview-like-round-by-round?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free answer: [Does Anthropic Hire New Grads?](https://www.designgurus.io/answers/detail/does-anthropic-hire-new-grads?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)
- Free answer: [Anthropic Company Culture, Mission, and Values](https://www.designgurus.io/answers/detail/what-is-the-culture-of-the-anthropic-company?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme)

## Go deeper

This repository gives the outline. The courses below teach each round in full.

- [Grokking the AI System Design Interview](https://www.designgurus.io/course/grokking-the-ai-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): model serving, retrieval, and agents, which match the design questions reported here.
- [Grokking the Anthropic Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-anthropic-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): the full course for the forward deployed loop, with staged coding exercises and a chapter on the values round.
- [Grokking the Coding Interview](https://www.designgurus.io/course/grokking-the-coding-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): the coding patterns that the staged builds assume you already know.
- [Grokking the System Design Interview](https://www.designgurus.io/course/grokking-the-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): the core method and the building blocks, including caching and load balancing.
- [Grokking Modern Behavioral Interview](https://www.designgurus.io/course/grokking-behavioral-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=readme): the STAR method and a story bank for the behavioral conversations.

Related free guides: [Anthropic system design interview](https://github.com/design-gurus/grokking-system-design/blob/main/companies/anthropic.md), [Anthropic forward deployed engineer interview](https://github.com/design-gurus/forward-deployed-engineer-interview/blob/main/companies/anthropic.md), [OpenAI Interview Guide](https://github.com/design-gurus/openai-interview-guide), [Grokking AI System Design](https://github.com/design-gurus/grokking-ai-system-design), and [Grokking Coding Interview](https://github.com/design-gurus/grokking-coding-interview).

For the system design round, see [Grokking System Design](https://github.com/design-gurus/grokking-system-design), the free companion guide to patterns, question walkthroughs, and cheat sheets.

## More free guides

Every guide below is free, follows the same short-page format, and comes from DesignGurus.io.

- **Core guides:** [Grokking System Design](https://github.com/design-gurus/grokking-system-design), [Grokking Coding Interview](https://github.com/design-gurus/grokking-coding-interview), [Grokking AI System Design](https://github.com/design-gurus/grokking-ai-system-design), [Design Patterns](https://github.com/design-gurus/design-patterns), [Best System Design Resources](https://github.com/design-gurus/best-system-design-resources), [Best System Design Courses](https://github.com/design-gurus/best-system-design-courses)
- **By interview round:** [System Design Numbers](https://github.com/design-gurus/system-design-numbers), [API Design Interview](https://github.com/design-gurus/api-design-interview), [Frontend System Design Interview](https://github.com/design-gurus/frontend-system-design-interview), [Mobile System Design Interview](https://github.com/design-gurus/mobile-system-design-interview), [Microservices Interview Questions](https://github.com/design-gurus/microservices-interview-questions), [Concurrency Interview](https://github.com/design-gurus/concurrency-interview)
- **By role:** [DevOps and SRE Interview](https://github.com/design-gurus/devops-sre-interview), [Data Engineering Interview](https://github.com/design-gurus/data-engineering-interview), [Forward Deployed Engineer Interview](https://github.com/design-gurus/forward-deployed-engineer-interview), [Solutions Architect Interview](https://github.com/design-gurus/solutions-architect-interview)
- **Seniority and behavioral:** [Staff Engineer Interview](https://github.com/design-gurus/staff-engineer-interview), [Engineering Manager Interview](https://github.com/design-gurus/engineering-manager-interview), [Amazon Leadership Principles](https://github.com/design-gurus/amazon-leadership-principles), [Software Engineer Levels](https://github.com/design-gurus/software-engineer-levels)
- **By company:** [Google Interview Guide](https://github.com/design-gurus/google-interview-guide), [Meta Interview Guide](https://github.com/design-gurus/meta-interview-guide), [Amazon Interview Guide](https://github.com/design-gurus/amazon-interview-guide), [Microsoft Interview Guide](https://github.com/design-gurus/microsoft-interview-guide), [Apple Interview Guide](https://github.com/design-gurus/apple-interview-guide), [Netflix Interview Guide](https://github.com/design-gurus/netflix-interview-guide), [OpenAI Interview Guide](https://github.com/design-gurus/openai-interview-guide)

## Contributing

Corrections, new questions, and reports of how an Anthropic loop was run are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

## License

The content is licensed under [CC BY 4.0](LICENSE). See [NOTICE.md](NOTICE.md) for what the license covers and how to attribute.
