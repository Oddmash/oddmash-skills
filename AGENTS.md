# Oddmash skills repository

Follow the [Oddmash concurrent work claims](https://github.com/Oddmash/.github/blob/main/AGENTS.md#concurrent-work-claims) and organization collaboration rules before implementation, review, CI retries, or merges.

Follow the [Oddmash organization agreements](https://github.com/Oddmash/.github/blob/main/AGENTS.md). This repository owns reusable skill text and installation tooling. Product repositories own their build commands, deployment, API contracts, and local instructions.

- Use English for skill manifests, instructions, and commit messages. Keep names stable across changes and make activation boundaries explicit.
- Apply the organization's plain-language convention in skill instructions and generated product copy. Avoid em dashes (U+2014), en dashes (U+2013) as sentence punctuation, decorative separators, and generic slogans; use direct sentences and preserve literal code or quotations.
- Use lowercase kebab-case for new file and directory names across skills and generated projects, except tool/framework-required names, existing public contracts and conventional manifests such as `SKILL.md`, `AGENTS.md`, `README.md` and `package.json`. Follow the organization engineering baseline for identifier, style and compatibility rules. Do not rename existing paths without checking references and migration impact.
- Keep cross-product skills under `skills/`. Use `products/<repo>/` for techniques that require a specific codebase. Link optional details from the entrypoint that uses them.
- Use narrow instructions that change a decision. Assign one owner for each decision or acceptance check and link to it instead of repeating it. Separate required contracts and safety/accessibility requirements from defaults and revisable product preferences. A default must never force an existing layout or unnecessary UI. Verify installation, manifest structure and realistic routing before delivery. Never place secrets or private product data in skill content.
- Treat skills as guidance. They cannot authorize external mutations. A maintainer decides release and production actions.
- Follow the organization ready-for-review default for skill changes and use the Git workflow skill for draft exceptions, verification and merge requirements.
- For any skill-guided repository change, inspect outstanding review findings before handoff, address valid findings with regression evidence, and respond in the original discussion using the scoped review collaboration workflow. Do not confuse a resolved finding with PR approval or request repeated whole-PR reviews.

Run `python3 -m unittest discover -s tests` for installation or validation changes.

## GitHub account use

Follow the [Oddmash GitHub account policy](https://github.com/Oddmash/.github/blob/main/docs/github-account-policy.md). Use the verified maintainer account for authorized GitHub work, with command-scoped authentication and a separate checkout or worktree per session. Reserve the alternate account for isolated tests. Only `qtaghdi` gives final approval to and manually merges external contributions.

## Applying shared and product guidance

Start from the latest authorized user goal, within applicable safety, repository authority, public contracts and accessibility requirements. Establish product purpose and first useful action, then choose the smallest usable design. Apply shared defaults only when they serve that purpose. Existing implementation, screenshots and previous layout choices are evidence and constraints to inspect, not automatic reasons to preserve UI. If they conflict with an authorized redesign, update the decision and its outcome-based tests together; do not weaken real compatibility or accessibility checks.

Use the role map in [README.md](README.md). Load the primary decision owner, the product playbook when relevant, and only the specialists triggered by the changed scope. Resolve contradictory guidance before coding. If repeated feedback reveals a systemic design issue, revisit the original decision and its owning guidance instead of appending a new exception each time.

## Integration contract

- This repository is the source of truth for reusable skills. Do not move agent runtime code, credentials, deployment policy, or product-specific authority here.
- Agent maintainers consume skills by exact path at a reviewed immutable commit, with independent upgrade and rollback decisions. Preserve stable skill names and paths or document migrations.
- Keep implementation lessons in the skill that owns the decision. Link the public product evidence in the change record, and leave product selectors, spacing values, article catalogs, and release commands in the product repository. Record what was observed in automation, the browser, or production.
- Changes to a skill's activation, expected evidence, or compatibility must describe the impact on consumers. A skill cannot grant access, approve a deployment, or override the organization agreements or target repository contracts.

## Agent contribution attribution

Follow the [Oddmash agent attribution convention](https://github.com/Oddmash/.github/blob/main/AGENTS.md#agent-contribution-attribution). When a commit materially incorporates a verified finding or recommendation from Lead, Impact, Triage, QA, Release, Docs, or Architect, append the canonical `Co-authored-by` trailer for each actual contributing GitHub account. Deduplicate trailers, preserve human authorship and record the source role or discussion for shared identities. Do not credit unused advice, coordination or approval alone, and do not rewrite published history.

## Delivery workflow

- Use focused branches from the current `main` and target `main` directly for infrastructure changes. The organization product `develop` convention does not apply here. Preserve existing in-flight work and require current-head CI, review, normal merge commits and approved release or deployment policies.
- Find or create a scoped issue before implementation and verify an explicit issue reference in every implementation PR body before opening and at handoff.

## Skill improvement feedback

Route recurring verified non-security product-quality findings through the [skill improvement proposal workflow](docs/skill-improvement-proposals.md). Maintain one open proposal per owning skill and evidence category, distinguish product defects from shared guidance gaps, and retain independent reviewed consumer upgrades. Skills and agents do not publish or modify guidance without explicit maintainer authorization.
