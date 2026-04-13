---
name: color-contrast
description: Ensure accessible color contrast ratios across all UI states and text sizes. Use when defining a color system or auditing an existing design for contrast compliance.
---

# Color Contrast

Ensure that text, UI components, and visual information are legible for users with low vision and colour deficiencies.

## What You Do

You help evaluate and fix color contrast across a design — checking text, interactive components, icons, and data visualisation against WCAG requirements.

## Contrast Ratios (WCAG 2.2 AA)

- **Normal text** (< 18pt / 14pt bold): minimum **4.5:1**
- **Large text** (≥ 18pt / 14pt bold): minimum **3:1**
- **UI components and graphical objects**: minimum **3:1** against adjacent color
- **Decorative elements**: no requirement
- **Disabled components**: no requirement (but consider usability)

## Enhanced (AAA)

- Normal text: 7:1
- Large text: 4.5:1

## Common Failure Patterns

- Light grey text on white backgrounds
- Placeholder text in form inputs (often 40% opacity — usually fails)
- Disabled button states that become unreadable
- Text on photographic backgrounds without a scrim
- Coloured text on coloured backgrounds (e.g., brand blue on brand yellow)
- Focus indicators with insufficient contrast against the focused element

## Color Blindness Considerations

- Never use color alone to convey information — always pair with shape, pattern, or text
- Deuteranopia (red-green): affects ~8% of males. Red/green combinations are indistinguishable.
- Protanopia: similar to deuteranopia
- Tritanopia (blue-yellow): less common

## Tools

- Colour Contrast Analyser (desktop tool)
- WebAIM Contrast Checker
- Figma plugins: Contrast, Stark, A11y - Color Contrast Checker
- Simulator: Sim Daltonism (macOS)

## Further Reading

- WCAG 2.2 Success Criterion 1.4.3 — Contrast (Minimum)
- Accessible Colors — clrs.cc
