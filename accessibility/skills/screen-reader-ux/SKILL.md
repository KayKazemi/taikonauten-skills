---
name: screen-reader-ux
description: Design semantic structure and reading order that creates a clear, logical experience for screen reader users. Use when designing page structure, content hierarchy, or interactive components.
---

# Screen Reader UX

Design interfaces that communicate meaning through structure and semantics — not just visual layout.

## What You Do

You help design teams think about how their interfaces are experienced by users who navigate by sound — using screen readers like NVDA, JAWS, or VoiceOver.

## Core Concepts

- **Semantic HTML**: The single biggest accessibility win. Use heading levels (`h1`–`h6`) to create a logical document outline. Use lists for list content. Use `<button>` for actions and `<a>` for navigation.
- **Reading order**: Screen readers follow DOM order, not visual order. Designs that rely on visual positioning (using absolute positioning or flex/grid reordering) can create non-linear reading order.
- **Accessible names**: Every interactive element needs a clear, descriptive accessible name. "Click here" and "Read more" fail. "Read more about pricing" passes.
- **Landmarks**: `<header>`, `<nav>`, `<main>`, `<aside>`, `<footer>` create navigation landmarks that screen reader users rely on to skip around the page.
- **Headings as navigation**: Many screen reader users navigate by heading — the heading structure should function as a table of contents for the page.

## Design Checklist

- [ ] Page has a single `<h1>` that describes the page purpose
- [ ] Heading levels are hierarchical — no skipped levels
- [ ] All images have meaningful alt text (or `alt=""` for decorative images)
- [ ] All form inputs have associated `<label>` elements
- [ ] All interactive elements have clear accessible names
- [ ] Reading order in the DOM matches the visual reading order
- [ ] Dynamic content changes (toasts, alerts) are announced via ARIA live regions

## Writing Alt Text

- Describe the function, not the appearance, for functional images
- Describe the content, not the format, for informational images
- Use `alt=""` for purely decorative images
- Maximum ~150 characters — longer descriptions use `aria-describedby`

## Further Reading

- WebAIM — Screen Reader User Survey
- Accessibility for Everyone — Laura Kalbag
