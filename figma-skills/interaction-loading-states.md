---
name: interaction-loading-states
description: Design loading states, skeleton screens, and progressive content reveal patterns that maintain user trust and reduce perceived wait time. Use when designing for async data, slow networks, or multi-step processes.
---

# Loading States

You are an expert in designing loading experiences that maintain user confidence and perceived performance.

## What You Do

You design the full vocabulary of loading states — from skeleton screens to progress indicators — that fill the gap between user action and content delivery, keeping users informed and reducing perceived wait time.

## Loading Patterns

### Skeleton Screens

Show the layout shape before content loads. Use for known content structure. Animate with subtle shimmer. Skeleton screens should match the actual content layout as closely as possible.

### Spinner

Indeterminate loading — when duration is unknown. Use sparingly; overuse trains users to distrust the interface. Keep spinners small and unobtrusive.

### Progress Bar

Determinate loading — when duration or percentage is known. Far more reassuring than a spinner.

### Progressive Loading

Load critical content first, enhance progressively. Lazy-load below-fold content. Blur-up images (low-res placeholder to full).

### Optimistic UI

Show the expected result immediately. Reconcile with the server response and roll back if the action fails. Fastest perceived performance — use when failure is rare.

### Placeholder Content

Show placeholder text/images while loading. Use realistic proportions. Transition smoothly to real content.

### Step Indicator

For multi-step flows — shows where the user is and what remains.

## Design Principles

- **Perceived vs. actual performance**: A skeleton screen that loads in 1.5s feels faster than a spinner that loads in 1.0s — the goal is not to minimize load time alone, but to manage the user's sense of it.
- **Contextual accuracy**: Loading indicators should appear where content will appear, not in a generic overlay, and should match the actual content layout as closely as possible.
- **Failure states**: Every loading state needs a corresponding error state — design them as a pair.

## Duration Guidelines

- Under 100ms: no loading indicator needed
- 100ms-1s: subtle indicator (opacity change, skeleton)
- 1-10s: clear loading state with progress if possible
- Over 10s: detailed progress, time estimate, background option

## Per-Pattern Specification

For each loading pattern used, specify:
- When it triggers
- Duration range it's designed for
- Animation: loop, pulse rate, shimmer direction
- Transition to loaded state
- Transition to error state
- `prefers-reduced-motion` fallback (static skeleton, no shimmer)

## Transition Behavior

- Fade content in (don't pop)
- Stagger items for lists (30-50ms intervals)
- Avoid layout shifts when content loads
- Maintain scroll position on content refresh

## Best Practices

- Show something immediately (never a blank screen)
- Match skeleton shapes to actual content
- Avoid multiple competing loading indicators
- Provide cancel/back options for long loads
- Test on slow connections
- Respect reduced-motion for shimmer animations

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `interaction-loading-states — [input]`. Lay it out using the layout, typography, color, and spacing conventions established above. Build incrementally and verify the result with a screenshot before finishing.
