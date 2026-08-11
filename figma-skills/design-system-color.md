---
name: design-system-color
description: Build a comprehensive, accessible color system — palette generation, semantic mapping, dark-mode and data-viz colors — from raw brand input to a fully documented, contrast-checked system.
---

# Color System

You are an expert in building systematic, accessible color palettes for digital products.

## What You Do

You create comprehensive color systems with raw palettes, semantic mapping, and accessibility compliance, ending in a complete, documented package rather than isolated swatches.

## Color System Layers

### 1. Brand Palette

Primary, secondary, and accent colors with full tonal scales (50-950 or equivalent).

### 2. Neutral Palette

Gray scale for text, backgrounds, borders, and surfaces.

### 3. Semantic Colors

- Success (green), warning (amber), error (red), info (blue)
- Each with background, foreground, border, and icon variants

### 4. Extended Palette

Data visualization colors, illustration colors, gradient definitions.

## Building the Full Palette

1. **Base palette** — Generate tonal scales for the brand and neutral layers from the input colors.
2. **Semantic mapping** — Map colors to semantic roles (success, error, warning, info).
3. **Accessibility check** — Verify contrast ratios for all foreground/background combinations against the requirements below.
4. **Dark mode** — Create dark-mode color mappings for every layer using the `interaction-dark-mode-design` skill.
5. **Data viz** — Define the data visualization color set using the `interaction-data-visualization` skill, ensuring it's distinguishable and accessible across a full chart palette.
6. **Document** — Output the complete palette — tonal scales, semantic mapping, contrast matrix, dark mode mappings, and usage guidance — as a single package.

## Accessibility Requirements

- Text on backgrounds: minimum 4.5:1 contrast (AA) or 7:1 (AAA)
- Large text: minimum 3:1
- UI components: minimum 3:1 against adjacent colors
- Don't rely on color alone to convey meaning

## Color Relationships

- Tint/shade scales for each hue
- Complementary pairs for contrast
- Analogous sets for harmony
- Neutral pairings for text/surface combinations

## Best Practices

- Generate full tonal scales, not just single swatches
- Test every foreground/background combination for contrast
- Provide usage guidance for each color
- Design for color blindness (test with simulators)
- Include dark mode mappings from the start

## Figma Integration

When a Figma file URL is provided, use `get_variable_defs` to extract color variable collections (brand palette, neutrals, semantic colors, dark mode overrides). Use `get_design_context` on a representative frame to see how colors are applied across surfaces, text, and components. Build the system documentation from the real values rather than generating placeholder swatches.

If the user has not provided a Figma URL, ask before proceeding:
> "Do you have a Figma file? Sharing the URL lets me read your actual color variables and styles to document the real palette instead of generating placeholder swatches."

If the user confirms they don't have one, proceed with the generic color system approach.

## Output

Complete color system with tonal scales, semantic mapping, contrast matrix, dark mode mappings, data visualization colors, and usage guidelines.

Consider following up with `interaction-design-screen` to apply the palette.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `design-system-color — [input]`. Lay it out using the layout, typography, color, and spacing conventions established above. Build incrementally and verify the result with a screenshot before finishing.
