---
name: interaction-responsive-audit
description: Audit a design for responsive behavior across breakpoints.
argument-hint: "[screen or feature name to audit]"
---

# interaction-responsive-audit

Audit a design for responsive behavior.

## Steps

1. **Breakpoints** — Review behavior at each breakpoint using `interaction-responsive-design` skill.
2. **Grid** — Check layout grid compliance using `interaction-layout-grid` skill.
3. **Typography** — Verify type scaling using `design-system-typography-scale` skill.
4. **Spacing** — Check spacing consistency using `design-system-spacing` skill.
5. **Hierarchy** — Verify hierarchy holds at all sizes using `interaction-visual-hierarchy` skill.
6. **Touch targets** — Verify minimum sizes for touch using `interaction-responsive-design` skill.
7. **Report** — Document findings with recommendations.

## Output

Responsive audit report with findings per breakpoint, compliance status, and remediation recommendations.
Consider following up with `interaction-design-screen` to redesign problem areas.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `interaction-responsive-audit — [input]`. Lay it out using the layout, typography, color, and spacing conventions established above. Build incrementally and verify the result with a screenshot before finishing.
