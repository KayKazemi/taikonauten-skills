---
name: testing-evaluate
description: Run a heuristic evaluation of an existing design.
argument-hint: "[design, screen, or flow to evaluate]"
---

# testing-evaluate

Run a heuristic evaluation of a design.

## Steps

1. **Scope** — Define screens and flows to evaluate.
2. **Heuristic review** — Evaluate against Nielsen's heuristics using `testing-heuristic-evaluation` skill.
3. **Flow analysis** — Review user flows for issues using `interaction-user-flow-diagram` skill.
4. **Accessibility check** — Evaluate accessibility using `accessibility-test-plan` skill.
5. **Severity rating** — Rate and prioritize all findings.
6. **Recommendations** — Provide specific improvement suggestions.

## Output

Evaluation report with findings per heuristic, severity ratings, accessibility issues, and prioritized recommendations.
Consider following up with `testing-usability-test-plan` to validate findings with real users.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `testing-evaluate — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
