# QA evidence and release recommendation

## Severity and triage

Classify confirmed findings by impact rather than visual preference. Keep priority separate from severity and explain uncertainty.

| Severity | Typical impact |
| --- | --- |
| S0 Critical | Confirmed severe data loss/exposure, critical safety risk or fundamentally unusable release |
| S1 High | Core task blocked, material accessibility barrier, major compatibility regression or serious recovery failure |
| S2 Medium | Important degraded workflow with reasonable workaround or bounded impact |
| S3 Low | Minor usability, visual or documentation defect |

Document material legal or privacy uncertainty as an unresolved release risk, not a fabricated confirmed defect. Report defensive security concerns without exploit instructions.

## Case evidence

Record case ID, requirement, expected result, actual result, outcome (pass / fail / blocked / not applicable / not run), environment, exact revision, evidence and issue or fix reference. For not applicable state the reason; for blocked or not run state the missing environment or prerequisite. Do not include real customer information or secrets.

## Defect report

- Concise English issue title for public repositories; affected feature and version.
- Severity, priority, scope, actual versus expected behavior, safe minimal reproduction and relevant sanitized evidence.
- Recommended remediation and regression criterion; note whether confirmed, suspected or environmental.
- Link existing issues rather than duplicating them. Post only if authorized.

## Handoff

Summarize tested revision and environments, exact commands and outcomes, matrix counts, critical user journeys, verified fixes, open defects, blockers, coverage gaps and residual risks. Quantify what was covered as a denominator where practical (routes, scenario cases, engines, viewports, interactive states), and distinguish inspecting every route from exercising every state or input sequence. Distinguish local, CI, preview and production evidence. For a deployed site, record the deployed revision and a result checked at the live URL. Name the browser engine, branded browser, or physical device actually used. WebKit automation does not establish Safari app coverage, and a mobile viewport does not establish physical-device, software-keyboard, or address-bar behavior.

Recommend **ready** only when all applicable mandatory checks pass, required CI/review is current and there are no unresolved material blockers. Recommend **not ready** for failed or unverified mandatory checks, critical/high defects affecting release, or unresolved material risk; identify next steps. Optional findings may be deferred with explicit maintainer review and recorded scope. This is a QA recommendation, not permission to merge, publish or deploy.

## Escalation boundaries

Seek specialist human review for binding legal/compliance decisions, independent accessibility certification, regulated or safety-critical products, real financial reconciliation, high-impact privacy incidents and production security assurance. Use applicable official requirements and qualified specialists; do not claim certifications or guarantees from an automated test. Validate real-device and user-research claims with genuine evidence; mock results are not substitutes.
