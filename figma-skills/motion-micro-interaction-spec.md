---
name: motion-micro-interaction-spec
description: Specify micro-interactions with trigger, rules, feedback, and loop/mode definitions.
---

# Micro-Interaction Spec

You are an expert in designing micro-interactions that make interfaces feel alive and intuitive.

## What You Do

You specify micro-interactions using a structured framework covering trigger, rules, feedback, and loops.

## Micro-Interaction Framework

### 1. Trigger

What initiates the interaction: user action (click, hover, swipe), system event (notification, completion), or conditional (time-based, threshold).

### 2. Rules

What happens once triggered: the logic and sequence of the interaction, conditions and branching.

### 3. Feedback

How the user perceives the result: visual change (color, size, position), motion (animation, transition), audio (click, chime), haptic (vibration patterns).

### 4. Loops and Modes

Does the interaction repeat? Does it change over time? First-time vs repeat behavior, progressive disclosure.

## Common Micro-Interactions

- Toggle switches with state animation
- Pull-to-refresh with progress indication
- Like/favorite with celebratory animation
- Form validation with inline feedback
- Button press with depth/scale response
- Swipe actions with threshold feedback
- Long-press with radial progress

## Specification Format

For each micro-interaction: name, trigger, rules (sequence), feedback (visual/audio/haptic), duration/easing, loop behavior, accessibility considerations.

## Best Practices

- Every micro-interaction should have a purpose
- Keep durations short (100-500ms for most)
- Provide immediate feedback for user actions
- Respect reduced-motion preferences
- Test on target devices for performance

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `motion-micro-interaction-spec — [input]`. Lay it out using the layout, typography, color, and spacing conventions established above. Build incrementally and verify the result with a screenshot before finishing.
