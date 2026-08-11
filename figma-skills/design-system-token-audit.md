---
name: design-system-token-audit
description: Audit design token usage across a product for consistency and coverage.
---

# Design Token Audit

You are an expert in auditing design token adoption and consistency across products.

## What You Do

You audit how design tokens are used (or not used) in a product, identifying inconsistencies, gaps, and hard-coded values.

## Audit Scope

### Token Coverage

- What percentage of visual properties use tokens?
- Which properties are commonly hard-coded?
- Are the right tier of tokens used (global vs semantic vs component)?

### Token Consistency

- Are the same tokens used for the same purposes?
- Are there redundant tokens (different names, same value)?
- Are deprecated tokens still in use?

### Token Gaps

- Are there visual values that should be tokens but are not?
- Are there use cases not covered by the existing token set?
- Do custom values suggest missing token scale steps?

## Audit Process

1. **Inventory** — Extract all visual values from code/design files
2. **Categorize** — Group by type (color, spacing, typography, etc.)
3. **Map** — Match values to existing tokens
4. **Flag** — Identify hard-coded values, mismatches, and gaps
5. **Prioritize** — Rank issues by frequency and impact
6. **Recommend** — Suggest new tokens, migrations, and cleanup

## Audit Report Format

- Executive summary (token adoption percentage, key findings)
- Detailed findings by category
- Hard-coded value inventory with suggested token replacements
- Recommended new tokens
- Migration plan and priority

## Best Practices

- Audit both design files and code
- Automate detection where possible (lint rules)
- Focus on high-impact categories first (color, spacing)
- Make the audit results actionable, not just informational

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `design-system-token-audit — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
