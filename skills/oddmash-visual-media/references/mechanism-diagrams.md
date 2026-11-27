# Mechanism-specific technical diagrams

Choose one question the reader should answer after viewing the scene. Use the actual source, contract, observed product output or documented example as evidence. Write the entities, relationships, conditions and invariants before selecting a visual form. Where the source does not establish a behavior, label it as an illustrative example or omit it.

## Choose the grammar

| Reader question | Useful visual grammar | Represent directly |
| --- | --- | --- |
| Who imports, calls or owns what? | Architecture or dependency graph | Group boundaries, directional labeled edges, shared dependencies and ownership |
| What happens when a request crosses actors? | Sequence or swimlane | Actors on separate lanes, messages in time order, alternate outcomes |
| What changes after an event or failed operation? | State transition, branching flow, or version timeline | Initial state, event, condition, next state, preserved or rejected state |
| What changed between two implementations? | Aligned comparison | Same input or entity on both sides, changed relationship, result or limitation |
| How does changing input change output? | Interactive example or real output capture | Same input, adjustable variable, visible output, accessible feedback |
| What does the product actually do? | Actual screenshot, focused recording or reproducible demo | Real interface context and a meaningful action; label fixtures and reconstructions |

Use a list for straightforward prose or a simple linear sequence. Use a table for exact repeated-field comparisons. Avoid diagrams that only convert paragraphs into boxes. A more complex diagram is not automatically better.

## Construct the scene

1. Establish a primary visual path and focal relationship. Use placement, alignment, grouping and hierarchy before borders and ornament. Select meaningful node shapes or typographic roles only when distinctions matter.
2. Make edges encode direction, dependency, event, or a condition; label ambiguous edges and branches. Do not join independent facts with sequential arrows. Keep shared entities recognizable rather than duplicating them to fill a grid.
3. Align comparable inputs, states, and outcomes. Highlight the change and disclose trade-offs or boundaries, not merely a green "after" state. Distinguish errors, pending and success with labels or shapes as well as color. Keep exact labels short and preserve source identifiers.
4. Prefer semantic HTML and CSS for readable layouts with native text, tables and controls. Use accessible SVG when explicit connectors, graph geometry or precise paths make the relationship clearer; use a diagram renderer when its layout and accessibility meet the task. Keep diagrams responsive through meaningful reflow, alternate compact layouts, or a deliberately labeled zoomable dense view with a readable equivalent. Never solve narrow layouts by shrinking text beyond legibility or clipping meaningful edges.
5. Use actual captured or reproduced product behavior where practical. For illustrative state or data, identify the source/assumption and distinguish it from a test capture or measurement. Do not invent UI, benchmark results, relationships or traces.

## Representative choices

- A library that changes from one global stylesheet to component-owned CSS: compare the same consumer imports, show which CSS files each reaches, and identify the shared dependency. Do not chain two unrelated component examples as consecutive events.
- Two editors starting at the same revision: place the editors and authoritative store on distinct lanes, show which write succeeds, the rejected stale write, and the retained revision. Do not claim automatic merge if none exists.
- A workflow with current and superseded checks: show decision conditions and distinguish waiting, failed, and eligible outcomes using the documented semantics. Avoid speculative internal roles or a happy-path-only transcript.
- A text layout utility: hold text, font and width constant for the native and enhanced results. If a live comparison is feasible, use actual engine output; check input changes that produce different results and cases where output stays equal; never force a visual difference or imply improvement when the result is unchanged. Otherwise label a manually constructed example as illustrative, not a measured result.

## Acceptance

At the actual embedded width, ask a reader to identify the mechanism without the explanation paragraph: what is related to what, what triggers the change, which result follows, and what is not implied. Choose applicable questions. Compare the render with the source; verify every edge, label, branch, version and outcome. If the reader could learn the same thing from an unchanged short paragraph or the diagram hides the crucial distinction, simplify or redesign.

Inspect desktop and representative narrow supported widths, relevant themes and locales, and adjacent reading content. Check internal text and connector clarity, alignment, clipping, focus where interactive, and a useful nonvisual description. For motion or live input, test triggering, intermediate and settled states and accessible fallback as specified by visual media. Record actual renders and concrete defects fixed; structural tests and screenshots alone do not establish technical accuracy or comprehension.
