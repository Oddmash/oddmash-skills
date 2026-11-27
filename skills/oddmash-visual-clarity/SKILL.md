---
name: oddmash-visual-clarity
description: Evaluate and improve visual hierarchy, legibility, readability and discoverability in Oddmash interfaces and product graphics.
---

# Oddmash visual clarity

Inspect the rendered interface at representative desktop and narrow widths. Identify the primary task and what must be noticed first. Assess the result independently of the implementation and functional CI. A correct feature may still have an unclear, cluttered, or visually inappropriate design.

- Establish hierarchy through spacing, size, weight and contrast. Avoid competing accents, excessive bold text, decorative cards and repeated headings. Use product tokens and real content in the supported locales.
- In reading indexes and editorial landings, use closer spacing within a title, its description and its related content than between independent groups. Inspect wrapped headings and descriptions on both sides of column breakpoints. Align corresponding list starts only when neighboring columns are meant to be scanned together. In a single column preserve each natural group height. Compare the rendered relationships as well as measured gaps.
- Preserve legibility under wrapping, zoom and localization. Check density, alignment and clipping. Keep essential information available without hover or motion.
- Distinguish actions, selection, error and success visibly without relying on color alone.
- Use intentional motion to demonstrate real changes; keep content legible and provide pause, reduced-motion and offscreen behavior.
- Compare screenshots and actual tasks. Distinguish observed defects from aesthetic preferences.

- Audit final geometry across skeleton, loading and loaded states, consistent control heights/padding/icon alignment, focus rings, truncation with accessible access to complete content, responsive spacing, safe areas, scroll and overlay layering. Compare empty/error and dense content alongside the happy path. Keep placeholders and decorative motion subordinate to meaningful content.

## Technical visual review

When reviewing diagrams, examples, or visual demonstrations, use the mechanism and visual structure selected by [visual media](../oddmash-visual-media/SKILL.md). Inspect the rendered scene, not only its source or its prose. Check that the focal relationship, direction, labels, boundaries and meaningful differences are visible without reading the adjacent explanation. Compare a simpler alternative: remove decorative cards, repeated text, arrows that do not encode a relationship, and motion that does not expose a change. Preserve legitimate simple sequences; do not demand complexity for its own sake. Verify the scene at its actual embedded width and narrow layout, with accessible equivalent content and honest provenance. Record meaning and readability acceptance separately from functional CI.

## Subtractive visual review

For a substantial landing change, apply the [product-specific website acceptance gate](../oddmash-brand-design/references/product-website-direction.md#acceptance-before-handoff). Record concrete visible evidence for the primary action, hero artifact, full-page hierarchy and narrow layout. Investigate a large unexplained empty region, clipped focus, misaligned control/icon, or unsolicited sticky/scroll-following content before declaring ready.

- Before adding or retaining a label, metric, badge, progress indicator, explanatory sentence or control, identify the specific user decision it supports. Remove it when the result, adjacent content or existing control communicates the same information. Do not default to pills, badges, separate columns, progress indicators, or additional text for ordinary states. Use the lightest legible signal that conveys the required meaning. Keep essential accessibility semantics and measured values needed for an actual input constraint.
- Inspect the entire rendered page at desktop, representative mobile and the narrow supported breakpoint. Then inspect high-risk components at their actual allocated width, including tab lists, toolbars, copy buttons and overlays. Check both axes of internal overflow, alignment and clipping; do not accept document-level reflow alone. Reserve scrollbar behavior for intentionally scrollable content such as long code, not ordinary controls.
- For a multi-column reading interface, inspect the complete viewport with left navigation, reading column, contextual rail and header together. Verify the intended readable measure, actual allocated widths, internal gaps and unused space on both outer edges at breakpoint boundaries and representative ultrawide widths. Do not fix one oversized gutter by relocating the same empty region to the other edge. Choose a balanced composition deliberately; avoid stretching prose indefinitely just to consume space. Compare full screenshots and geometry before and after, including short and long pages and expanded navigation with scrollbars.

- Inspect product preview assets themselves and their rendered frames. Preserve meaningful product UI such as navigation sidebars, toolbars, labels and focus context; avoid accidental cropping from image aspect-ratio or object-fit choices. If a close-up is intentional, identify it as such and keep a representative complete interface available without hovering.
- Review the initial, transitioning and settled visual states. A successful interaction test is not a visual approval. Record concrete defects and resolve them before considering the surface ready. If the same critique returns after multiple patches, assess the whole composition and owning design decision; test a simpler alternative instead of adding another rule or decoration. Inspect critical transitions as well as the still frame. Compare the result against the user goal, not whether previous controls or expected animation classes still exist.

For operational dashboards, assess the changed operator tasks against [dashboard design](../oddmash-dashboard-design/SKILL.md). Inspect actual allocated widths, readable data hierarchy, icon baselines, state prominence, detail interactions and all supported themes. Record rendered acceptance separately from functional CI.
