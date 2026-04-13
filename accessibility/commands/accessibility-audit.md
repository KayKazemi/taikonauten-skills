---
description: Run a full accessibility audit across a product or component set, covering WCAG 2.2 AA, keyboard navigation, screen reader UX, and BFSG requirements.
argument-hint: "[product, feature, or component to audit]"
---

# /accessibility-audit

Run a comprehensive accessibility audit.

## Steps

1. **Scope**: Define what is being audited — which pages, flows, or components in $ARGUMENTS. Prioritise: authentication, checkout/core conversion flows, and navigation.
2. **Contrast audit**: Use the `color-contrast` skill to check all text, UI components, and graphical elements against WCAG 2.2 AA requirements.
3. **Keyboard audit**: Use the `keyboard-navigation` skill to verify full keyboard operability — tab order, focus visibility, component keyboard patterns.
4. **Focus management**: Use the `focus-management` skill to review modals, dynamic content, and SPA navigation.
5. **Screen reader review**: Use the `screen-reader-ux` skill to evaluate heading structure, landmark usage, alt text, and accessible names.
6. **ARIA review**: Use the `aria-patterns` skill to check ARIA usage on custom components — roles, states, properties, and live regions.
7. **BFSG check**: Use the `bfsg-compliance` skill to verify the accessibility statement exists and is complete, and that the feedback mechanism is in place.
8. **Report**: Produce an audit report with a WCAG criterion reference for each issue, severity rating (critical/major/minor), and remediation guidance.

## Output

Accessibility audit report with prioritised issues mapped to WCAG criteria, severity ratings, and actionable remediation steps.

Consider following up with `/accessibility:wcag-review` for a focused design-stage review, or `/accessibility:inclusive-review` for a broader disability-type coverage check.
