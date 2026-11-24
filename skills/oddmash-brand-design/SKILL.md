---
name: oddmash-brand-design
description: Establish or review Oddmash visual direction for websites and product interfaces, including product-specific landing pages, brand geometry, semantic color, multilingual typography, and responsive hierarchy.
---

# Oddmash brand design

Read the product's visual baseline. For interfaces using Oddmash UI, inspect the shared tokens and the product's semantic overrides. Treat the individual product's identity as the primary design system: derive its palette, typography, geometry, imagery, layout rhythm, and visual examples from its purpose, audience, and existing assets. Use shared Oddmash tokens and components as adaptable defaults, not a mandatory visual theme or fixed composition. If no identity exists, establish a product-specific direction before implementation. Do not copy an unrelated product's palette or use the organization ribbon as decoration by default.

For new or substantially revised landing pages, read [product-specific website direction](references/product-website-direction.md) before choosing a composition or writing code. Derive the direction from the real product and apply its rendered acceptance checks even when the request only says to make a landing page.

- Where the Oddmash ribbon is part of the product identity, study the approved mark before deriving shapes. Its distinctive cues are continuity through the folds, adjoining front and reverse planes, and the change of light at each bend. Use those cues to mark a real boundary, direction, or grouping. Review the main scene with decorative marks hidden. If the remaining layout has no product-specific focal point, revise the composition.
- Use contrast and hierarchy before extra ornament. When using the shared neutral palette, reserve blue for focus and red for errors; otherwise select accessible semantic colors that fit the product. Preserve meaningful product-specific colors and encode states in more than one visual channel where needed.
- Ground the hero in a real product artifact, such as a verified code example, actual interface or gameplay. Avoid generic marketing layouts made from repeated eyebrow labels, oversized slogans, decorative metrics, gradients, and interchangeable card grids. Do not treat this as a ban on useful cards or product-specific visual effects; choose the layout according to the actual content and task.
- Choose display, body, UI, and code faces by role. Geist Sans and Geist Mono are useful starting points in the shared system. Check actual glyph coverage, mixed-script line breaks, fallback, transfer size, and the license before committing font assets.
- For Korean prose, apply [Korean typography and Kowrap adoption](../oddmash-internationalization/references/korean-typography.md); judge semantic line breaks with actual type and measured layout, not hardcoded line breaks or a visual guess.
- Compare real renders at narrow and desktop widths, including long labels and visible focus. Keep product-specific styling in the consumer. Promote an abstraction into Oddmash UI once more than one product demonstrates the same stable need.

For a motion brief, use the [motion design skill](../oddmash-motion-design/SKILL.md).

Use [web delivery](../oddmash-web-delivery/SKILL.md) for framework and delivery choices, [developer documentation](../oddmash-developer-documentation/SKILL.md) for public API content, and [visual clarity](../oddmash-visual-clarity/SKILL.md) for independent rendered assessment.

- Review complete interaction states using actual token pairs in every supported theme, including skeleton, disabled, pending, warning, error, success, focus and selected. Check contrast and non-color cues with [accessibility](../oddmash-accessibility/SKILL.md); document font, icon and asset rights with [copyright and licensing](../oddmash-copyright-licensing/SKILL.md).

## Shared soft geometry

Preserve a visible keyboard focus indicator on rounded buttons and links, and ensure it stays visible in every supported theme.

Use a restrained Vercel/Geist-inspired starting point, adjusting values to the brand and real geometry: 6px for small controls, 8px for standard buttons and inputs, 12px for cards and code blocks, 16px for overlays and large surfaces, and 24px for prominent product previews. Reserve pill radii for chips, avatars and compact status indicators. Keep edges straight where alignment or measured content requires it. Use role-based tokens, subtle borders, quiet elevation and generous whitespace; do not round every nested surface. Preserve product colors, imagery and distinct composition. Use the supported themes and evaluate nested corner alignment, focus visibility and overflow in real renders rather than enforcing a numeric radius.
