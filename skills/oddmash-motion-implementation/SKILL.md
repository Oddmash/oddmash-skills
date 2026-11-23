---
name: oddmash-motion-implementation
description: Implement and test Oddmash web motion with repeatable state transitions, measurement-safe rendering, keyboard input, and a reduced-motion path.
---

# Oddmash motion implementation

Identify the committed state, the measured geometry, and the decoration representing it. If the intended effect is still open, use the [motion design skill](../oddmash-motion-design/SKILL.md).

- Prefer explicit CSS transition properties and the owning product's timing tokens. When an animated property would distort measurement or hit targets, use a transform on a separate decorative layer.
- Compute the target from the newest input. Keep state transitions and focus independent of finish events. Cancel scheduled work when its owner is disposed. Leave first-render markup identical under both motion preferences.
- For width or resize gestures, clamp the marker to the actual available space. The content should update without waiting for decoration. Repeated requests should settle at the last target.
- For a comparison replay, derive the movement vector from actual rendered positions under equal constraints; use a separate non-interactive, accessibility-hidden decoration and keep both committed results readable. Cancel or retarget on new input or a geometry change. Do not animate a CSS width that drives the measurement itself.
- In a browser, test that motion starts when expected, the final geometry matches the committed state, and keyboard input keeps working during interruption. Run a separate reduced-motion case and assert equivalent state and focus without decorative travel.
