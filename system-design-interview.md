# The Anthropic system design interview

The Anthropic system design round is commonly reported as a 60-minute interview in the first onsite loop. The questions are framed around AI infrastructure, such as GPU clusters and model serving, but the graded skills are classic distributed systems. You do not need to explain how the model works inside. Your task is to design the system around it.

## Three traits of the round

| Trait | What it means for you |
|---|---|
| AI framing, infrastructure core | You need queues, batching, routing, and failure handling, not machine learning theory |
| Novel, open problems | Questions are reported to be close to what Anthropic teams are working on, and the interviewer may have no single correct answer |
| Extra weight on reliability | Reasoning about what breaks and how the system degrades earns more than an unusual architecture |

## Commonly reported questions

| Question | Reported numbers | Related lesson |
|---|---|---|
| Design an inference batching system for one GPU, where users wait for the result | Up to 100 inputs per batch | [Serving Optimizations](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/serving-optimizations?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview) |
| Extend that design to a fleet of GPUs | Routing, capacity tracking, and failover in the middle of a batch | [Model Serving Basics](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/model-serving-basics?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview) |
| Design a token generation service for a large language model | About 100,000 requests per second | [Back of the Envelope Math for AI Systems](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/back-of-the-envelope-math-for-ai-systems?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview) |
| Design a distributed search system | About 1 billion documents and 1 million queries per second | [Designing Twitter Search](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/designing-twitter-search?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview) |

Inference means running a trained model to produce an output. Other reported questions include a file cache and an agent system that adapts to new tasks. The single-GPU batching question is the most frequently reported.

## What a strong answer includes

The batching question shows the expected structure.

1. **Requirements.** Ask for the latency of one batch, the target latency at the 99th percentile (p99), and the request rate. Ask whether batch latency stays about constant as the batch fills.
2. **Core design.** A front-end service gives each request an ID and places it in a queue with its response channel. A dispatcher forms a batch when 100 inputs are waiting or when a timeout of 10 to 50 milliseconds expires.
3. **The trade-off.** The timeout limits the added delay at low traffic and keeps throughput at high traffic. Throughput is the number of requests completed per second.
4. **Failure handling.** State what happens when the GPU fails during a batch. Requests are retried, which requires idempotency, or they fail fast with a clear error. Idempotency means a repeated request has the same effect as one request.
5. **Overload.** Limit the queue length and apply backpressure, which means rejecting new work when the queue is full.
6. **Metrics.** Name queue depth, batch fill ratio, GPU utilization, and median and p99 latency.

For the fleet version, add a routing layer that tracks each worker through heartbeats and counts of requests in progress. A heartbeat is a periodic signal that shows a server is alive. Route each batch to the healthy worker with the lowest load.

## What is graded

- **Requirements discipline.** You obtain numbers before you draw components, and you calculate throughput aloud.
- **Trade-off reasoning.** Each choice comes with the alternative you rejected.
- **Failure thinking.** You raise crashes, overload, and partial failure before the interviewer asks.
- **Comfort with ambiguity.** You state assumptions and revise the design when a constraint is added.
- **Communication.** The interviewer always knows which part of the design you are discussing.

Sources also report that awareness of safety and security implications is graded.

## What the products imply

Anthropic serves Claude through an API at high volume. The topics that follow from this are batching, caching, GPU utilization, streaming output, and cost per request. Applied AI and forward deployed loops use a different design round, built on a customer's Claude deployment. See [Roles](roles.md).

## Go deeper

- [Grokking the AI System Design Interview](https://www.designgurus.io/course/grokking-the-ai-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview): model serving, inference cost, retrieval, and agents.
- Lesson: [Inference Economics](https://www.designgurus.io/course-play/grokking-the-ai-system-design-interview/doc/inference-economics?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview), in Grokking the AI System Design Interview
- Lesson: [Latency vs Throughput](https://www.designgurus.io/course-play/grokking-the-system-design-interview/doc/latency-vs-throughput?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview), in Grokking the System Design Interview
- Lesson: [Introduction to Messaging System](https://www.designgurus.io/course-play/grokking-system-design-fundamentals/doc/introduction-to-messaging-system?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview), in Grokking System Design Fundamentals
- Free answer: [What to Expect in the Anthropic System Design Interview](https://www.designgurus.io/answers/detail/what-to-expect-in-the-anthropic-system-design-interview?utm_source=github&utm_medium=repo&utm_campaign=anthropic-interview-guide&utm_content=system-design-interview)
- Free guide: [Anthropic system design interview](https://github.com/design-gurus/grokking-system-design/blob/main/companies/anthropic.md), in Grokking System Design
