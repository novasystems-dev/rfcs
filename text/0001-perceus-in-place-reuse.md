# RFC 0001: Perceus In-Place Buffer Recycling

- Feature Name: `perceus_in_place_reuse`
- Start Date: 2026-11-06
- Status: Accepted / Implemented in Nova v0.1.0+

## Summary
Employs precise reference-counting with compile-time in-place buffer recycling (Perceus model). When an object's reference count is proven to be 1 at runtime, mutations execute destructively in place without allocating new memory chunks, eliminating garbage collection pauses completely.
