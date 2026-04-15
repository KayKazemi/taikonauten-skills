<div align="center">

# Taikonauten Skills

Design intelligence for Claude Code.
Ask it to build your token system, write a component spec, run an accessibility audit,
structure a client pitch — and get output that reflects how designers actually think and work.

**90 skills · 34 commands · 12 plugins**

[Get started](#getting-started) · [Browse plugins](#plugins) · [Connect Figma](#figma-integration) · [All commands](#commands)

</div>

---

This is a plugin collection for [Claude Code](https://docs.anthropic.com/en/docs/claude-code). Each **skill** is a concentrated unit of design expertise — not generic AI output. Each **command** chains skills into a complete workflow you can run in one line.

Install only the plugins that match your discipline. You don't need everything.

---

## Getting Started

Two steps. Under a minute.

**1 — Add the marketplace**

```
/plugin marketplace add KayKazemi/taikonauten-skills
```

**2 — Install what you need**

```
/plugin
```

Open the **Discover** tab, browse all 12 plugins, and install the ones relevant to your work.

---

## Plugins

<table>
<tr>
<td width="50%" valign="top">

### Research
[design-research](./design-research) · 10 skills · 4 commands

Build your research foundation. Personas, empathy maps, journey maps, interview scripts, usability test plans, card sort analysis. Start a project right.

</td>
<td width="50%" valign="top">

### Design Systems
[design-systems](./design-systems) · 8 skills · 3 commands

Define the source of truth. Design tokens, component specs, naming conventions, pattern libraries, icon systems, accessibility auditing. Connect directly to Figma variables.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### UX Strategy
[ux-strategy](./ux-strategy) · 9 skills · 3 commands

Shape what gets built. Competitive analysis, market positioning, design principles, experience mapping, stakeholder alignment. Frame the problem before solving it.

</td>
<td width="50%" valign="top">

### UI Design
[ui-design](./ui-design) · 9 skills · 4 commands

Craft the visual layer. Color systems, typography scales, spacing systems, layout grids, responsive design, data visualization. Ground every decision in a system.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Interaction Design
[interaction-design](./interaction-design) · 7 skills · 3 commands

Design what happens between states. Micro-interaction specs, state machines, gesture patterns, error handling, animation principles, loading patterns.

</td>
<td width="50%" valign="top">

### Prototyping & Testing
[prototyping-testing](./prototyping-testing) · 8 skills · 4 commands

Validate before you ship. Prototype strategies, usability testing, heuristic evaluation, A/B experiments, user flow diagrams, wireframe specs.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Design Ops
[design-ops](./design-ops) · 9 skills · 3 commands

Keep the work moving. Handoff specs, critique frameworks, sprint planning, feedback management, revision workflows, QA checklists.

</td>
<td width="50%" valign="top">

### Designer Toolkit
[designer-toolkit](./designer-toolkit) · 7 skills · 4 commands

The work around the work. Design rationale, presentations, pitch decks, case studies, UX writing, design system adoption guides.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Brand Identity
[brand-identity](./brand-identity) · 7 skills · 3 commands

Build something lasting. Brand strategy, logo systems, color identity, typography identity, brand voice, visual guidelines.

</td>
<td width="50%" valign="top">

### Client Pitch
[client-pitch](./client-pitch) · 6 skills · 3 commands

Win the room. Proposals, project scoping, client briefing, kickoff facilitation, pitch structure, feedback management.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Motion Design
[motion-design](./motion-design) · 6 skills · 3 commands

Make it feel alive. Motion principles, scroll animation, transition systems, hero animations, brand motion, loading animation.

</td>
<td width="50%" valign="top">

### Accessibility
[accessibility](./accessibility) · 7 skills · 3 commands

Design for everyone. WCAG 2.2, screen reader UX, keyboard navigation, ARIA patterns, focus management, BFSG compliance.

</td>
</tr>
</table>

---

## Figma Integration

10 skills can read directly from your Figma files when the [Figma MCP](https://www.figma.com/developers/mcp) is connected. Instead of generating placeholders, they pull your actual variables, components, and design context — so what comes out reflects what's actually in your file.

**Setup:** Add the Figma MCP in Claude Code's MCP settings. Once connected, these skills will ask for a Figma URL if you don't provide one, and fall back to the generic approach if you don't have a file yet.

| Skill | What Figma unlocks |
|-------|--------------------|
| `design-token` | Reads your variable collections → real token names and values, no placeholders |
| `component-spec` | Inspects actual layer structure, variants, and token references |
| `color-system` | Extracts your palette from color variables and applied styles |
| `typography-scale` | Reads text styles and type variables directly from the file |
| `spacing-system` | Pulls spacing variables and verifies them against applied layouts |
| `handoff-spec` | Reads measurements, token references, and layout from the target frame |
| `naming-convention` | Audits your actual layer and component names, not a hypothetical |
| `pattern-library` | Searches and inventories existing components in your design system |
| `icon-system` | Inventories icon count, categories, and grid spec from your library |
| `accessibility-audit` | Visual inspection, real contrast values, and layer structure review |

---

## Commands

Commands chain skills together into a complete workflow — one line, one outcome.

**Design Research**

| Command | What it does |
|---------|-------------|
| `/design-research:discover` | Run a full user research discovery cycle |
| `/design-research:interview` | Prepare and conduct a user interview |
| `/design-research:test-plan` | Create a usability test plan |
| `/design-research:synthesize` | Synthesize research data into insights |

**Design Systems**

| Command | What it does |
|---------|-------------|
| `/design-systems:audit-system` | Audit a design system for consistency and accessibility |
| `/design-systems:create-component` | Scaffold a full component specification |
| `/design-systems:tokenize` | Extract and organize design tokens |

**UX Strategy**

| Command | What it does |
|---------|-------------|
| `/ux-strategy:strategize` | Develop a complete UX strategy |
| `/ux-strategy:benchmark` | Run a competitive benchmarking analysis |
| `/ux-strategy:frame-problem` | Structure an ambiguous challenge into a clear problem |

**UI Design**

| Command | What it does |
|---------|-------------|
| `/ui-design:design-screen` | Design a complete screen layout |
| `/ui-design:color-palette` | Generate a full color palette with accessibility checks |
| `/ui-design:type-system` | Create a complete typography system |
| `/ui-design:responsive-audit` | Audit a design for responsive behavior |

**Interaction Design**

| Command | What it does |
|---------|-------------|
| `/interaction-design:design-interaction` | Design a complete interaction flow |
| `/interaction-design:map-states` | Model states and transitions for a component |
| `/interaction-design:error-flow` | Design error handling for a feature |

**Prototyping & Testing**

| Command | What it does |
|---------|-------------|
| `/prototyping-testing:prototype-plan` | Create a prototyping and testing plan |
| `/prototyping-testing:evaluate` | Run a heuristic evaluation |
| `/prototyping-testing:test-plan` | Design a complete usability testing plan |
| `/prototyping-testing:experiment` | Design an A/B experiment |

**Design Ops**

| Command | What it does |
|---------|-------------|
| `/design-ops:plan-sprint` | Plan a design sprint |
| `/design-ops:handoff` | Generate a developer handoff package |
| `/design-ops:setup-workflow` | Set up a design team workflow |

**Designer Toolkit**

| Command | What it does |
|---------|-------------|
| `/designer-toolkit:write-rationale` | Write design rationale for decisions |
| `/designer-toolkit:build-presentation` | Structure a design presentation |
| `/designer-toolkit:write-case-study` | Create a portfolio case study |
| `/designer-toolkit:write-pitch` | Build a complete pitch deck |

**Brand Identity**

| Command | What it does |
|---------|-------------|
| `/brand-identity:brand-audit` | Audit an existing brand for consistency and strategic clarity |
| `/brand-identity:create-identity` | Create a complete visual identity from brand strategy |
| `/brand-identity:define-voice` | Define brand voice, tone, and messaging framework |

**Client Pitch**

| Command | What it does |
|---------|-------------|
| `/client-pitch:write-proposal` | Write a complete client proposal from a brief |
| `/client-pitch:run-kickoff` | Prepare and facilitate a project kickoff |
| `/client-pitch:scope-project` | Define and document full project scope |

**Motion Design**

| Command | What it does |
|---------|-------------|
| `/motion-design:design-motion` | Design a complete motion system for a product |
| `/motion-design:motion-audit` | Audit existing motion for consistency and performance impact |
| `/motion-design:animate-transition` | Design transitions between specific states or pages |

**Accessibility**

| Command | What it does |
|---------|-------------|
| `/accessibility:accessibility-audit` | Run a full accessibility audit across a product or component |
| `/accessibility:wcag-review` | Review designs against WCAG 2.2 AA criteria |
| `/accessibility:inclusive-review` | Review designs across disability types for inclusive coverage |

---

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines on adding new skills, commands, and plugins.

## License

MIT — see [LICENSE](./LICENSE).
