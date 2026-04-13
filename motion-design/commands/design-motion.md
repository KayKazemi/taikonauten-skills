---
description: Design a complete motion system for a product, from principles through to a motion token set and pattern library.
argument-hint: "[product name and brand personality description]"
---

# /design-motion

Design a complete motion system end-to-end.

## Steps

1. **Motion principles**: Use the `motion-principles` skill to define 3–4 guiding principles that reflect the brand's personality for $ARGUMENTS.
2. **Brand motion language**: Use the `brand-motion` skill to establish the motion DNA — characteristic easing, timing philosophy, choreography style, and signature animated moments.
3. **Transition system**: Use the `transition-system` skill to define motion tokens (duration and easing scales) and the full vocabulary of page and component transitions.
4. **Loading states**: Use the `loading-animation` skill to design the loading state vocabulary — skeleton screens, spinners, progress, and optimistic UI patterns.
5. **Accessibility**: Define the `prefers-reduced-motion` policy and list every animation with its fallback behaviour.
6. **Documentation**: Compile into a motion guidelines document: principles, token system, pattern library, and anti-patterns.

## Output

Motion system documentation: principles, motion tokens, transition vocabulary, loading pattern library, and accessibility policy.

Consider following up with `/motion-design:animate-transition` to spec individual transitions, or `/motion-design:motion-audit` to validate existing motion against the system.
