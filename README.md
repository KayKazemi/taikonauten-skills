# Taikonauten Skills
Agentic skills, commands, and plugins for design — from research and strategy to brand identity, motion, accessibility, and delivery.
**90 skills** and **34 commands** across **12 plugins** for [Claude Code](https://docs.anthropic.com/en/docs/claude-code).
## Plugins
| Plugin | Skills | Commands | Description |
|--------|--------|----------|-------------|
| [design-research](./design-research) | 10 | 4 | User research: personas, empathy maps, journey maps, interviews, usability testing, and card sorting. |
| [design-systems](./design-systems) | 8 | 3 | Build and maintain design systems: tokens, components, accessibility, theming, and documentation. |
| [ux-strategy](./ux-strategy) | 9 | 3 | Shape product direction: competitive analysis, market positioning, design principles, experience mapping, and alignment. |
| [ui-design](./ui-design) | 9 | 4 | Craft polished interfaces: layout grids, color systems, typography, responsive design, and data viz. |
| [interaction-design](./interaction-design) | 7 | 3 | Design meaningful interactions: micro-animations, state machines, gestures, error handling, and feedback. |
| [prototyping-testing](./prototyping-testing) | 8 | 4 | Validate designs: prototyping strategies, usability testing, heuristic evaluation, and A/B experiments. |
| [design-ops](./design-ops) | 9 | 3 | Streamline operations: critique frameworks, handoff specs, sprint planning, client feedback, and revision workflows. |
| [designer-toolkit](./designer-toolkit) | 7 | 4 | Essential utilities: design rationale, presentations, pitch decks, case studies, UX writing, and system adoption. |
| [brand-identity](./brand-identity) | 7 | 3 | Build brand identities: strategy, visual systems, logo systems, guidelines, voice, and typographic identity. |
| [client-pitch](./client-pitch) | 6 | 3 | Win and manage client work: proposals, scoping, briefing, kickoff facilitation, pitch structure, and feedback. |
| [motion-design](./motion-design) | 6 | 3 | Design meaningful motion: principles, scroll animation, transition systems, hero animations, and brand motion. |
| [accessibility](./accessibility) | 7 | 3 | Design inclusively and meet legal standards: WCAG 2.2, screen reader UX, keyboard navigation, ARIA, and BFSG. |
## Quick Start

### Step 1: Add the Marketplace

In Claude Code, run:

```
/plugin marketplace add KayKazemi/taikonauten-skills
```

This registers the marketplace so you can browse and install individual plugins.

### Step 2: Install Plugins

Open the plugin manager and browse available plugins:

```
/plugin
```

Go to the **Discover** tab to see all 12 design plugins, then select and install the ones you want.

## What Are Skills and Commands?
- **Skills** are domain knowledge units (nouns). They teach Claude about a design topic — like creating user personas, defining design tokens, or writing error messages.
- **Commands** are workflows (verbs). They chain multiple skills together to accomplish a task — like running a full design system audit or planning a usability test.
## All Commands
| Command | Plugin | Description |
|---------|--------|-------------|
| `/design-research:discover` | design-research | Run a full user research discovery cycle. |
| `/design-research:interview` | design-research | Prepare and conduct a user interview. |
| `/design-research:test-plan` | design-research | Create a usability test plan. |
| `/design-research:synthesize` | design-research | Synthesize research data into insights. |
| `/design-systems:audit-system` | design-systems | Audit a design system for consistency and accessibility. |
| `/design-systems:create-component` | design-systems | Scaffold a full component specification. |
| `/design-systems:tokenize` | design-systems | Extract and organize design tokens. |
| `/ux-strategy:strategize` | ux-strategy | Develop a complete UX strategy. |
| `/ux-strategy:benchmark` | ux-strategy | Run a competitive benchmarking analysis. |
| `/ux-strategy:frame-problem` | ux-strategy | Structure an ambiguous challenge into a clear problem. |
| `/ui-design:design-screen` | ui-design | Design a complete screen layout. |
| `/ui-design:color-palette` | ui-design | Generate a full color palette with accessibility checks. |
| `/ui-design:type-system` | ui-design | Create a complete typography system. |
| `/ui-design:responsive-audit` | ui-design | Audit a design for responsive behavior. |
| `/interaction-design:design-interaction` | interaction-design | Design a complete interaction flow. |
| `/interaction-design:map-states` | interaction-design | Model states and transitions for a component. |
| `/interaction-design:error-flow` | interaction-design | Design error handling for a feature. |
| `/prototyping-testing:prototype-plan` | prototyping-testing | Create a prototyping and testing plan. |
| `/prototyping-testing:evaluate` | prototyping-testing | Run a heuristic evaluation. |
| `/prototyping-testing:test-plan` | prototyping-testing | Design a complete usability testing plan. |
| `/prototyping-testing:experiment` | prototyping-testing | Design an A/B experiment. |
| `/design-ops:plan-sprint` | design-ops | Plan a design sprint. |
| `/design-ops:handoff` | design-ops | Generate a developer handoff package. |
| `/design-ops:setup-workflow` | design-ops | Set up a design team workflow. |
| `/designer-toolkit:write-rationale` | designer-toolkit | Write design rationale for decisions. |
| `/designer-toolkit:build-presentation` | designer-toolkit | Structure a design presentation. |
| `/designer-toolkit:write-case-study` | designer-toolkit | Create a portfolio case study. |
| `/designer-toolkit:write-pitch` | designer-toolkit | Build a complete pitch deck for new business or a design proposal. |
| `/brand-identity:brand-audit` | brand-identity | Audit an existing brand for consistency and strategic clarity. |
| `/brand-identity:create-identity` | brand-identity | Create a complete visual identity from brand strategy. |
| `/brand-identity:define-voice` | brand-identity | Define brand voice, tone, and messaging framework. |
| `/client-pitch:write-proposal` | client-pitch | Write a complete client proposal from a brief. |
| `/client-pitch:run-kickoff` | client-pitch | Prepare and facilitate a project kickoff. |
| `/client-pitch:scope-project` | client-pitch | Define and document full project scope. |
| `/motion-design:design-motion` | motion-design | Design a complete motion system for a product. |
| `/motion-design:motion-audit` | motion-design | Audit existing motion for consistency and performance impact. |
| `/motion-design:animate-transition` | motion-design | Design transitions between specific states or pages. |
| `/accessibility:accessibility-audit` | accessibility | Run a full accessibility audit across a product or component. |
| `/accessibility:wcag-review` | accessibility | Review designs against WCAG 2.2 AA criteria. |
| `/accessibility:inclusive-review` | accessibility | Review designs across disability types for inclusive coverage. |
## Contributing
See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on adding new skills, commands, and plugins.
## License
MIT — see [LICENSE](./LICENSE).
