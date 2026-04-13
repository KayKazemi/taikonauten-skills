---
description: Write a complete client proposal from a brief or meeting notes.
argument-hint: "[client name, project type, and budget range]"
---

# /write-proposal

Write a complete client proposal.

## Steps

1. **Brief review**: Use the `client-brief` skill to extract and clarify the client's challenge, objectives, and success criteria from available inputs for $ARGUMENTS.
2. **Scope definition**: Use the `project-scoping` skill to define deliverables, phases, revision rounds, assumptions, and dependencies.
3. **Approach narrative**: Use the `pitch-structure` skill to shape the "our understanding" and "proposed approach" sections with a clear point of view.
4. **Timeline and investment**: Build a phase-by-phase timeline and present the investment clearly — itemised by phase if relevant.
5. **Draft full proposal**: Write all sections end-to-end using the `proposal-writing` skill. Executive summary is written last.
6. **Review**: Check for vague language, unsubstantiated claims, and any pricing ambiguity.

## Output

Complete proposal document ready for client delivery, including executive summary, understanding, approach, deliverables, timeline, investment, and next steps.

Consider following up with `/client-pitch:run-kickoff` once the proposal is accepted.
