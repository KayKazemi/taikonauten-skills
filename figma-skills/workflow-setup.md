---
name: workflow-setup
description: Set up a design team workflow and rituals.
argument-hint: "[team size and context, e.g., '4-person design team in a startup' or 'design system team']"
---

# workflow-setup

Set up a design team workflow.

## Steps

1. **Team structure** — Define roles and responsibilities using `workflow-team` skill.
2. **Rituals** — Establish collaboration cadence using `workflow-team` skill.
3. **Critique process** — Set up design critique format using `workflow-design-critique` skill.
4. **Review gates** — Define quality checkpoints using `workflow-design-review-process` skill.
5. **Versioning** — Establish file and library versioning using `design-system-version-control` skill.
6. **QA process** — Set up design QA workflow using `workflow-design-qa-checklist` skill.

## Output

Team workflow document with rituals calendar, critique format, review process, versioning strategy, QA checklist, and tooling recommendations.
Consider following up with `workflow-design-sprint-plan` to kick off your first project with the new workflow.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `workflow-setup — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
