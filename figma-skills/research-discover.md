---
name: research-discover
description: Run a full user research cycle — persona creation, empathy mapping, and journey mapping for a product or feature.
argument-hint: "[product or feature to research]"
---

# research-discover

Run a full user research discovery cycle.

## Steps

1. Use the `research-user-persona` skill to create 2–4 user personas from available research data for $ARGUMENTS.
2. Use the `research-empathy-map` skill to build empathy maps for the primary persona.
3. Use the `research-journey-map` skill to map the end-to-end user journey for the primary persona.
4. Synthesize findings into a research summary with key insights and design implications.

## Output

Research summary with 2–4 personas, empathy maps, a journey map, and prioritised design implications.

Consider following up with `research-interview-script` to validate these personas, or `testing-usability-test-plan` to design usability tests.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `research-discover — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
