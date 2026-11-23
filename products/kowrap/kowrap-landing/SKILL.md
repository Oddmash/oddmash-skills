---
name: kowrap-landing
description: Change or verify the Kowrap landing, typography, live CSS comparison, or documentation site. Use for Kowrap browser measurements and static site delivery, including the width ruler.
---

# Kowrap landing and docs

Read Kowrap's AGENTS.md and CONTRIBUTING.md. Preserve Next.js static export, the configured deployment base path, and the boundary between site presentation and the published engine.

- Make the first view identify Kowrap as a Korean line-breaking library, then show actual CSS keep-all and WrapText results simultaneously, at equal measured widths and font settings. Use realistic copy with a visible change in a complete word. Keep the editor and synchronized code discoverable; expose forced breaks as an optional Kowrap-only control. If viewport constraints clamp a requested width, show the measured width rather than implying the requested one is rendered.
- Keep display typography and decoration separate from the text used for the comparison. Record font source, license, transfer size, fallback, and font-ready remeasurement. When heading glyphs are subsetted, update the subset with the copy.
- Treat width as committed input. Animate the measuring marker independently and match the settled marker to the rendered width. A before/after replay must derive its movement from both rendered word positions; keep the results visible, use a static destination cue for reduced motion, and verify rapid input.
- Verify with the repository's static build and Chromium, Firefox, and WebKit. Include the landing workflow and relevant documentation routes. Check font failure, code disclosure and copy, and the configured base path when affected.
