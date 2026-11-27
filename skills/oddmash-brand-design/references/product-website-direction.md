# Product-specific website direction

## Decide before composing

Read the current product, README, supported features, brand assets, audience, usage examples, and actual UI. Inspect existing screenshots or run the product when possible. Record a concise direction in the work notes: product type, audience, first useful action, three brand traits tied to real evidence, visual anchor, content hierarchy, and what to avoid. If identity is missing, derive it from the product rather than asking the maintainer to pick arbitrary colors. Preserve established identities unless a rebrand is requested.

Choose the dominant visitor task, not a fixed landing template. Combine paths when a product has multiple audiences.

Confirm the landing's language scope from the product and the intended audience before writing copy. For a multilingual landing or a change to locale behavior, load [internationalization](../../oddmash-internationalization/SKILL.md). Verify each supported locale through the headline, navigation, first action, demo feedback and destination docs. Where a destination is available only in a fallback language, make the language of that destination clear.

| Product type | First useful action | Design and content direction |
| --- | --- | --- |
| Library or SDK | Install and complete a real integration | Readable editorial or technical typography, restrained palette, native docs with search when useful, runnable quickstart, API reference, recipes and limitations. Show input/output or a working example above the fold. |
| Developer tool or extension | Inspect or solve a real problem | Real tool UI or a focused interactive workflow, reproducible example, install/setup, compatibility, privacy and troubleshooting. |
| Consumer or SaaS product | Understand the value and start a useful task | Actual product screens, realistic scenarios, product-specific imagery and interaction, clear primary action, relevant pricing/support only when real. |
| Game or entertainment | Understand the experience and play | Gameplay, core loop, controls, genuine atmosphere, distinctive art direction and motion tied to the game; play/download and platform requirements. |
| Studio or portfolio | Understand the maker and inspect projects | Distinct editorial voice, recognizable work, real project artifacts and clear project links; avoid generic agency claims. |

For example, Juliya should foreground text at the same measured width before/after and readable API documentation. Boundra needs to demonstrate its actual boundary-checking workflow with verified code and results. A game-focused planning tool should foreground its actual map workflow and visual identity, not a generic developer-tool dashboard. Treat these as examples of reasoning, not layouts to reproduce.

## Maintainer-preferred reference sites

Choose references that match the visitor task. Use references named by the maintainer first and inspect current rendered pages before borrowing principles. Record which traits apply. If a site is inaccessible, use its current repository and product guidance and record the visual evidence gap.

