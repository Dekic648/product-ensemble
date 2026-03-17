# Product Quartet

Product Quartet is a complete product design workflow for your coding agents, built on top of a set of composable "skills" that make sure your agent doesn't just jump into building — it thinks through the experience, the scope, the strategy, and the technical risks first.

## The Five Agents

| Agent | Role | Runs | Output |
|-------|------|------|--------|
| **UX Designer** | Defines the user experience — flows, interactions, friction, IA | 1st (leads) | UX Brief |
| **Product Manager** | Shapes UX into buildable spec — scope, stories, acceptance criteria | 2nd | Annotated Product Spec |
| **CPO / Strategist** | Validates strategic fit — vision, positioning, timing, opportunity cost | 3rd | Strategic Assessment |
| **Lead Engineer** | Flags technical risks — architecture gaps, security, scalability | 4th | Technical Advisory |
| **Roadmap Strategist** | Synthesizes all artifacts into a prioritized implementation plan | 5th (last) | Prioritized Implementation Roadmap |

## How It Works

It starts the moment you describe what you want to build. Instead of jumping straight into code, your agent steps back and thinks through the product.

The **UX Designer** goes first — asking what the user actually does, step by step, where they'll get confused, and what the happy path looks like. Once you've signed off on the experience, the **Product Manager** takes that vision and draws the line between what's in and what's out. Scope, user stories, acceptance criteria — the stuff that turns a good idea into a buildable spec.

Then the **CPO** weighs in at the strategic level: is this the right bet? Does it serve the long-term vision? They issue a verdict — GO, REDIRECT, DEFER, or KILL. If they redirect, the PM revises and the CPO re-evaluates. The orchestrator handles this loop automatically (max 3 iterations).

Then the **Lead Engineer** reviews what everyone agreed on and flags technical risks — missing error recovery, no caching strategy, privacy gaps, vendor lock-in — each rated by severity. Advisory only.

Finally, the **Roadmap Strategist** takes everything the team has produced and synthesizes it into a prioritized implementation roadmap — phases, dependencies, effort sizing, and sequencing rationale. The first phase always delivers a closed loop of user value. Technical risks get front-loaded. Deferred items get explicit activation triggers. You review the roadmap and decide how to proceed.

You approve after every agent. Nothing advances without your sign-off. And because the skills trigger automatically, you don't need to do anything special. Your coding agent just has a product team.

## Soft Launch First, Always

Every quartet session produces a **Soft Launch** plan — a complete, shippable V1 designed to validate your core thesis with real users. It's not a prototype. It's a finished product, scoped tightly.

Once you've shipped V1 and collected real-world feedback, you can expand into a **Full Launch** — adding safety review, research validation, go-to-market strategy, and data-driven iteration.

You don't need Full Launch to ship. You need it to scale.

## Commands

| Command | What it does |
|---------|-------------|
| `/quartet:design` | Soft Launch session — idea through all five agents, produces shippable V1 plan |
| `/quartet:critique` | Run all five agents on an existing proposal in Soft Launch mode |
| `/quartet:full-launch` | Expand a shipped V1 into Full Launch — safety, research, GTM, data-driven iteration |
| `/quartet:ux-review` | Standalone UX Designer review |
| `/quartet:tech-review` | Standalone Lead Engineer technical review |

## Installation

### Claude Code Plugin Marketplace

```bash
/plugin install product-quartet@claude-plugins-official
```

### Claude Code (via Plugin Marketplace)

```bash
/plugin marketplace add milovandekic/product-quartet-marketplace
/plugin install product-quartet@product-quartet-marketplace
```

### Manual Installation

Clone this repo and point Claude Code at the directory:

```bash
git clone https://github.com/milovandekic/product-quartet.git
```

Then reference the skills directory in your Claude Code configuration.

## Repo Structure

```
product-quartet/
├── .claude-plugin/
│   ├── plugin.json              # Plugin manifest
│   └── marketplace.json         # Marketplace config
├── skills/
│   ├── ux-designer/SKILL.md        # UX Designer agent
│   ├── product-manager/SKILL.md    # Product Manager agent
│   ├── cpo/SKILL.md                # CPO / Strategist agent
│   ├── lead-engineer/SKILL.md      # Lead Engineer agent
│   └── roadmap-strategist/SKILL.md # Roadmap Strategist agent
├── commands/
│   ├── design.md                # /quartet:design — Soft Launch session
│   ├── critique.md              # /quartet:critique — critique existing (Soft Launch)
│   ├── full-launch.md           # /quartet:full-launch — expand V1 to Full Launch
│   ├── ux-review.md             # /quartet:ux-review — UX only
│   └── tech-review.md           # /quartet:tech-review — tech only
├── agents/
│   └── orchestrator.md          # Sequencing, routing, redirect loops
├── README.md
└── RELEASE-NOTES.md
```

## Trigger

The quartet activates when you describe a new feature or product idea:

- "I want to add onboarding to my app"
- "Let's design a notifications system"
- "I'm building a marketplace, where do I start?"

Or invoke directly with `/quartet:design`.

## Design Principles

- **Distinct voices** — each agent has a non-overlapping lens and worldview
- **Sequential, not parallel** — order matters. UX before scope. Scope before strategy. Strategy before architecture
- **User gates** — you approve every artifact before it moves forward
- **Advisory, not authoritative** — agents recommend. You decide
- **Redirect loops** — the CPO can send work back to the PM. The orchestrator manages this automatically
- **Composable** — use the full quartet or invoke individual agents standalone

## License

MIT
