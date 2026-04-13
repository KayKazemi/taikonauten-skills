---
description: Design the motion for a specific transition between states, screens, or components.
argument-hint: "[describe the transition, e.g. 'product card expanding to detail view']"
---

# /animate-transition

Design the motion spec for a specific transition.

## Steps

1. **Understand the spatial context**: Describe the spatial relationship between the origin and destination for $ARGUMENTS — where is the user coming from, where are they going?
2. **Select the transition pattern**: Use the `transition-system` skill to identify the appropriate transition category (page, modal, list, in-place, shared element).
3. **Design the choreography**: Define enter and exit behaviour for all involved elements — what moves, what fades, what stays still.
4. **Specify timing**: Select duration and easing values from the motion token system. Justify any deviations.
5. **Scroll or hero context**: If scroll-driven, use the `scroll-animation` or `hero-animation` skill to apply relevant constraints and specifications.
6. **Accessibility**: Define the `prefers-reduced-motion` fallback explicitly.
7. **Handoff spec**: Write the complete motion spec — element-by-element, with duration, easing, delay, and trigger — ready for developer implementation.

## Output

Complete motion specification for the transition: choreography description, timing values, easing values, and reduced-motion fallback.
