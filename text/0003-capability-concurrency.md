# RFC 0003: Capability-Gated Concurrency (iso / val / ref)

- Feature Name: `capability_concurrency`
- Start Date: 2026-11-06
- Status: Accepted / Implemented in Nova v0.1.0+

## Summary
Statically tracks isolation (`iso`), immutable sharing (`val`), and thread-local references (`ref`) to prevent data races and deadlocks at compile time without runtime locks or thread sanitizers.
