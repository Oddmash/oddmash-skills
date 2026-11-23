---
name: oddmash-quality-assurance
description: Design or assess Oddmash functional, usability, accessibility, performance, compatibility, or regression verification for a product change.
---

# Oddmash quality assurance

Read the requirements, repository test commands, current behavior, and affected contracts. Define the expected result before running checks.

- Build a risk-based test matrix covering the changed behavior, relevant boundary values, failure and recovery, and existing behavior that must remain stable. Prefer meaningful assertions over snapshots or test counts.
- For user-facing changes, verify real interaction under representative conditions: keyboard, focus, narrow layouts, long labels, relevant themes, reduced motion, and actual browser or device behavior. Choose browser coverage based on the affected platform.
- For performance, use the same fixtures, environment, measurement definition, and repeated runs when comparing alternatives. Report variance and distinguish measured results from estimates.
- Add focused regression coverage for confirmed defects when implementation is authorized. Keep fixtures synthetic, deterministic, and free of private data; avoid external side effects and offensive testing.
- Record tested revision, commands, conditions, results, reproducible observations, and unverified cases. A passing local test is not evidence of remote CI or deployment success. Separate environment blockers from failed assertions.

Use product-specific verification playbooks when applicable; they supplement rather than replace these criteria.
