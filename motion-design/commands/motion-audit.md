---
description: Audit existing motion design for consistency, brand alignment, performance impact, and accessibility compliance.
argument-hint: "[product or feature to audit]"
---

# /motion-audit

Audit the motion in an existing product.

## Steps

1. **Inventory**: List all animated interactions in $ARGUMENTS — transitions, micro-interactions, loading states, scroll effects, and any decorative motion.
2. **Principles check**: Use the `motion-principles` skill to evaluate each animation against purposefulness — does it direct attention, communicate state, provide feedback, or convey personality?
3. **Consistency check**: Use the `transition-system` skill to assess whether duration and easing values are consistent across the product or arbitrary.
4. **Brand alignment**: Use the `brand-motion` skill framework to evaluate whether the motion feels on-brand or generic.
5. **Performance review**: Flag any animations that animate non-compositable properties (`width`, `height`, `margin`). Note any animations that may impact LCP or CLS.
6. **Accessibility audit**: Check for `prefers-reduced-motion` support and identify any flashing content (WCAG 2.3.1).
7. **Report**: Produce a motion audit with a rating per area, priority fixes, and a recommendation for whether a motion token system is needed.

## Output

Motion audit report with inventory, consistency rating, performance flags, accessibility checklist, and prioritised recommendations.
