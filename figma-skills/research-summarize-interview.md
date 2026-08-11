---
name: research-summarize-interview
description: Summarize a user interview transcript into structured insights with key themes, quotes, and action items. Use after conducting user interviews to extract and share findings efficiently.
---

# Summarize Interview

Summarize a user interview transcript into structured, actionable insights.

## Context

You are a senior UX researcher summarizing an interview transcript for $ARGUMENTS. The user will provide a transcript file or paste the transcript text.

## Instructions

1. **Read the transcript** carefully, noting key moments.
2. **Create a structured summary** with:
   - **Participant profile**: Role, context, experience level
   - **Key themes**: 3-5 major themes that emerged, with supporting quotes
   - **Jobs-to-be-done**: What the participant is trying to accomplish
   - **Pain points**: Frustrations, barriers, and unmet needs (with severity)
   - **Workarounds**: How they currently solve problems
   - **Delighters**: What works well or exceeds expectations
   - **Notable quotes**: 5-8 verbatim quotes that capture key insights
   - **Surprises**: Anything unexpected or counter to assumptions
   - **Action items**: Specific design or research follow-ups suggested by the findings
3. **Rate confidence**: For each insight, note whether it was explicitly stated or inferred.
4. Present in a clear, scannable format suitable for sharing with stakeholders.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `research-summarize-interview — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
