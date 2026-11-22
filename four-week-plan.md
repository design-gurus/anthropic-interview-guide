# A four-week plan for the Anthropic interview

This plan prepares you for the Anthropic software engineer loop in four weeks and assumes about 10 hours of study per week. It gives the first week to the written answer and staged coding, the second to system design, the third to values and the project review, and the fourth to full practice runs. Each week ends with a finish condition that you can check.

## The plan at a glance

| Week | Focus | Hours | Finish condition |
|---|---|---|---|
| 1 | Written answer and staged coding | 10 | A 300-word answer, and one build extended 3 times inside 90 minutes |
| 2 | System design for model serving | 10 | The batching design explained aloud in 20 minutes, including one GPU failure |
| 3 | Values stories and the project review | 10 | 6 written stories, one stated disagreement, and a 2-page project document |
| 4 | Timed practice runs | 10 | 2 coding runs, 1 design run, and 1 values conversation completed |

## Week 1: the written answer and staged coding

Write the "Why Anthropic?" answer first, because it is read before any interview. Name one specific thing you have read or used. Connect it to your work, and state the skill you would contribute. Then practice saying it aloud in 90 seconds.

For coding, complete three staged builds in Python:

- An LRU cache, with [Exercise: An LRU Cache That Gains Constraints](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-an-lru-cache-that-gains-constraints?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=four-week-plan).
- A duplicate file finder, with [Exercise: Finding Duplicate Files](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-finding-duplicate-files?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=four-week-plan).
- A small ledger with deposits, withdrawals, and transfers, which you extend three times.

**Finish condition:** the written answer is 200 to 400 words, and you extended one build three times inside 90 minutes without starting again.

## Week 2: system design for model serving

Study the building blocks first: queues, batching, caching, load balancing, and failover. Then work through the four reported questions in [System design interview](system-design-interview.md). For each one, state the requirements in numbers before you draw anything.

Practice the single-GPU batching question until it is fluent. Then remove a GPU in the middle of a batch and repair your design.

**Finish condition:** you can explain the batching design aloud in 20 minutes, with the batch timeout, the queue limit, and the failure path.

## Week 3: values and the project review

Read Anthropic's published views on AI safety and its Responsible Scaling Policy. Write down one point where you disagree and the evidence that would change your mind.

Write six stories from your own work. Include a disagreement, a mistake you owned, and a time you chose care over speed. For each one, add what you got wrong.

Choose one project in which you made the decisions. Write two pages on what you chose, what you rejected, what broke, and what the numbers were.

**Finish condition:** six stories, one disagreement, and the project document all exist in writing.

## Week 4: timed practice runs

Run each round under interview conditions, with another person where possible.

- Two coding runs of 90 minutes, with a new requirement every 20 minutes.
- One design run of 60 minutes on a question you have not seen.
- One values conversation of 60 minutes, in which the other person challenges each answer twice.

After each run, write down where you lost time. Repeat only the weakest round.

**Finish condition:** all four runs are complete, and you have repeated the weakest one.

## Additions for Applied AI and forward deployed roles

- Build one small application on the Claude API with retrieval, one tool call, and a written evaluation set.
- Extend it into an agent with two or three tools, and write an MCP server for one of them.
- Practice the design questions for these roles in [Question bank](question-bank.md), ending each with how you would evaluate the system.

Sources suggest five weeks for the Applied AI loop when you add this work.

## Go deeper

- [Grokking the Anthropic Forward Deployed Engineer Interview](https://www.designgurus.io/course/grokking-the-anthropic-forward-deployed-engineer-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=four-week-plan): staged exercises, the values chapter, and two mock loops.
- Lesson: [A Thirty Day Study Plan](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/a-thirty-day-study-plan?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=four-week-plan), in Grokking the Anthropic Forward Deployed Engineer Interview
- Lesson: [A Framework for AI Design Answers](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/a-framework-for-ai-design-answers?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=four-week-plan), in Grokking the AI System Design Interview
- Lesson: [System Design Interviews: A Step by Step Guide](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/system-design-interviews-a-step-by-step-guide?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=four-week-plan), in Grokking the System Design Interview
- Lesson: [Context, Constraints, Choices, Results](https://www.designgurus.io/course-play/grokking-staff-engineer-interview/doc/context-constraints-choices-results?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=four-week-plan), in Grokking Staff Engineer Interview
- Free answer: [How to Answer the "Why Anthropic?" Application Question](https://www.designgurus.io/answers/detail/how-to-answer-why-anthropic?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=four-week-plan)
