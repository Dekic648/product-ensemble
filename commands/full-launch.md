---
description: "Expand a shipped Soft Launch into Full Launch — re-evaluates with real data, adds Safety & Compliance, Research/Feasibility, Go-to-Market, and produces an expanded roadmap"
---

You are starting a **Full Launch** Product Ensemble session.

## What This Does

Full Launch builds on a Soft Launch that has already shipped. It takes what you learned from V1 and expands the product into a scalable, production-grade offering with the layers that weren't needed for initial validation.

**Prerequisites:** You should have already completed a Soft Launch (`/ensemble:design`) and ideally shipped V1 to real users. Run `/ensemble:retro` first if you haven't already — Full Launch is most valuable when informed by real-world data.

## Full Launch Sequence

```
1. Re-evaluation    → Core 5 agents re-run with V1 data (abbreviated, focused on what changed)
2. Safety Review    → Safety & Compliance Reviewer assesses regulatory and compliance gaps
3. Research Check   → Research Advisor validates feasibility of expanded capabilities
4. GTM Strategy     → GTM Strategist defines pricing, distribution, and launch plan
5. Full Roadmap     → Roadmap Strategist produces expanded Full Launch roadmap incorporating all of the above
```

## What Full Launch Adds

| Layer | What It Does | Why It Waits Until Now |
|-------|-------------|----------------------|
| **Safety & Compliance Review** | Dedicated review of regulatory, safety, and compliance requirements for your domain | Soft Launch validates the thesis; Full Launch ensures it scales safely |
| **Research / Feasibility Validation** | Assesses whether unproven capabilities can support expanded scope | V1 data reveals where feasibility assumptions held and where they didn't |
| **Go-to-Market Strategy** | Pricing, distribution, launch planning, documentation strategy | You don't market something you haven't validated |

## How to Use

Provide:
1. **Your original Soft Launch artifacts** (or point to where they live)
2. **V1 learnings** — metrics, user feedback, surprises, friction points (or output from `/ensemble:retro`)
3. **Expanded goals** — what you want Full Launch to achieve beyond V1

## Process

### Phase 1: Core Re-evaluation (Abbreviated)

Re-run the 5 core agents in sequence, but focused on what changed:
- **UX Designer:** Review V1 flows against real user behavior. What needs to change?
- **Product Manager:** Update scope — what moves from deferred to in-scope? What new stories emerged?
- **CPO:** Re-validate strategic fit with V1 evidence. Has the thesis held?
- **Lead Engineer:** Update technical advisory with V1 learnings — what technical debt needs addressing?

This phase is abbreviated — agents focus on deltas from Soft Launch, not a repeat of the full analysis. Use the product-ensemble skills for each agent.

### Phase 2: Full Launch Specialists

After the core re-evaluation, run the three Full Launch specialists in sequence:

1. **Safety & Compliance** (product-ensemble:safety-compliance) — reviews regulatory requirements, data flows, accessibility, and safety-critical paths. Produces a Safety & Compliance Review.

2. **Research Advisor** (product-ensemble:research-advisor) — assesses whether expanded capabilities are feasible at the required quality bar. Produces a Feasibility Assessment with recommended spikes.

3. **GTM Strategist** (product-ensemble:gtm-strategist) — defines go-to-market strategy: pricing, distribution channels, launch sequence, documentation needs. Produces a GTM Strategy.

User approval gates apply after each specialist, same as Soft Launch.

### Phase 3: Full Launch Roadmap

The **Roadmap Strategist** (product-ensemble:roadmap-strategist) runs last, producing an expanded roadmap that incorporates:
- Updated core artifacts from Phase 1
- Compliance requirements and actions from Safety Review
- Research spikes and capability validation from Feasibility Assessment
- GTM activities, documentation, and launch phasing from GTM Strategy
- All deferred items from Soft Launch whose activation triggers have been met

The Full Launch roadmap should clearly distinguish between:
- **Product development phases** (features, fixes, expansions)
- **Compliance workstreams** (regulatory actions, accessibility, audit trails)
- **Research spikes** (capability validation before commitment)
- **GTM workstreams** (docs, pricing setup, channel activation, launch sequence)

## Domain Configuration

Check for `domain.md` in the project root. During Full Launch, domain context is especially critical for:
- Safety & Compliance (regulatory requirements vary dramatically by domain)
- Research Advisor (technology constraints are domain-specific)
- GTM Strategist (distribution channels and pricing depend on market context)

If `domain.md` hasn't been configured, strongly recommend the user fill it out before proceeding with Full Launch.

## When to Use Full Launch

- V1 is shipped and you have real user data
- You're entering a regulated domain (healthcare, automotive, finance, AI safety)
- You're scaling from early adopters to a broader market
- Deferred items from Soft Launch have hit their activation triggers
- You need pricing, distribution, and launch planning

## When NOT to Use Full Launch

- You haven't shipped Soft Launch yet — go ship first
- You're still iterating on the core thesis — use `/ensemble:retro` then `/ensemble:design`
- You want to add a single feature — use `/ensemble:design` for that feature
