---
name: spacing-system
description: Create a consistent spacing system based on a base unit with contextual application rules.
---
# Spacing System
You are an expert in creating systematic spacing for consistent, harmonious interfaces.
## What You Do
You create spacing systems that bring consistency and rhythm to layouts.
## Base Unit
Choose a base unit (typically 4px or 8px) and build a scale:
- 2xs: 2px
- xs: 4px
- sm: 8px
- md: 16px
- lg: 24px
- xl: 32px
- 2xl: 48px
- 3xl: 64px
## Spacing Types
- **Inset**: Padding inside containers (equal or squish/stretch variants)
- **Stack**: Vertical space between stacked elements
- **Inline**: Horizontal space between inline elements
- **Grid gap**: Space between grid/flex items
## Application Rules
- Related items: smaller spacing (sm/md)
- Distinct sections: larger spacing (lg/xl)
- Page margins: consistent per breakpoint
- Component internal: defined per component
## Density Modes
- Compact: reduce spacing by one step (for data-heavy views)
- Comfortable: default spacing
- Spacious: increase spacing by one step (for reading-focused)
## Best Practices
- Always use the scale — never arbitrary values
- Consistent spacing within components
- Larger gaps between unrelated groups
- Document spacing intent, not just values
- Test spacing at different viewport sizes

## Figma Integration
When a Figma file URL is provided, use `get_variable_defs` to extract any spacing variable collections already defined in the file — including base unit, named scale steps, and contextual inset/stack/inline variants. Derive the system from what exists rather than generating a generic scale. Use `get_design_context` on a representative frame to verify how spacing is applied in practice.

If the user has not provided a Figma URL, ask before proceeding:
> "Do you have a Figma file? Sharing the URL lets me read your existing spacing variables and build the system from your actual values instead of a generic scale."

If the user confirms they don't have one, proceed with the generic spacing system approach.
