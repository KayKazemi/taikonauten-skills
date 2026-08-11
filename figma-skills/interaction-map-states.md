---
name: interaction-map-states
description: Model the states and transitions for a complex UI component.
argument-hint: "[component name, e.g., 'media player' or 'multi-step checkout']"
---

# interaction-map-states

Model states and transitions for a complex component.

## Steps

1. **Identify states** — List all possible states using `interaction-state-machine` skill.
2. **Map transitions** — Define events and transitions using `interaction-state-machine` skill.
3. **Loading states** — Define loading behavior per state using `interaction-loading-states` skill.
4. **Error states** — Map error conditions using `interaction-error-handling-ux` skill.
5. **Feedback** — Define feedback per transition using `interaction-feedback-patterns` skill.
6. **Animation** — Specify transition animations using `motion-principles` skill.

## Output

Complete state machine diagram with states, events, transitions, guards, actions, and UI representation per state.
Consider following up with `interaction-design` for detailed interaction specs.

## Build

Use the `generate_diagram` tool to create a FigJam board named `interaction-map-states — [input]`, using Mermaid `stateDiagram-v2` syntax: one state per node, labeled transitions for each event, guards noted in transition labels, and nested/composite states for any sub-states (e.g. loading sub-states within a parent state). If more than one Figma plan/team is available, ask which to use before generating.
