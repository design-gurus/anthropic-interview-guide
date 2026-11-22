# The Anthropic coding interview

The Anthropic coding rounds are commonly reported as staged builds, not algorithm puzzles. You write a small program that works, and the interviewer or the test platform then adds a requirement that you must fit into your own code. The score depends on whether your design absorbs each change, so clear structure matters more than speed.

## Where coding appears

| Round | Commonly reported format | What is evaluated |
|---|---|---|
| Technical screen | 60 to 90 minutes live in a shared Python environment, or about 90 minutes on CodeSignal | Working code under requirements that grow |
| Take-home, for some roles | A timed exercise done on your own schedule | Realistic engineering judgment |
| Onsite coding | About 60 minutes, live | The same staged pattern, with questions on edge cases, concurrency, and scale |

Candidates report CodeSignal, Colab, and Replit as tools. Some reports describe a shorter live screen of 45 to 60 minutes. Formats vary by team, so confirm yours with the recruiter.

## What the problems look like

Reported problems are close to daily engineering work:

- Build the core business logic of a banking application with several transaction types.
- Write a function that converts stack trace samples into a call trace.
- Find and remove duplicate files.
- Design the core logic behind an API.
- Parse and reshape data, or debug code that you did not write.

Some versions are reported to lock each level until the tests for the previous level pass. In the banking problem, candidates report running out of time more often than being stuck.

## What is graded

| Criterion | What the interviewer looks for |
|---|---|
| Working code first | A simple version that passes before any improvement |
| Structure that absorbs change | The next requirement is an addition, not a rewrite |
| Readability | Small functions and clear names |
| Language fluency | Python syntax and the standard library without lookups |
| Communication | You explain each decision as you make it |

Python is the expected language. Anthropic's careers page is reported to allow reference materials during technical assessments. It also expects you to know basic syntax and standard libraries. Treat that as permission to check one method signature, not as time to learn the language.

Live rounds are reported to run without AI tools unless the interviewer says otherwise. See [Interview process](interview-process.md) for the rule at each stage.

## How to practice

1. Choose a small build, such as a ledger or a cache, and finish a version that passes its tests.
2. Add one new requirement and change your own code without starting again. Repeat this three times.
3. Set a timer for 90 minutes and practice in Python only.
4. After each session, count the lines you rewrote. The number should fall from week to week.

An LRU cache is a good first build. It keeps the most recently used items and removes the least recently used item when it is full. The lesson [Exercise: An LRU Cache That Gains Constraints](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-an-lru-cache-that-gains-constraints?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=coding-interview) runs this build in stages.

Sources say that data structure fluency still helps, although pattern recognition is not what is scored. Keep a base in hash maps, stacks, intervals, and graphs. A hash map is a table that finds a value by its key in constant time. The [Question bank](question-bank.md) lists 14 pattern problems for this base.

For a take-home, treat the stated time limit as real. Sources report that submitting far more than was requested is not rewarded. Add a short note on what you would do with more time.

## Go deeper

- [Grokking the Coding Interview](https://www.designgurus.io/course/grokking-the-coding-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=coding-interview): the coding patterns that the staged builds assume.
- Lesson: [How Staged Coding Rounds Work](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/how-staged-coding-rounds-work?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=coding-interview), in Grokking the Anthropic Forward Deployed Engineer Interview
- Lesson: [Exercise: Finding Duplicate Files](https://www.designgurus.io/course-play/grokking-the-anthropic-forward-deployed-engineer-interview/doc/exercise-finding-duplicate-files?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=coding-interview), in Grokking the Anthropic Forward Deployed Engineer Interview
- Lesson: [Code That Grows With Each Requirement](https://www.designgurus.io/course-play/grokking-the-forward-deployed-engineer-interview/doc/code-that-grows-with-each-requirement?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=coding-interview), in Grokking the Forward Deployed Engineer Interview
- Lesson: [Introduction to Hash Map Pattern](https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-hash-map-pattern?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=coding-interview), in Grokking the Coding Interview
- Free answer: [Does Anthropic Use CodeSignal in Interviews?](https://www.designgurus.io/answers/detail/does-anthropic-use-codesignal-in-interviews?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=coding-interview)
