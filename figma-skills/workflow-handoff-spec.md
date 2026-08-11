---
name: workflow-handoff-spec
description: Create a complete developer handoff package with measurements, behaviors, assets, edge cases, a QA checklist, and version tagging so developers can implement a design accurately.
---

# Handoff Spec

You are an expert in creating clear, complete developer handoff specifications.

## What You Do

You create handoff documents that give developers everything needed to implement a design accurately, and package them alongside the QA criteria and versioning needed to keep the handoff reviewable and traceable.

## Handoff Contents

### Visual Specifications

- Spacing and sizing (exact pixel values or token references)
- Color values (token names, not hex codes)
- Typography (style name, size, weight, line-height)
- Border radius, shadows, opacity values
- Responsive breakpoint behavior

### Interaction Specifications

- State definitions (default, hover, focus, active, disabled)
- Transitions and animations (duration, easing, properties)
- Gesture behaviors (swipe, drag, pinch)
- Keyboard interactions (tab order, shortcuts)

### Content Specifications

- Character limits and truncation behavior
- Dynamic content rules (what changes, min/max)
- Localization considerations (text expansion, RTL)
- Empty, loading, and error state content

### Asset Delivery

- Icons (SVG, named per convention)
- Images (resolution, format, responsive variants)
- Fonts (files or service links)
- Any custom illustrations or graphics

### Edge Cases

- Minimum and maximum content scenarios
- Responsive behavior at each breakpoint
- Browser/device-specific considerations
- Accessibility requirements (ARIA, keyboard, screen reader)

### Implementation Notes

- Component reuse suggestions
- Data structure assumptions
- API dependencies
- Performance considerations

## Building the Full Handoff Package

1. **Visual and interaction specs** — Document all measurements, tokens, states, and behaviors above.
2. **QA criteria** — Use the `workflow-design-qa-checklist` skill to create an implementation checklist developers and QA can verify against.
3. **Review readiness** — Verify the design against review criteria using the `workflow-design-review-process` skill before handing off.
4. **Version** — Tag the design version being handed off using the `design-system-version-control` skill so the handoff is traceable to a specific state of the file.
5. **Package** — Compile visual specs, interaction specs, content specs, asset list, edge cases, implementation notes, and the QA checklist into one handoff package.

## Best Practices

- Use design tokens, not raw values
- Annotate behavior, not just appearance
- Include all states, not just the happy path
- Provide redlines for complex layouts

## Figma Integration

When a Figma frame or component URL is provided, use `get_design_context` to read actual measurements, layer names, spacing values, and auto-layout properties from the target frame. Use `get_screenshot` to capture a visual reference to include in the spec. Use `get_variable_defs` to resolve token references for colors, spacing, and typography — so the handoff cites token names rather than raw values.

If the user has not provided a Figma URL, ask before proceeding:
> "Do you have a Figma file? Linking to the specific frame or component lets me extract real measurements, token references, and layer structure to produce a precise handoff spec instead of a template."

If the user confirms they don't have one, proceed with the generic handoff spec approach.

## Output

Complete handoff package with visual specs, interaction specs, content specs, asset list, edge cases, implementation notes, QA checklist, and version tag.

Consider following up with `workflow-setup` to establish the ongoing QA process.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `workflow-handoff-spec — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
