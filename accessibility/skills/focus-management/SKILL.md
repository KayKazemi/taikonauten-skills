---
name: focus-management
description: Define focus states, focus traps, skip navigation, and programmatic focus management for accessible interactive experiences. Use when designing modals, drawers, SPAs, or complex navigation patterns.
---

# Focus Management

Design and specify how focus moves through an interface — the most overlooked and most impactful accessibility discipline.

## What You Do

You help design teams plan focus behaviour for interactive patterns: where focus starts, where it goes when things open and close, and how to prevent it from getting lost.

## Focus State Design

Every interactive element must have a visible focus indicator that meets WCAG 2.2 AA (Success Criterion 2.4.11):
- Minimum focus indicator area: perimeter of the component × 2px
- Focus indicator must have 3:1 contrast against adjacent colours
- Focus indicator must not be entirely inside the component boundary

### Design Principles

- Design focus rings as part of the component token system — not as browser defaults
- Focus states should be visually distinct from hover states
- High-contrast mode must be considered — use `forced-colors: active` media query

## Focus Traps

A focus trap keeps keyboard focus within a container while it is open. Required for:
- Modal dialogs
- Drawers and side panels
- Cookie consent overlays
- Any overlay that blocks interaction with the page behind it

Specification:
- Focus moves to the first focusable element when the container opens
- Tab at the last element wraps to the first; Shift+Tab at the first wraps to the last
- Escape closes the container and returns focus to the element that triggered it

## Skip Navigation

"Skip to main content" links allow keyboard users to bypass navigation on every page load.
- Must be the first focusable element in the DOM
- Can be visually hidden until focused (using clip/transform, not `display: none`)
- Can include multiple skip links for complex layouts: "Skip to navigation", "Skip to search"

## SPA and Dynamic Content

In single-page applications, navigation does not trigger a page reload — focus management must be handled explicitly:
- On route change: move focus to the page heading or a landmark
- On modal open: move focus into the modal
- On toast/alert: announce via ARIA live region (do not move focus unless action is required)
- On content load: if content replaces a focused element, move focus to the new content

## Further Reading

- WCAG 2.4.3 — Focus Order
- WCAG 2.4.7 — Focus Visible
- WAI-ARIA Authoring Practices — Dialog Pattern
