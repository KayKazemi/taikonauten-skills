---
name: keyboard-navigation
description: Design keyboard-first interaction patterns that allow full navigation without a mouse. Use when designing interactive components, forms, or navigation systems.
---

# Keyboard Navigation

Design interfaces that work completely without a mouse — essential for motor-impaired users, power users, and switch access users.

## What You Do

You help ensure that every interaction in a design can be completed using only a keyboard, following established navigation conventions that users have learned.

## Keyboard Navigation Conventions

- **Tab**: Move focus to the next interactive element
- **Shift+Tab**: Move focus to the previous interactive element
- **Enter**: Activate a focused link or button
- **Space**: Toggle a checkbox; activate a button
- **Arrow keys**: Navigate within a component (menus, tabs, radio groups, sliders)
- **Escape**: Close a modal, dismiss a popover, cancel an action
- **Home/End**: Jump to first/last item in a list or menu

## Tab Order Principles

- Tab order must follow a logical, predictable sequence — typically left-to-right, top-to-bottom in LTR layouts
- Skip links ("Skip to main content") allow keyboard users to bypass repetitive navigation
- `tabindex="0"` adds an element to the natural tab order
- `tabindex="-1"` removes from tab order but allows programmatic focus
- Avoid positive `tabindex` values — they override natural order and create confusion

## Component-Level Patterns

- **Menus and dropdowns**: Arrow keys navigate items; Escape closes
- **Modal dialogs**: Focus must move into the modal on open; Tab is trapped within the modal; Escape closes; focus returns to the trigger on close
- **Tabs**: Arrow keys switch between tab panels; Tab moves focus into the active panel
- **Sliders**: Arrow keys increment/decrement; Home/End for min/max

## Designing Visible Focus

All interactive elements need a visible focus state that meets WCAG 2.2 AA (2.4.11). A 2px outline with 3:1 contrast against adjacent colours is the minimum. Design focus states as part of the component, not as an afterthought.

## Further Reading

- WCAG 2.2 — 2.1 Keyboard Accessible
- WAI-ARIA Authoring Practices Guide — W3C