- [Boundra](https://oddmash.github.io/boundra/) shows a concrete developer problem and its result near the first action.
- [Oddmash UI](https://oddmash.github.io/oddmash-ui/) gives developers clear paths to installation, component usage and an interaction lab.
- [Oddmash Website](https://oddmash.github.io/oddmash-website/) uses a single brand mark, a compact project gallery and purposeful workflow motion.
- [Juliya](https://oddmash.github.io/juliya/) uses one genuine interactive demonstration as the focal point, with synchronized examples and native developer documentation.
- Borrow the way a reference makes its product understandable. Keep colors, artwork, component arrangement and page structure grounded in the current product.
- For a material redesign, compare the candidate against these references on content density, whitespace, hierarchy and first-action discoverability. Do not claim visual parity without inspecting actual renders.

## Motion for product proof

Decide what behavior the visitor needs to see before choosing an animation. A static output is sufficient when the visitor can already understand the result. When movement communicates a change, load [motion design](../../oddmash-motion-design/SKILL.md) before implementing the hero. Start with the visitor's input and show the real consequence on the same surface. For a gesture or stateful component, let the visitor trigger the change and offer a keyboard-operable equivalent. Use automatic sequencing when multiple real states need explanation and the sequence adds context the visitor cannot get from the initial view. Keep the headline and first action visible from first paint. Check an interrupted transition and a reduced-motion state that still demonstrates the outcome.

For an immersive hero, compare a spacious demonstration stage with a static proof. Use one artifact to connect cause, action and consequence. Juliya reveals reflow across measured widths. Boundra could show an architecture path, a diagnostic and a corrected path. Follow the motion specialist's sequencing and interruption guidance when automatic playback serves that story.

## Design from identity

For a new or material redesign, use a short direction record with two compositions, real visual reference or product artifact provenance, and the reason the chosen layout serves the first useful action. Do not make collection of references a blocker for a small requested edit. Establish an explicit above-the-fold reading order at desktop and narrow widths; avoid burying a first usable example below generic copy. Choose one primary action per decision point; retain secondary destinations only when they serve distinct outcomes.

- Choose a composition around one irreplaceable product artifact. Compare at least two genuinely different compositions for a substantial redesign (for example a single transforming artifact vs simultaneous comparison). Consider removing existing UI before adding to it; choose by visitor task, not trend or existing markup. Define the typography roles, semantic colors, spacing rhythm, shape language, imagery and motion before polishing.
- Use actual screens, code, outputs, diagrams or gameplay rather than fabricated dashboards, stock filler, or decorative abstract 3D art. Use custom illustration only when it communicates something specific and has appropriate rights.
- Do not default to oversized centered headline, pill eyebrow, gradient glow, glass panels, identical rounded feature cards, gratuitous badges, floating decorative blobs, excessive icons, fake metrics, logo strips or generic AI copy. Any such treatment must have a product-specific purpose. Avoid a uniform hero/features/CTA template across products.
- Use purposeful asymmetry, whitespace, text scale, contrast and content density. Choose the surface and accent from the product's current identity and the needs of its main artifact, such as readable code or visible focus. When the identity is still forming, compare distinct palette directions on that same artifact and record the reason for the choice. Light surfaces, dark surfaces and green accents are all product decisions. Shared components provide accessible behavior and semantic token roles. Set product-level token values to match the chosen direction.
- Use direct human copy. State what happens, how to use it and what the visitor gains. Remove repeated slogans, padded feature lists, em/en dashes as sentence punctuation, invented evidence and unnecessary labels.

## Native documentation and delivery

For libraries and developer tools, use the [developer documentation](../../oddmash-developer-documentation/SKILL.md) skill for the complete human-facing documentation and usage journey. Keep the landing focused on the product proof and the path to those docs. For other products, provide usage steps and support when needed, not an irrelevant API reference.

Derive the page sequence and CTA from the visitor task; omit sections without evidence or purpose. Route framework selection to [web delivery](../../oddmash-web-delivery/SKILL.md).

## Acceptance before handoff

Inspect actual rendered desktop and mobile screenshots and interact with the first useful flow. Answer each question with evidence, not a design claim.

- Can a new visitor identify what this product does and take the primary action without hunting?
- Is the main visual genuine, task-relevant and accurate? Would replacing the product name make the page obviously wrong? If not, revise it.
- Are the primary and secondary actions distinguishable, readable documentation available on-site, and all live examples consistent with the supported product?
- Do real long localized text, code, narrow screens, zoom, keyboard/focus, supported themes, reduced motion and loading/error states remain usable?
- Is the design visually coherent without excessive decoration, generic copy, repetitive sections or brand-incompatible shared components?
- Did the build, navigation, links, examples and relevant interactions actually pass? Record screenshots, commands, exact revision and unverified cases. Revise defects before reporting ready.

Do not promise uniqueness from a checklist alone. Validate against actual content and rendered evidence; if the product cannot be run, label illustrative material and report the missing evidence.

## Subtractive composition gate

For material landing changes, capture and inspect full-page renders and critical crops at representative desktop, mobile and the narrow supported breakpoint. Compare actual before/after renders when redesigning. Inspect the first useful action end-to-end, header and navigation, demo/code area, footer, localized long copy and interaction states. Check computed layout and screenshot geometry for blank gaps, clipping, internal scrollbars, image crop, misaligned icon/label pairs and competing focal points. Check intermediate animation frames for overlapping glyphs or unreadable text as well as the initial and settled states. Test scroll position and motion interruption; automatic content must not unexpectedly follow scrolling or obscure reading. A visual review must report concrete observed defects (or explicitly unverified surfaces) rather than treating green CI as design acceptance.

For each section, state its distinct job in the visitor journey. Remove redundant sections, repeated descriptions, implementation telemetry and decorative controls. Put installation and a real integration example near the first product proof for libraries unless a stronger visitor task justifies another order. Inspect the actual visual density, component allocation, responsive toolbar wrapping and internal overflow; keep deliberate scrolling for long content while ensuring controls do not acquire accidental scrollbars. Require an intentional visual review after functional CI rather than relying on it.

Apply the [shared visual language](../SKILL.md#shared-visual-language) to the landing page. Keep a primary preview, supporting surfaces and actions visually distinct. Check how the product's geometry and spacing carry the hierarchy at mobile and desktop widths.
