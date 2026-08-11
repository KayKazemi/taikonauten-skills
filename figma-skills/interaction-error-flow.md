---
name: interaction-error-flow
description: Design a complete error handling flow for a feature.
argument-hint: "[feature name, e.g., 'payment processing' or 'file upload']"
---

# interaction-error-flow

Design complete error handling for a feature.

## Steps

1. **Identify errors** — List all possible error conditions using `interaction-error-handling-ux` skill.
2. **Prevention** — Design prevention measures using `interaction-error-handling-ux` skill.
3. **State modeling** — Map error states using `interaction-state-machine` skill.
4. **Feedback** — Design error communication using `interaction-feedback-patterns` skill.
5. **Recovery** — Design recovery paths using `interaction-error-handling-ux` skill.
6. **Loading** — Handle timeout and retry states using `interaction-loading-states` skill.

## Output

Error handling specification with error inventory, prevention measures, state diagram, error messages, recovery flows, and retry strategies.
Consider following up with `interaction-map-states` for the full component state model.

## Build

Use the `generate_diagram` tool to create a FigJam board named `interaction-error-flow — [input]`, using Mermaid flowchart syntax (LR direction, all shape/edge text quoted) covering the error's full lifecycle: trigger → detection (diamond decision) → error communication (rectangle) → recovery action (rounded rectangle) → retry/resolution or escalation. Color the failure branch distinctly from the recovery/happy-path branch. If more than one Figma plan/team is available, ask which to use before generating.
