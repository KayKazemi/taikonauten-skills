---
name: aria-patterns
description: Apply ARIA roles, labels, properties, and live regions correctly to make custom interactive components accessible. Use when building or reviewing non-native interactive components.
---

# ARIA Patterns

Use ARIA correctly to communicate role, state, and property to assistive technologies when HTML semantics alone are insufficient.

## What You Do

You help design and development teams apply ARIA attributes correctly — and avoid the common mistake of using ARIA to fix problems that semantic HTML would solve better.

## The First Rule of ARIA

> "If you can use a native HTML element or attribute with the semantics and behaviour you require already built in, do that instead."

Use `<button>` instead of `<div role="button">`. Use `<nav>` instead of `<div role="navigation">`. ARIA is for cases where native HTML has no equivalent — not a shortcut.

## Key ARIA Concepts

- **role**: Defines what an element is (e.g., `role="dialog"`, `role="tab"`, `role="alert"`)
- **aria-label**: Provides an accessible name when visible text is absent or insufficient
- **aria-labelledby**: Points to an element whose text content becomes the accessible name
- **aria-describedby**: Points to supplementary description text
- **aria-hidden**: Removes an element from the accessibility tree (use for decorative icons)
- **aria-expanded**: Communicates open/closed state for accordions, dropdowns, menus
- **aria-selected**: Communicates selected state for tabs and listboxes
- **aria-checked**: Communicates checked state for custom checkboxes and switches
- **aria-disabled**: Communicates disabled state without removing from tab order
- **aria-live**: Creates a live region that announces dynamic content changes

## ARIA Live Regions

- `aria-live="polite"`: Announces update when user is idle. Use for: search results, notifications, status messages.
- `aria-live="assertive"`: Interrupts immediately. Use only for: errors, critical alerts.
- `role="status"`: Polite live region for status messages
- `role="alert"`: Assertive live region for errors and critical notices

## Common Component Patterns

- **Accordion**: `role="button"`, `aria-expanded`, `aria-controls`
- **Tabs**: `role="tablist"`, `role="tab"`, `role="tabpanel"`, `aria-selected`, `aria-controls`
- **Modal**: `role="dialog"`, `aria-modal`, `aria-labelledby`
- **Tooltip**: `role="tooltip"`, `aria-describedby`
- **Toggle/Switch**: `role="switch"`, `aria-checked`

## Further Reading

- WAI-ARIA Authoring Practices Guide — W3C
- Using ARIA — W3C Notes
