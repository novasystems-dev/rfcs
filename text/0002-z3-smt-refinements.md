# RFC 0002: Z3 SMT Compile-Time Refinement Verification

- Feature Name: `smt_refinement_types`
- Start Date: 2026-11-06
- Status: Accepted / Implemented in Nova v0.1.0+

## Summary
Integrates the Microsoft Z3 SMT theorem prover directly into the Nova typechecker. Refinement predicates like `{x: Int | x > 0}` or `{n: Int | n >= 0 && n < len}` are verified at compile-time, eliminating runtime array bounds checks and zero-division panics with formal proof.
