# Pragmatic Reactive Programming in Java with Project Reactor

Reactor is more than just a _library of operators_. In this workshop, attendees learn how to write **idiomatic, safe, and efficient** reactive code in Java using **Project Reactor**. The focus is on building the core competencies needed to navigate reactive systems *without cargo-culting*: when reactive programming shines, when it hurts, and how to reason about correctness, performance, and operability.

The workshop is modular and tailored to meet your team’s specific needs. We begin with a complimentary assessment to understand your goals and expectations, ensuring the content aligns with your environment, constraints, and tech stack.

## Key learning points

- Foundations: multithreading and asynchronous programming
  - a distilled version of our deep-dive workshop: [Multithreading and asynchronous programming in Java](../java-async-programming/workshop.md)

- Reactive principles and standards
  - The Reactive Manifesto: what it promises (and what it doesn’t)
  - Reactive Streams: why backpressure exists and what it costs
  - Reactive Extensions: stream processing as a mental model

- Project Reactor fundamentals
  - **Threading model**: who runs what, when, and why
  - **Cold vs hot publishers** and the consequences for correctness and load
  - **Backpressure**: strategies, buffering, and how overload actually manifests
  - `publishOn()` vs `subscribeOn()` and common pitfalls
  - **Schedulers**: choosing the right one; avoiding scheduler starvation
  - Operators and composition patterns (transformations, flattening, concurrency control)
  - Lifecycle hooks (`doOn…`, `doFinally`, `usingWhen`, etc.) and safe resource handling
  - Error handling and recovery: retry strategies, timeouts, fallbacks, and “poison” signals
  - Testing reactive pipelines: `StepVerifier`, `TestPublisher`, `VirtualTimeScheduler`
  - Parallelization patterns and safe concurrency
  - Debugging techniques: checkpoints, stack traces, `Hooks`, operator debugging trade-offs
  - Performance tuning: allocation hotspots, fusion, throughput vs latency trade-offs
  - Context propagation: Reactor `Context`, request-scoped data, logging correlation

- Finding and fixing the biggest real-world failure mode: **blocking**
  - Identifying unwanted blocking operations
  - Handling blocking I/O safely (`boundedElastic`, offloading patterns, bulkheads)
  - Why blocking inside reactive pipelines is so destructive

- Context and state management
  - `ThreadLocal` variables vs Reactor `Context` (and why they don’t mix by default)
  - Designing APIs that don’t require thread-local state

- Reactive web applications with Spring
  - Spring WebFlux architecture and runtime model
  - Refactoring Spring MVC to WebFlux: migration strategies and pitfalls
  - Observability: WebFlux and distributed tracing; correlation IDs; context propagation to logs/traces

- Reactive data access and integration
  - Reactive database access: when it helps, when it complicates your domain model
  - RSocket: protocol overview, interaction models, and real use cases

- Reactive programming vs virtual threads
  - Comparing models: ergonomics, performance characteristics, and operational complexity
  - How to choose pragmatically (and when to mix approaches)

<a href="mailto:contact@4comprehension.com">Reach out for a free training needs analysis!</a>
