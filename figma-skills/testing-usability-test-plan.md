---
name: testing-usability-test-plan
description: Design a comprehensive usability test plan with research questions, methodology, participant criteria, persona-aligned tasks, metrics, and a facilitation guide — plus a live-prototype module for method selection, click/findability testing, and testing logistics. Use when planning moderated or unmoderated usability testing sessions.
---

# Usability Test Plan

Design a comprehensive usability test plan for evaluating designs and prototypes.

## Context

You are a senior UX researcher designing a usability test plan for $ARGUMENTS. If the user provides files (prototypes, designs, personas), read them first.

## Instructions

1. **Define objectives**: What specific questions should this test answer?
2. **Create the test plan** with:
   - **Research questions**: 3-5 specific questions to answer
   - **Methodology**: Moderated vs unmoderated, remote vs in-person, think-aloud protocol
   - **Participants**: Screening criteria, sample size (5-8 per segment), recruitment approach
   - **Tasks**: 5-8 realistic task scenarios with success criteria and expected completion time. If personas are available, align each task to a primary persona's goals and context rather than writing generic scenarios.
   - **Metrics**: Task success rate, time on task, error rate, SUS/SEQ scores, satisfaction rating
   - **Facilitation guide**: Script for introduction, task delivery, probing, and debrief
   - **Data collection**: What to record, observation template, note-taking framework
   - **Analysis plan**: How findings will be synthesized and prioritized
3. **Include a pilot test checklist**: What to verify before the real sessions.
4. Think step by step. Present in a ready-to-use format.

## If Testing a Live Prototype

When the test involves a working or high-fidelity prototype rather than static designs, add this module:

- **Method selection**: Use the `workflow-prototype-strategy` skill to choose the right testing approach for the prototype's fidelity and the questions being asked.
- **Click/findability tests**: Where navigation or information architecture is in question, use the `testing-click-test-plan` skill to design targeted click/findability tests alongside the moderated tasks.
- **Accessibility testing**: Include an accessibility pass using the `accessibility-test-plan` skill.
- **Logistics**: Give extra weight to participants, schedule, equipment, and facilitation logistics — live-prototype sessions have more that can go wrong technically than static-design reviews, so confirm device/browser setup, prototype link stability, and screen-recording tooling before the pilot.

## Output

Complete usability test plan with research questions, persona-aligned tasks, success metrics, participant criteria, facilitation guide, data collection plan, pilot checklist, and — where a live prototype is involved — method selection, click/findability tests, accessibility testing, and logistics.

Consider following up with `research-synthesize` to help analyse results after testing, or `research-interview-script` to prepare follow-up interview scripts, or `testing-evaluate` for an expert review before user testing.

## Build

Use the `figma-use` skill to materialize this as a new frame on the current page in the active Figma file, named `testing-usability-test-plan — [input]`. Lay it out as a polished one-page document: an eyebrow label, bold headline, and meta line at the top; numbered sections with clear typographic hierarchy; tables for structured or comparative data; and colored status badges or callout boxes to highlight key points, severity, or priority where relevant. Build incrementally and verify the result with a screenshot before finishing.
