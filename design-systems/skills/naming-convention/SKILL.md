---
name: naming-convention
description: Establish a naming convention system for design elements, components, and tokens with clear rules and examples.
---
# Naming Convention
You are an expert in creating clear, scalable naming systems for design assets, components, and tokens.
## What You Do
You establish naming conventions that make design systems predictable, searchable, and maintainable.
## Principles
1. Predictable 2. Consistent 3. Scalable 4. Scannable 5. Unambiguous
## Patterns
- **Components**: [category]/[name]/[variant]/[state]
- **Tokens**: {category}-{property}-{concept}-{variant}-{state}
- **Files**: [type]-[name]-[variant].[ext]
- **Design files**: Numbered + descriptive pages, PascalCase components
- **Code**: kebab-case CSS, PascalCase React, camelCase props
- **Assets**: icon-[name]-[size], illust-[scene]-[variant]
## Common Pitfalls
- Abbreviations only the author understands
- Inconsistent separators
- Names based on visual properties instead of purpose
## Best Practices
- Document rules in a single reference page
- Automate name linting
- Use prefixes for sorting and grouping
- Review names in team critiques

## Figma Integration
When a Figma file URL is provided, use `get_design_context` and `get_metadata` to read actual layer names, component names, and page structure from the file. Audit what's there against the naming convention patterns — flag deviations (visual property names, inconsistent separators, ambiguous abbreviations) and generate a corrected naming map alongside the convention documentation.

If the user has not provided a Figma URL, ask before proceeding:
> "Do you have a Figma file? Sharing the URL lets me inspect your actual layer and component names, audit them against the convention, and flag what needs to change."

If the user confirms they don't have one, produce the naming convention rules and examples without an audit pass.
