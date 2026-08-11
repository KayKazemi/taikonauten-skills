<div align="center">

# Design Skills

Design intelligence as standalone Figma custom skills.
Ask it to build your token system, write a component spec, run an accessibility audit,
structure a client pitch — and get output that reflects how designers actually think and work.

**112 flat skill files**

[Get started](#getting-started) · [Browse skills](#skills)

</div>

---

This repo is a flat collection of [Figma custom skills](https://agentskills.io/specification) for design work. Every file in [`/figma-skills`](./figma-skills) is a single, standalone `.md` file — no folders, no manifests, no plugin structure. Each one defines exactly one skill and is triggered directly by its filename.

Use only the files that match your discipline. You don't need everything.

Every skill ends with a `## Build` step that materializes its output as a tangible artifact instead of leaving it as chat text: UI/system/component skills and document-style skills (reports, personas, briefs, strategy docs) build a named frame on the current page via `figma-use`; flow/state-style skills build a FigJam board via `generate_diagram`.

---

## Getting Started

Point Figma's custom skills setting at this repository (or copy individual files) and add the `.md` files you want from [`/figma-skills`](./figma-skills). Each file is self-contained — drop in as many or as few as you need, with no extra setup, dependencies, or manifest to register.

---

## Skills

All 112 skills live flat in [`/figma-skills`](./figma-skills), grouped here by discipline for browsing. This repo previously shipped as a 12-plugin Claude Code marketplace; that structure has been fully retired in favor of Figma's flat custom-skill format, and the groupings below are just for navigation — every file is independent.

| Discipline | Example skills |
|---|---|
| Research | `research-user-persona`, `research-empathy-map`, `research-journey-map`, `research-interview-script`, `testing-usability-test-plan`, `research-card-sort-analysis` |
| Design Systems | `design-system-token`, `design-system-component-spec`, `design-system-naming-convention`, `design-system-pattern-library`, `design-system-icon`, `accessibility-audit` |
| UX Strategy | `strategy-competitive-analysis`, `strategy-market-positioning`, `strategy-design-principles`, `research-experience-map`, `workflow-stakeholder-alignment` |
| UI Design | `design-system-color`, `design-system-typography-scale`, `design-system-spacing`, `interaction-layout-grid`, `interaction-responsive-design`, `interaction-data-visualization` |
| Interaction Design | `motion-micro-interaction-spec`, `interaction-state-machine`, `interaction-gesture-patterns`, `interaction-error-handling-ux`, `interaction-visual-hierarchy` |
| Prototyping & Testing | `workflow-prototype-strategy`, `testing-heuristic-evaluation`, `testing-a-b-test-design`, `interaction-user-flow-diagram`, `interaction-wireframe-spec` |
| Design Ops | `workflow-handoff-spec`, `workflow-design-critique`, `workflow-design-sprint-plan`, `workflow-feedback-management`, `workflow-revision` |
| Designer Toolkit | `workflow-design-rationale`, `deliverables-presentation-deck`, `deliverables-case-study`, `interaction-ux-writing`, `design-system-adoption` |
| Brand Identity | `brand-strategy`, `brand-logo-system`, `brand-color-identity`, `brand-typography-identity`, `brand-voice` |
| Client Pitch | `deliverables-proposal-writing`, `workflow-project-scoping`, `workflow-client-brief`, `workflow-kickoff-facilitation`, `deliverables-pitch-deck` |
| Motion Design | `motion-principles`, `motion-scroll-animation`, `motion-transition-system`, `motion-hero-animation`, `motion-animate-transition` |
| Accessibility | `accessibility-wcag-compliance`, `accessibility-screen-reader-ux`, `accessibility-keyboard-navigation`, `accessibility-aria-patterns`, `accessibility-bfsg-compliance` |

Browse the full list in [`/figma-skills`](./figma-skills) — filenames are self-descriptive and match each skill's `name:` frontmatter.

---

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on adding or editing skills.

## License

MIT — see [LICENSE](./LICENSE).
