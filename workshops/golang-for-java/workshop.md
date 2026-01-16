# Idiomatic Go for Java Developers

In this workshop, attendees transition from Java to Go by learning **idiomatic Go**, not "Java written in Go syntax". We focus on the mental model shifts that matter: simplicity over frameworks, composition over inheritance, explicitness over magic, concurrency as a language feature, and pragmatic engineering trade-offs.

The goal is to help Java developers become productive in Go quickly *and* avoid the common traps: over-architecting, misusing interfaces, fighting the error model, and building dependency-heavy designs that Go actively discourages.

The workshop is modular and tailored to meet your team’s specific needs. We begin with a complimentary assessment to understand your goals, use cases (services, CLIs, libraries), and constraints, ensuring the content aligns with your environment.

## Key learning points

- **The Go mindset (what to stop doing, what to start doing)**
    - Why Go resists: deep abstraction stacks, "smart" frameworks, annotation-driven programming
    - Readability as a scalability strategy: code that is easy to audit and change
    - Composition first: small types, explicit dependencies, simple data flows
    - Pragmatic engineering trade-offs: when "less clever" is objectively better
    - Idiomatic Go as a team convention: consistency > personal style

- **Modularity, structure and organization of Go applications**
    - Packages as the primary unit of encapsulation (and how to keep them cohesive)
    - Project layout patterns that scale (internal packages, cmd/, pkg/, and when to avoid them)
    - Boundaries by dependency direction: keeping domain logic framework-agnostic
    - Configuration, wiring, and bootstrap: where “composition root” lives in Go

- **Dependency Injection without a DI container (no Spring required)**
    - Constructor injection with plain functions
    - Composition root: explicit wiring instead of magic
    - Interfaces for seams (only where needed), not everywhere
    - The functional options pattern: extensibility without frameworks
    - Managing lifecycle and shutdown (contexts, closers, graceful termination)

- **Demystifying consumer-side _interfaces_**
    - Interfaces are *discovered*, not declared: design from the caller's needs
    - Accept interfaces, return concrete types: why it improves usability
    - Keeping interfaces small: "one-method" interfaces and capability-based design
    - Avoiding premature abstraction: when interfaces make code worse
    - Testing seams: swapping implementations without heavy mocking

- **Concurrent programming with goroutines and channels**
    - Goroutines vs threads: practical scheduling and what to expect
    - Channels as coordination tools: when to use them (and when not to)
    - Worker pools, fan-out/fan-in, pipelines: common patterns
    - Cancellation, deadlines, and timeouts with `context.Context`
    - Avoiding data races: mutexes vs channels; safe sharing and ownership
    - Backpressure, buffering, and preventing goroutine leaks

- **Effective unit testing without mocks**
    - Table-driven tests and subtests as a default style
    - Testing behavior via real implementations and fakes (not mock-heavy design)
    - In-memory adapters: repositories, clocks, HTTP clients, and message buses
    - Golden tests, property-ish checks, and deterministic concurrency tests
    - Keeping tests fast and meaningful: avoiding overspecification
    - Benchmarking and profiling basics: catching regressions early

## Additional modules (optional, based on your stack)
- Error handling as a design tool: wrapping, classification, and contracts (`errors.Is/As`)
- HTTP services the Go way: stdlib handlers, middleware patterns, and graceful shutdown
- Tooling culture: `gofmt`, `go test`, `go vet`, `staticcheck`, module versioning
- Performance essentials: allocation/escape intuition, slices/maps pitfalls, `pprof` workflow
- Migration playbook: mapping common Java patterns to Go equivalents (and when to drop them)

<a href="mailto:contact@4comprehension.com">Reach out fo
