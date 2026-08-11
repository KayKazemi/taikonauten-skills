---
name: motion-principles
description: Apply core principles of motion design — timing, easing, choreography, continuity, and purpose — to create UI animation that feels intentional, natural, and brand-consistent. Use as the foundation for any motion design work.
---

# Motion Principles

Ground every animation decision in principles rather than aesthetics to create motion that is purposeful, performant, and coherent.

## What You Do

You help teams define and apply motion principles that make a product feel alive without being distracting — and that encode brand personality into how things move.

## Core Principles

- **Purpose**: Every animation should do one of: direct attention, communicate state, provide feedback, or convey personality. If it does none of these, remove it.
- **Timing/Duration**: Duration should match the weight and distance of the change.
  - Micro (50-100ms): button states, toggles
  - Short (150-250ms): tooltips, fades, small movements
  - Medium (250-400ms): page transitions, modals
  - Long (400-700ms): complex choreography
  - Avoid anything over 700ms in UI.
- **Easing**: Natural movement rarely moves at constant speed.
  - Ease-out: decelerating (entering elements) — fast start, soft landing
  - Ease-in: accelerating (exiting elements) — gentle start, fast exit
  - Ease-in-out: both (moving between positions)
  - Linear: only for continuous animations (progress bars)
- **Choreography**: Related elements should animate together. Stagger sequential items by 30-50ms each to create flow rather than chaos; lead with the most important element, use a consistent direction for related movements, and limit total sequence duration to under 700ms.
- **Continuity**: Motion should reinforce the spatial model of the interface — elements should move in ways that make sense given where they came from and where they're going.
- **Natural**: Follow physics (acceleration, deceleration).
- **Interruptible**: Animations can be cancelled mid-flight.

## Animation Types

- **Entrance**: fade in, slide in, scale up
- **Exit**: fade out, slide out, scale down
- **Emphasis**: pulse, shake, bounce
- **Transition**: morph, crossfade, shared element
- **Loading**: skeleton shimmer, spinner, progress

## The 12 Principles (Disney, adapted for UI)

Squash and stretch, anticipation, staging, straight-ahead vs pose-to-pose, follow through, slow in and slow out, arcs, secondary action, timing, exaggeration, solid drawing (solid form), appeal — applied proportionally to UI context.

## Accessibility

- Respect `prefers-reduced-motion` media query — always provide a non-animated fallback
- Avoid flashing content (WCAG 2.3.1: no more than 3 flashes per second)
- Do not use motion as the sole means of conveying information

## Best Practices

- Don't animate for the sake of it — if it fails the Purpose test above, cut it
- Test on low-powered devices
- Favor the shorter end of each duration band for anything on the critical interaction path
- Use will-change or transform for performance

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `motion-principles — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
