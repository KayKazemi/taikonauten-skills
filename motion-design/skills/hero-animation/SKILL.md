---
name: hero-animation
description: Design hero section and entry animations that make a strong first impression and establish the brand's motion character. Use for marketing pages, product launches, and brand moments.
---

# Hero Animation

Design the opening animation that sets the tone for everything that follows.

## What You Do

You help conceive, specify, and evaluate hero animations — the first animated moment a user encounters, which does more to establish brand perception than any other single motion decision.

## Hero Animation Types

- **Cinematic reveal**: Content fades or scales into view with careful choreography
- **Type animation**: Headlines appear character by character, word by word, or line by line
- **Looping ambient**: A subtle, continuous animation that adds life without demanding attention
- **Scroll-activated story**: The hero animation is driven by initial scroll, drawing the user in
- **Video or lottie hero**: A produced animation or video that plays on load

## Design Considerations

- **Instant value**: The hero must communicate value before the animation completes — key messages should be legible within 1 second
- **Performance**: Hero animations run on first load — they must not delay LCP (Largest Contentful Paint). Target under 2.5s LCP.
- **Brand fidelity**: The motion language should feel like an extension of the brand's personality, not a template effect
- **Loop quality**: If the animation loops, the loop point should be invisible
- **Mobile parity**: Define the mobile variant — complex hero animations often need simplified versions for small screens

## Specification

- Storyboard or frame-by-frame description of the animation sequence
- Duration and timing for each element
- Easing for each motion
- Fallback for `prefers-reduced-motion`
- Performance budget (KB for any animation assets)
