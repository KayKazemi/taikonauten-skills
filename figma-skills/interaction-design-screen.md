---
name: interaction-design-screen
description: Design a complete screen layout from a description or requirements.
argument-hint: "[screen description, e.g., 'user profile settings page' or 'e-commerce product listing']"
---

# interaction-design-screen

Design a complete screen layout from a description.

## Steps

1. **Structure** — Define layout grid using `interaction-layout-grid` skill.
2. **Hierarchy** — Establish visual priority using `interaction-visual-hierarchy` skill.
3. **Typography** — Apply type styles using `design-system-typography-scale` skill.
4. **Color** — Apply color system using `design-system-color` skill.
5. **Spacing** — Apply consistent spacing using `design-system-spacing` skill.
6. **Responsive** — Define behavior across breakpoints using `interaction-responsive-design` skill.
7. **Dark mode** — Specify dark mode adaptation using `interaction-dark-mode-design` skill.

## Output

Complete screen specification with layout, hierarchy, typography, color, spacing, responsive behavior, and dark mode.
Consider following up with `interaction-responsive-audit` to verify the design.

## Build

Use the `figma-use` skill to materialize the screen as a new frame on the current page in the active Figma file, named `interaction-design-screen — [input]`. Lay it out as a real UI screen using the layout grid, hierarchy, typography, color, and spacing established above. Build incrementally (skeleton first, then fill in content) and verify the result with a screenshot before finishing.
