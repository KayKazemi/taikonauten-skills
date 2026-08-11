---
name: design-system-tokenize
description: Extract and organize design tokens from an existing design or stylesheet.
argument-hint: "[CSS file, design file, or description of values to tokenize]"
---

# design-system-tokenize

Extract hard-coded values and organize into a structured token system.

## Steps

1. **Extract** — Scan for all visual values.
2. **Deduplicate** — Group similar values using `design-system-token` skill.
3. **Categorize** — Organize by category.
4. **Hierarchy** — Define global/semantic/component tiers using `design-system-token` skill.
5. **Naming** — Apply conventions using `design-system-naming-convention` skill.
6. **Themes** — Map variants using `design-system-theming` skill.
7. **Document** — Generate reference using `design-system-documentation-template` skill.

## Output

Token specification with inventory, hierarchy, theme mapping, and migration guide.
Consider following up with `design-system-audit`.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `design-system-tokenize — [input]`. Lay it out using the layout, typography, color, and spacing conventions established above. Build incrementally and verify the result with a screenshot before finishing.
