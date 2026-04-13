---
name: loading-animation
description: Design loading states, skeleton screens, and progress animations that maintain user trust and reduce perceived wait time. Use when designing for async data, slow networks, or multi-step processes.
---

# Loading Animation

Design loading states that keep users oriented and confident during wait times.

## What You Do

You help design the full vocabulary of loading states — from skeleton screens to progress indicators — that fill the gap between user action and content delivery.

## Loading Pattern Types

- **Spinner**: Indeterminate loading — when duration is unknown. Use sparingly; overuse trains users to distrust the interface.
- **Progress bar**: Determinate loading — when duration or percentage is known. Far more reassuring than a spinner.
- **Skeleton screen**: A low-fidelity representation of the content layout that appears while content loads. Reduces perceived wait time vs. a blank state.
- **Optimistic UI**: Show the result of an action immediately and revert on failure. Fastest perceived performance — use when failure is rare.
- **Shimmer / pulse**: Animated skeleton effect that signals activity without implying completion.
- **Step indicator**: For multi-step flows — shows where the user is and what remains.

## Design Principles

- **Perceived vs. actual performance**: A skeleton screen that loads in 1.5s feels faster than a spinner that loads in 1.0s
- **Contextual accuracy**: Skeleton screens should match the actual content layout as closely as possible
- **Consistent placement**: Loading indicators should appear where content will appear, not in a generic overlay
- **Failure states**: Every loading state needs a corresponding error state — design them as a pair

## Specification

For each loading pattern:
- When it triggers
- Duration range it's designed for
- Animation: loop, pulse rate, shimmer direction
- Transition to loaded state
- Transition to error state
- `prefers-reduced-motion` fallback (static skeleton, no shimmer)

## Further Reading

- "The Psychology of Waiting" — David Maister
- Designing for Performance — Lara Callender Hogan
