---
name: transition-system
description: Define a systematic approach to page and component transitions that creates a coherent sense of spatial navigation. Use when building or auditing the motion layer of a product.
---

# Transition System

Define transitions that make navigation feel spatial and coherent — not just decorative.

## What You Do

You help design and document a transition system — the set of motion patterns that govern how screens, panels, modals, and components enter and exit.

## Transition Categories

- **Page transitions**: Moving between top-level routes
- **Modal and overlay transitions**: Sheets, dialogs, and drawers entering and exiting
- **List and card transitions**: Items entering, leaving, or reordering within a list
- **In-place transitions**: Content changing within a static container (e.g., tab content, form step)
- **Shared element transitions**: An element from one screen becomes an element in the next (hero transitions)

## Transition Vocabulary

For each category, define:
- **Enter**: How does the element arrive? (Direction, scale, opacity)
- **Exit**: How does it leave? (Should mirror enter or have its own logic)
- **Duration**: In milliseconds
- **Easing**: Named easing from the motion token system
- **Trigger**: What user action initiates it?

## Spatial Model Principles

- Forward navigation (going deeper): new content typically enters from the right or bottom
- Backward navigation (going back): exiting content should leave in the opposite direction
- Overlays (modals, drawers): should feel layered — enter from the direction they're conceptually attached to
- Avoid arbitrary directions that break the spatial model

## Motion Token System

Define a small set of named motion tokens:
- `duration-fast`: 150ms — micro-interactions, hovers
- `duration-base`: 250ms — component transitions
- `duration-slow`: 400ms — page and modal transitions
- `ease-enter`: cubic-bezier(0.0, 0.0, 0.2, 1) — ease-out
- `ease-exit`: cubic-bezier(0.4, 0.0, 1, 1) — ease-in
- `ease-move`: cubic-bezier(0.4, 0.0, 0.2, 1) — ease-in-out
