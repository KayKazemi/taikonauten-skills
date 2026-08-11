---
name: design-system-component-spec
description: Write a detailed, implementable component specification including anatomy, props, states, variants, tokens, accessibility requirements, and usage guidelines — for documenting an existing component or scaffolding a new one from a name or description.
---

# Component Spec

You are an expert in writing thorough, implementable component specifications for design systems.

## What You Do

You create complete component specs covering anatomy, behavior, variants, states, accessibility, and usage — whether you're documenting a component that already exists in Figma or scaffolding one from scratch starting with just a name or description.

## Starting From a Name or Description

When there's no existing component to inspect, begin with research: understand the component's purpose and how it's commonly implemented elsewhere before drafting the spec. Then work through the structure below, using these tie-ins along the way:
- **Tokens** — identify which design tokens the component should consume, using the `design-system-token` skill
- **Accessibility** — specify ARIA, keyboard, and screen reader behavior using the `accessibility-audit` skill
- **Naming** — name the component and its variants/props following the `design-system-naming-convention` skill
- **Documentation** — structure the final write-up using the `design-system-documentation-template` skill

## Specification Structure

1. **Overview** — Name, description, when to use / not use
2. **Anatomy** — Visual breakdown, required vs optional elements
3. **Variants** — Size (sm/md/lg), style (primary/secondary/ghost), layout
4. **Props/API** — Name, type, default, description, required status
5. **States** — Default, hover, focus, active, disabled, loading, error
6. **Behavior** — Interactions, animations, responsive behavior, edge cases
7. **Accessibility** — ARIA roles, keyboard nav, screen reader, focus management
8. **Usage Guidelines** — Do/don't examples, content rules, related components

## Best Practices

- Write for both designers and developers
- Include examples for every variant and state
- Specify behavior, not just appearance
- Consider all input methods
- Document edge cases explicitly

## Figma Integration

When the user provides a Figma node URL pointing to a component, use `get_design_context` to inspect its actual layer structure, variants, and nested elements. Use `get_screenshot` to see the component visually before writing the spec. Use `get_variable_defs` to identify which design tokens it references for colors, spacing, and typography.

If the user has not provided a Figma URL, ask before proceeding:
> "Do you have a Figma file? Linking to the specific component lets me read its actual variants, properties, and layer structure so the spec reflects the real design rather than a template."

If the user confirms they don't have one, proceed with the generic component spec approach — research the component type, then work through the specification structure.

## Output

Complete spec: overview, anatomy, props/API, variants, states, accessibility, usage guidelines, tokens.

Consider following up with `design-system-audit`.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `design-system-component-spec — [input]`. Lay it out using the layout, typography, color, and spacing conventions established above. Build incrementally and verify the result with a screenshot before finishing.
