---
description: Audit an existing brand for consistency, strategic clarity, and visual coherence.
argument-hint: "[brand name or URL to audit]"
---

# /brand-audit

Audit an existing brand end-to-end.

## Steps

1. **Gather materials**: Collect existing logo files, brand guidelines, website, social profiles, and marketing materials for $ARGUMENTS.
2. **Strategy audit**: Use the `brand-strategy` skill to evaluate whether the brand's purpose, values, and positioning are clearly defined and differentiated.
3. **Visual audit**: Use the `visual-identity` skill to assess consistency across logo, color, typography, and imagery across all touchpoints.
4. **Logo review**: Use the `logo-system` skill to check for variant completeness, misuse patterns, and reproduction quality.
5. **Voice audit**: Use the `brand-voice` skill to evaluate tone consistency across all communication channels.
6. **Accessibility check**: Flag any color combinations or type sizes that fail WCAG 2.2 AA contrast requirements.
7. **Consolidate findings**: Produce an audit report with a RAG (Red/Amber/Green) rating per area, top 3 strengths, and top 3 priority fixes.

## Output

Brand audit report with RAG ratings, key strengths, priority issues, and recommended next steps.

Consider following up with `/brand-identity:create-identity` to address visual gaps or `/brand-identity:define-voice` to address communication gaps.
