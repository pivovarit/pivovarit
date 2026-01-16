# Challenges of Distributed Systems

In this workshop, attendees learn the fundamentals of distributed systems and how to navigate their challenges.

Modern architectures increasingly rely on distributed components: microservices, event-driven systems, streaming platforms, caches, multi-region deployments, and third-party integrations. 

While these approaches can improve scalability and team autonomy, they also introduce a new class of problems—problems you don’t see in a single-process or single-node system. 

This workshop focuses on the foundational constraints and challenges of distributed systems.

The workshop is modular and tailored to meet the specific needs of your team. We begin with a complimentary assessment to understand your goals and expectations, ensuring the content is aligned with your needs.

Key learning points:
- CAP theorem and choosing trade-offs intentionally
- partial failures: latency, timeouts, retries, and cascading overload
- delivery guarantees: at-most-once, at-least-once, and exactly-once
- idempotency
- optimistic concurrency control and pessimistic locking
- ordering, duplications, and replays: designing for out-of-order events and redelivery
- exactly-once processing in practice: semantics vs implementation
- distributed transactions: choreography vs orchestration
- handling dual writes: transactional outbox pattern and change data capture (CDC)
- wall clock time vs logical time: Lamport timestamps, causal ordering
- testing distributed systems: fault injection, network partitions, retries, and chaos-style experiments
- coordination problems: leader election, locks, consensus basics, and when coordination becomes a bottleneck
- operational hygiene and observability
