---
name: workflow-prototype-plan
description: Create a prototyping and testing plan for a design initiative.
argument-hint: "[feature or initiative to prototype and test]"
---

# workflow-prototype-plan

Create a prototyping and testing plan.

## Steps

1. **Strategy** — Choose fidelity and method using `workflow-prototype-strategy` skill.
2. **Flows** — Map user flows to prototype using `interaction-user-flow-diagram` skill.
3. **Wireframes** — Specify wireframe layouts using `interaction-wireframe-spec` skill.
4. **Test scenarios** — Write usability tasks using `testing-test-scenario` skill.
5. **Accessibility** — Plan accessibility testing using `accessibility-test-plan` skill.
6. **Timeline** — Create a prototyping and testing schedule.

## Output

Prototyping plan with fidelity rationale, user flows, wireframe specs, test scenarios, accessibility plan, and timeline.
Consider following up with `testing-usability-test-plan` for detailed usability testing or `testing-evaluate` for expert review.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `workflow-prototype-plan — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
