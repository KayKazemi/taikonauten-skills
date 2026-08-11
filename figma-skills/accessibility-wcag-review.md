---
name: accessibility-wcag-review
description: Review designs against WCAG 2.2 AA criteria at the design stage, before development begins.
argument-hint: "[design file, screen, or component to review]"
---

# accessibility-wcag-review

Review designs for WCAG 2.2 AA conformance before handoff.

## Steps

1. **Contrast check**: Use the `accessibility-color-contrast` skill to verify all text/background combinations and UI component boundaries for $ARGUMENTS.
2. **Focus states**: Use the `accessibility-focus-management` skill to confirm that all interactive elements have a visible, compliant focus indicator designed.
3. **Keyboard patterns**: Use the `accessibility-keyboard-navigation` skill to verify that component behaviour follows established keyboard conventions.
4. **Accessible names**: Use the `accessibility-screen-reader-ux` skill to check that all interactive elements have meaningful labels — not "icon", "button", or "click here".
5. **Heading structure**: Verify the page heading hierarchy is logical and complete.
6. **ARIA requirements**: Use the `accessibility-aria-patterns` skill to identify any custom components that will require ARIA attributes and specify them.
7. **Motion and animation**: Check that any animations have a non-animated fallback for users with `prefers-reduced-motion: reduce` enabled. Flag any missing fallbacks as accessibility issues.
8. **Document findings**: Annotate the design with accessibility specs and a list of any items that need attention before handoff.

## Output

Annotated design review with accessibility specs and a checklist of WCAG 2.2 AA pass/fail items, ready for developer handoff.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `accessibility-wcag-review — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
