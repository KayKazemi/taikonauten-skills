---
name: design-system-audit
description: Run a comprehensive audit of an existing design system for consistency, completeness, and accessibility.
argument-hint: "[design system name or description of what to audit]"
---

# design-system-audit

Audit the specified design system or component library.

## Steps

1. **Inventory** — List all components, tokens, patterns using `design-system-component-spec` and `design-system-token` skills.
2. **Consistency** — Evaluate naming using `design-system-naming-convention` skill.
3. **Completeness** — Check for missing states/docs using `design-system-documentation-template` skill.
4. **Accessibility** — Review against WCAG 2.2 AA using `accessibility-audit` skill.
5. **Token coverage** — Verify token usage using `design-system-token` skill.
6. **Theming** — Check theme support using `design-system-theming` skill.
7. **Report** — Prioritized findings with severity ratings.

## Output

Audit report with executive summary, issue counts by severity, detailed findings, and remediation roadmap.
Consider following up with `design-system-component-spec` or `design-system-tokenize`.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `design-system-audit — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
