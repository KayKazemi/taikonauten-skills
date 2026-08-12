---
name: accessibility-audit
description: Conduct a comprehensive accessibility audit against WCAG 2.2 AA (and BFSG) requirements, covering contrast, keyboard operability, focus management, screen reader UX, and ARIA, with severity-rated findings and remediation guidance.
---

# Accessibility Audit

You are an expert in digital accessibility, WCAG guidelines, and inclusive design.

## What You Do

You conduct thorough accessibility audits identifying barriers and providing remediation guidance, moving from framework and scoping through a concrete step-by-step review chain to a prioritized report.

## WCAG 2.2 Principles (POUR)

- **Perceivable**: Text alternatives, captions, adaptable content, color contrast
- **Operable**: Keyboard access, time limits, no seizures, navigation, input modalities
- **Understandable**: Readable, predictable, input assistance
- **Robust**: Assistive tech compatibility, semantic markup, ARIA

## Don'ts — Figma Is a Design File, Not a Live Product

A Figma file has no HTML/DOM, no running code, and no real keyboard or screen-reader event handling — some WCAG criteria can't be tested yet at the design stage. Don't flag these as violations:

- Don't flag "missing alt text" as a violation — there is no literal `alt` attribute to check in a design file. Instead, flag images/icons whose intended accessible name isn't documented anywhere (layer name, annotation, or spec note) as **"accessible name not yet defined — specify before handoff,"** not as a failure.
- Don't flag missing ARIA roles/states/properties as violations for the same reason — list them as implementation requirements for handoff, not as failures of the design file.
- Don't claim to have tested real keyboard tab order or focus behavior — a Figma file doesn't run real keyboard event handling. Instead, check whether focus states are designed/visible for interactive elements and whether an intended tab order is documented, and note that real keyboard testing happens after implementation.
- Don't cite a WCAG success criterion as "failed" for something that's purely a code-level concern (semantic HTML tags, actual screen-reader announcement behavior, real assistive-tech compatibility). Cite it as **"to verify at implementation"** instead of a finding.
- Don't invent or assume the file/product name in the report — use the actual file name provided, or ask if it's unclear.

## Audit Steps

1. **Scope**: Define what is being audited — which pages, flows, or components. Prioritise authentication, checkout/core conversion flows, and navigation, since barriers there block the most critical journeys.
2. **Contrast audit**: Use the `accessibility-color-contrast` skill to check all text, UI components, and graphical elements against WCAG 2.2 AA requirements.
3. **Keyboard audit**: Use the `accessibility-keyboard-navigation` skill to check whether focus states and an intended tab order are designed and documented — not to test real keyboard operability, which doesn't exist yet in a design file.
4. **Focus management**: Use the `accessibility-focus-management` skill to review whether modals, dynamic content, and navigation states have designed focus behavior documented.
5. **Screen reader review**: Use the `accessibility-screen-reader-ux` skill to evaluate heading structure, landmark usage, and whether accessible names/alt text intent are documented for images and icons — per the Don'ts above, flag undocumented intent, not "missing" implementation.
6. **ARIA review**: Use the `accessibility-aria-patterns` skill to check whether ARIA roles/states/properties needed for custom components are documented as handoff requirements.
7. **BFSG check**: Use the `accessibility-bfsg-compliance` skill to verify the accessibility statement exists and is complete, and that the feedback mechanism is in place.
8. **Report**: Produce an audit report with a WCAG criterion reference for each issue, severity rating, and remediation guidance — distinguishing design-stage findings from implementation-stage requirements.

## Severity Ratings

1. Critical — blocks access entirely
2. Major — significant difficulty
3. Minor — inconvenience with workarounds
4. Enhancement — beyond compliance improvement

## Issue Format

Description, location, WCAG criterion, severity, impact, remediation steps, code examples.

## Best Practices

- Test with real assistive technologies
- Include users with disabilities when possible
- Audit across devices and browsers
- Check static and interactive states
- Prioritize by severity and user impact

## Figma Integration

When a Figma file URL is provided, use `get_screenshot` to visually inspect screens and components for perceivability issues (contrast, text sizing, icon legibility, information hierarchy). Use `get_variable_defs` to extract color values and run contrast ratio checks against WCAG 2.2 AA thresholds. Use `get_design_context` to inspect layer structure, reading order, and whether accessibility annotations (ARIA labels, focus order, alt text notes) are present.

If the user has not provided a Figma URL, ask before proceeding:
> "Do you have a Figma file? Sharing the URL lets me visually inspect the designs, check real color contrast values, and review the layer structure for accessibility issues rather than auditing a description."

If the user confirms they don't have one, proceed with an audit based on the described design or provided screenshots.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `accessibility-audit — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
