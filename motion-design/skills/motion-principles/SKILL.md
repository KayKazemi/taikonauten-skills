---
name: motion-principles
description: Apply core principles of motion design — timing, easing, choreography, and purpose — to create animation that feels intentional and brand-consistent. Use as the foundation for any motion design work.
---

# Motion Principles

Ground every animation decision in principles rather than aesthetics to create motion that is purposeful, performant, and coherent.

## What You Do

You help teams define and apply motion principles that make a product feel alive without being distracting — and that encode brand personality into how things move.

## Core Principles

- **Purpose**: Every animation should do one of: direct attention, communicate state, provide feedback, or convey personality. If it does none of these, remove it.
- **Timing**: Duration should match the weight and distance of the change. Micro-interactions: 100–200ms. Page transitions: 300–500ms. Avoid anything over 700ms in UI.
- **Easing**: Natural movement rarely moves at constant speed. Ease-out for entering elements (fast start, soft landing). Ease-in for exiting elements (gentle start, fast exit). Ease-in-out for moving elements.
- **Choreography**: Related elements should animate together. Stagger sequential elements to create flow rather than chaos.
- **Continuity**: Motion should reinforce the spatial model of the interface — elements should move in ways that make sense given where they came from and where they're going.

## The 12 Principles (Disney, adapted for UI)

Squash and stretch, anticipation, staging, straight-ahead vs pose-to-pose, follow through, slow in and slow out, arcs, secondary action, timing, exaggeration, solid drawing (solid form), appeal — applied proportionally to UI context.

## Accessibility

- Respect `prefers-reduced-motion` media query — always provide a non-animated fallback
- Avoid flashing content (WCAG 2.3.1: no more than 3 flashes per second)
- Do not use motion as the sole means of conveying information

## Further Reading

- The Illusion of Life — Frank Thomas & Ollie Johnston
- Animation at Work — Rachel Nabors
