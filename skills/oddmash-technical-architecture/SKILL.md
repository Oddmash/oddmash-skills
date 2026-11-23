---
name: oddmash-technical-architecture
description: Assess or design an Oddmash technical architecture, API or data contract, dependency choice, system boundary, or migration before materially changing a product.
---

# Oddmash technical architecture

Read the current architecture, repository agreements, runtime constraints, public contracts, and the concrete requirement. Prefer the smallest change that preserves existing behavior and can be verified.

- Map affected boundaries, ownership, data flow, and failure behavior. Separate domain logic from rendering and transport where that creates a stable testable boundary. Keep product-specific decisions in the product repository.
- Compare a small set of viable options against compatibility, maintenance, latency, complexity, cost, deployment constraints, and reversibility. Record why a dependency or abstraction earns its place rather than selecting it by popularity.
- Define contracts and invariants explicitly: types, errors, state transitions, data ownership, versions, and supported consumers. For migrations, identify old and new readers/writers, rollback conditions, and how existing data remains compatible.
- For sensitive data, define which component may access it and minimize permissions, retention, and disclosure. Use safe defensive design review; do not execute untrusted code or develop attacks. Do not assume authorization to access production systems.
- Document the selected design, rejected alternatives, unresolved risks, and a first independently verifiable implementation slice. Validate with the product's actual tests and runtime.

Use [quality assurance](../oddmash-quality-assurance/SKILL.md) for verification design and [web delivery](../oddmash-web-delivery/SKILL.md) for frontend implementation.
