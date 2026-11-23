---
name: oddmash-release-management
description: Prepare or verify an Oddmash release, version bump, package publication, deployment, release notes, or rollback while respecting each repository's release policy.
---

# Oddmash release management

Read the target repository's release policy, current version, remote state, open changes, and deployment instructions. A skill does not grant permission to publish, merge, or deploy.

- Establish the exact release candidate, previous published version, intended audience, and affected artifacts. Derive the version from the repository policy and actual compatibility impact rather than guessing.
- Reconcile package metadata, changelog, release notes, documentation, and artifacts. For libraries, verify the packed artifact in a clean consumer and public imports, types, runtime peers, and CSS where relevant. For deployed products, verify the intended environment and URL.
- Require appropriate passing checks for the exact candidate and evidence for changed behavior. Separate local tests, CI, preview, and production verification. Stop before any production action if authorization, required approvals, or the candidate state is unclear.
- For an authorized release, follow the repository's native publishing mechanism and verify the actual published version or deployment. Never expose credentials, bypass protected workflows, or assume workflow success means the artifact is available.
- Record exact revision, release URL, user-visible changes, verification gaps, and rollback or recovery path. If a failure occurs, preserve the previous working release and report the concrete blocker.

Use [quality assurance](../oddmash-quality-assurance/SKILL.md) for evidence and [product marketing](../oddmash-product-marketing/SKILL.md) for release communication.
