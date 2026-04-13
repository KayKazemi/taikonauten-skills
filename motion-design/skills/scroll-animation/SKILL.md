---
name: scroll-animation
description: Design scroll-driven animations and parallax effects that enhance storytelling without hurting performance or accessibility. Use when designing marketing pages, editorial experiences, or immersive product presentations.
---

# Scroll Animation

Design scroll-driven motion that enhances narrative and spatial understanding — without becoming a performance or accessibility liability.

## What You Do

You help plan, specify, and evaluate scroll-driven animations — from subtle entrance effects to complex parallax storytelling.

## Scroll Animation Patterns

- **Entrance animations**: Elements fade, slide, or scale into view as they enter the viewport
- **Parallax depth**: Background and foreground layers move at different speeds to create depth
- **Scroll-linked progress**: Elements animate in proportion to scroll position (e.g., a progress bar, a morphing shape)
- **Sticky storytelling**: Elements pin in place while scroll drives their internal animation
- **Reveal and mask**: Content is progressively revealed as the user scrolls

## Design Specifications

For each scroll animation, specify:
- **Trigger**: At what scroll position does the animation begin?
- **Duration**: Over what scroll distance does it play out?
- **Easing**: What curve describes the motion?
- **Direction**: Vertical, horizontal, or both?
- **Delay**: Is there a stagger between related elements?
- **Reduced motion**: What is the non-animated fallback?

## Performance Considerations

- Animate only `opacity` and `transform` — these can be handled by the GPU without layout reflow
- Avoid animating `width`, `height`, `margin`, `padding`, or `top/left` — these trigger layout recalculation
- Use `will-change: transform` sparingly and only when needed
- Test on low-powered devices — scroll animations are often designed on fast machines and tested on them last

## Accessibility

- All content must be accessible without interaction — scroll animations are an enhancement, not a content gate
- `prefers-reduced-motion: reduce` must disable or simplify all scroll animations
- Do not require scrolling precision to trigger important content

## Further Reading

- Animation at Work — Rachel Nabors
- CSS Animations and the Web Animations API — MDN
