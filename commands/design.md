---
description: "Run the full product ensemble on a new feature or product idea — UX Designer, Product Manager, CPO, Lead Engineer, and Roadmap Strategist in sequence"
---

You are starting a **Soft Launch** Product Ensemble design session.

## What This Does

This session produces a complete, shippable V1 — your Soft Launch plan. It's not a prototype or a beta. It's a finished product, scoped tightly to validate your core thesis with real users.

The orchestrator routes your feature idea through five specialized agents in sequence:

1. **UX Designer** — defines the user experience (flows, interactions, friction points)
2. **Product Manager** — shapes it into a buildable spec (scope, stories, acceptance criteria)
3. **CPO / Strategist** — validates strategic fit (vision alignment, competitive positioning, timing)
4. **Lead Engineer** — flags technical risks (architecture gaps, security, scalability)
5. **Roadmap Strategist** — synthesizes everything into a prioritized implementation roadmap

You approve after each agent before the next one begins.

## How to Use

Describe your feature or product idea. Be as detailed or rough as you like — the UX Designer will ask clarifying questions.

Examples:
- "I want to add onboarding to my app"
- "Let's design a notifications system"
- "I'm building a marketplace — where do I start?"

## Process

Use the product-ensemble:ux-designer skill first. After the UX Brief is approved by the user, proceed to product-ensemble:product-manager. After the Product Spec is approved, proceed to product-ensemble:cpo. If the CPO verdict is GO and the user approves, proceed to product-ensemble:lead-engineer.

If the CPO issues a REDIRECT, route back to product-ensemble:product-manager with the CPO's feedback. Maximum 3 redirect loops before surfacing to the user.

Follow the sequencing logic defined in the ensemble-orchestrator agent. Every artifact must be approved by the user before advancing.

After the Lead Engineer's technical advisory is approved, proceed to product-ensemble:roadmap-strategist. The Roadmap Strategist receives all four approved artifacts and produces a prioritized implementation roadmap.

After the roadmap is delivered, present the complete Soft Launch plan to the user. Frame it clearly: this is a shippable V1 ready to build. When the user is ready to scale after shipping V1, they can run `/ensemble:full-launch` to enter the Full Launch phase — which adds safety review, research validation, go-to-market strategy, and data-driven iteration.
