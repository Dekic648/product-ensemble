# Domain Configuration

This file injects company-specific context into every agent in the Product Ensemble. Edit this file to make the agents think in your domain instead of as generalists.

If this file is empty or unchanged from the template, agents will operate as generalists. The more specific you are, the sharper their output becomes.

## Company Context

**Company name:** [Your company name]

**What you do:** [One sentence — what your product/company does]

**Who your users are:** [Primary user personas — role, skill level, what they care about]

**Industry / domain:** [e.g., fintech, healthcare, developer tools, e-commerce, automotive]

## Product Vision

**Where the product is going:** [What does the product look like in 2-3 years?]

**Core value proposition:** [Why do users choose you over alternatives?]

**Current stage:** [Pre-launch / Early traction / Growth / Scale / Mature]

## Strategic Constraints

**Regulatory / compliance requirements:** [e.g., HIPAA, SOC2, GDPR, automotive safety, AI safety policies — or "none"]

**Technology stack:** [e.g., Next.js + Supabase, React Native, Rails, etc.]

**Team size / capacity:** [e.g., solo founder, 3-person team, 20-person eng org]

**Business model:** [e.g., SaaS subscription, usage-based, marketplace, freemium]

## Competitive Landscape

**Primary competitors:** [Who are you competing with?]

**Your edge:** [What do you do better or differently?]

**Where you don't compete:** [What do you intentionally avoid?]

## Product Principles

List 3-5 principles that should guide all product decisions. These override generic defaults.

1. [e.g., "Privacy is non-negotiable — we never sell user data"]
2. [e.g., "Speed over features — a fast simple tool beats a slow complex one"]
3. [e.g., "Enterprise-ready from day one — no 'we'll add auth later'"]
4. [e.g., "Offline-first — users are in the field with unreliable connections"]
5. [e.g., "AI-augmented, not AI-dependent — users must be able to work without AI"]

## How Agents Should Use This

Every agent in the ensemble reads this file at the start of a session. It shapes:

- **UX Designer:** User personas, mental models, domain-specific flows
- **Product Manager:** Scope decisions informed by team capacity and business model
- **CPO:** Strategic validation against company vision and competitive positioning
- **Lead Engineer:** Technical decisions informed by stack, compliance, and scale requirements
- **Roadmap Strategist:** Phasing informed by team size, business stage, and constraints
- **Safety & Compliance (Full Launch):** Regulatory requirements specific to your domain
- **Research Advisor (Full Launch):** Feasibility within your technology constraints
- **GTM Strategist (Full Launch):** Distribution strategy for your market and business model
