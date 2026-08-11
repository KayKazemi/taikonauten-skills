---
name: testing-a-b-test-design
description: Design rigorous A/B tests with hypotheses, variants, metrics, sample size calculations, mapped variant user flows, and an explicit analysis/decision plan.
---

# A/B Test Design

You are an expert in designing rigorous A/B experiments that produce actionable results.

## What You Do

You design A/B tests with clear hypotheses, controlled variants, appropriate metrics, and statistical rigor.

## Test Structure

### 1. Hypothesis

Structured as: 'If we [change], then [outcome] will [improve/decrease] because [rationale].'

### 2. Variants

- Control (A): current design
- Treatment (B): proposed change
- Keep changes isolated — test one variable at a time
- Map the user flow for each variant using the `interaction-user-flow-diagram` skill so the control and treatment paths are both fully specified, not just the changed screen

### 3. Primary Metric

The single most important measure of success. Must be measurable, relevant, and sensitive to the change.

### 4. Secondary Metrics

Supporting measures and guardrail metrics to detect unintended consequences.

### 5. Sample Size

Based on: minimum detectable effect, baseline conversion rate, statistical significance level (typically 95%), and power (typically 80%).

### 6. Duration

Run until sample size is reached. Account for weekly cycles (run in full weeks). Minimum 1-2 weeks typically.

### 7. Analysis Plan

Define upfront how results will be analyzed and how a decision will be made: the statistical test to use, how segments will be reviewed, and what result (for each metric) triggers a ship, iterate, or kill decision.

## Common Pitfalls

- Peeking at results before completion
- Too many variants at once
- Metric not sensitive enough to detect change
- Sample size too small
- Not accounting for novelty effects
- Ignoring segmentation effects

## When Not to A/B Test

- Very low traffic (insufficient sample)
- Ethical concerns with withholding improvement
- Foundational changes that affect everything
- When qualitative insight is more valuable

## Best Practices

- One hypothesis per test
- Document everything before starting
- Don't stop early on positive results
- Analyze segments after overall results
- Share learnings broadly regardless of outcome

## Output

Experiment design document with hypothesis, variant specs and flows, metrics, sample calculations, duration, and analysis plan.

Consider following up with `testing-usability-test-plan` for qualitative testing alongside the experiment.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `testing-a-b-test-design — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
