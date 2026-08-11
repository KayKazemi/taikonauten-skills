---
name: interaction-design
description: Design a complete interaction flow for a feature or component.
argument-hint: "[feature or component, e.g., 'add to cart flow' or 'drag-to-reorder list']"
---

# interaction-design

Design a complete interaction flow.

## Steps

1. **States** — Model the interaction states using `interaction-state-machine` skill.
2. **Micro-interactions** — Specify each micro-interaction using `motion-micro-interaction-spec` skill.
3. **Animation** — Define motion using `motion-principles` skill.
4. **Gestures** — Design touch/pointer interactions using `interaction-gesture-patterns` skill.
5. **Feedback** — Specify system feedback using `interaction-feedback-patterns` skill.
6. **Error handling** — Design error paths using `interaction-error-handling-ux` skill.
7. **Loading** — Design loading states using `interaction-loading-states` skill.

## Output

Complete interaction specification with state diagram, micro-interaction specs, animation details, gesture definitions, feedback plan, error flows, and loading states.
Consider following up with `interaction-map-states` for complex components or `interaction-error-flow` for critical paths.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `interaction-design — [input]`. Lay it out using the layout, typography, color, and spacing conventions established above. Build incrementally and verify the result with a screenshot before finishing.
