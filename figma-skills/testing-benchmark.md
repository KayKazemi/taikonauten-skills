---
name: testing-benchmark
description: Run a competitive benchmarking analysis across a set of products.
argument-hint: "[list of competitor products or market category]"
---

# testing-benchmark

Run a structured competitive benchmarking analysis.

## Steps

1. **Identify** — Define competitors using `strategy-competitive-analysis` skill.
2. **Criteria** — Establish evaluation dimensions using `strategy-metrics-definition` skill.
3. **Analyze** — Deep-dive each competitor using `strategy-competitive-analysis` skill.
4. **Compare journeys** — Map experiences using `research-experience-map` skill.
5. **Score and rank** — Create comparison matrix.
6. **Opportunities** — Find gaps using `strategy-opportunity-framework` skill.
7. **Report** — Synthesize into actionable findings.

## Output

Benchmarking report with profiles, comparison matrix, journey comparisons, opportunity map, and recommendations.
Consider following up with `strategy-strategize` or `strategy-frame-problem`.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `testing-benchmark — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
