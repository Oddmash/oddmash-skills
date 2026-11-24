# Product-specific website direction

## Decide before composing

Read the current product, README, supported features, brand assets, audience, usage examples, and actual UI. Inspect existing screenshots or run the product when possible. Record a concise direction in the work notes: product type, audience, first useful action, three brand traits tied to real evidence, visual anchor, content hierarchy, and what to avoid. If identity is missing, derive it from the product rather than asking the maintainer to pick arbitrary colors. Preserve established identities unless a rebrand is requested.

Choose the dominant visitor task, not a fixed landing template. Combine paths when a product has multiple audiences.

| Product type | First useful action | Design and content direction |
| --- | --- | --- |
| Library or SDK | Install and complete a real integration | Readable editorial or technical typography, restrained palette, searchable native docs, runnable quickstart, API reference, recipes and limitations. Show input/output or a working example above the fold. |
| Developer tool or extension | Inspect or solve a real problem | Real tool UI or a focused interactive workflow, reproducible example, install/setup, compatibility, privacy and troubleshooting. |
| Consumer or SaaS product | Understand the value and start a useful task | Actual product screens, realistic scenarios, product-specific imagery and interaction, clear primary action, relevant pricing/support only when real. |
| Game or entertainment | Understand the experience and play | Gameplay, core loop, controls, genuine atmosphere, distinctive art direction and motion tied to the game; play/download and platform requirements. |
| Studio or portfolio | Understand the maker and inspect projects | Distinct editorial voice, recognizable work, real project artifacts and clear project links; avoid generic agency claims. |

For example, Kowrap should foreground Korean text at the same measured width before/after and readable API documentation. Boundra needs to demonstrate its actual boundary-checking workflow with verified code and results. Vertactics should foreground its actual tactical map workflow and visual identity, not a generic developer-tool dashboard. Treat these as examples of reasoning, not layouts to reproduce.

## Design from identity

- Choose a composition around one irreplaceable product artifact. Compare at least two viable compositions for a substantial redesign (for example editorial demo vs split working surface); choose by visitor task, not trend. Define the typography roles, semantic colors, spacing rhythm, shape language, imagery and motion before polishing.
- Use actual screens, code, outputs, diagrams or gameplay rather than fabricated dashboards, stock filler, or decorative abstract 3D art. Use custom illustration only when it communicates something specific and has appropriate rights.
- Do not default to oversized centered headline, pill eyebrow, gradient glow, glass panels, identical rounded feature cards, gratuitous badges, floating decorative blobs, excessive icons, fake metrics, logo strips or generic AI copy. Any such treatment must have a product-specific purpose. Avoid a uniform hero/features/CTA template across products.
- Use purposeful asymmetry, whitespace, text scale, contrast, and content density. Use the shared soft geometry baseline for controls and surfaces unless the product has a documented reason to diverge; do not impose one palette, font, dark theme or layout on the entire organization. Reuse accessible behavior and semantic tokens without forcing visual sameness.
- Use direct human copy. State what happens, how to use it and what the visitor gains. Remove repeated slogans, padded feature lists, em/en dashes as sentence punctuation, invented evidence and unnecessary labels.
- Animate actual product behavior when useful. Prefer stable demonstrations with natural transitions and distinct examples; avoid endless decorative loops, forced auto-play, controls duplicated elsewhere, or motion that obscures reading. Provide accessible control when automatically moving content requires it, and a reliable static reduced-motion state.

## Native documentation and delivery

For libraries and developer tools, make installation, quickstart, examples, API/configuration, compatibility, limitations and troubleshooting available on the product website when applicable. Use the actual released API and test examples. Add clear navigation, relevant search, readable code blocks with language and copy feedback, headings and anchors, mobile navigation and cross-links. A GitHub source link is supplementary, not the documentation path. For other products, provide the actual usage steps and support needed by the visitor, not an irrelevant API reference.

Derive the page sequence and CTA from the visitor task; omit sections without evidence or purpose. Reuse the existing suitable framework; select a static-first framework for content-heavy projects only when it fits existing constraints.

## Acceptance before handoff

Inspect actual rendered desktop and mobile screenshots and interact with the first useful flow. Answer each question with evidence, not a design claim.

- Can a new visitor identify what this product does and take the primary action without hunting?
- Is the main visual genuine, task-relevant and accurate? Would replacing the product name make the page obviously wrong? If not, revise it.
- Are the primary and secondary actions distinguishable, readable documentation available on-site, and all live examples consistent with the supported product?
- Do real long localized text, code, narrow screens, zoom, keyboard/focus, supported themes, reduced motion and loading/error states remain usable?
- Is the design visually coherent without excessive decoration, generic copy, repetitive sections or brand-incompatible shared components?
- Did the build, navigation, links, examples and relevant interactions actually pass? Record screenshots, commands, exact revision and unverified cases. Revise defects before reporting ready.

Do not promise uniqueness from a checklist alone. Validate against actual content and rendered evidence; if the product cannot be run, label illustrative material and report the missing evidence.

For landing pages, use 16–24px for the primary product preview, 12–16px for supporting surfaces, and 8px for standard actions. Maintain readable spacing and straight content alignment; avoid nested rounded card grids. Review the mobile and desktop hierarchy before delivery.
