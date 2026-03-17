---
description: "Run a retrospective on a shipped Soft Launch — feed real-world learnings back into the product process to inform what's next"
---

You are running a **Product Ensemble Retrospective** on a shipped V1.

## What This Does

A Soft Launch is only valuable if you learn from it. This command captures what happened after V1 shipped — what worked, what didn't, what surprised you — and produces actionable insights that feed into either iteration or Full Launch.

## How to Use

Tell the retro what you learned. Provide whatever you have:

- **User feedback** — what users said, complained about, praised, or ignored
- **Metrics** — usage numbers, completion rates, drop-off points, engagement
- **Surprises** — things that worked unexpectedly well or broke unexpectedly
- **Friction points** — where users got stuck, confused, or abandoned the flow
- **Support tickets** — common questions or issues
- **Your own observations** — what felt right and what felt off

You don't need all of these. Share what you have.

## Process

### 1. Learning Capture

Organize the learnings into structured categories:

```markdown
# Retrospective: [Feature Name]

## What Worked
Things that validated the Soft Launch thesis — users did what we expected,
metrics hit targets, the experience felt right.

## What Didn't Work
Things that fell short — low adoption, user confusion, missing capabilities,
performance issues, wrong assumptions.

## Surprises
Things we didn't predict — unexpected use cases, features users loved/hated
more than expected, behaviors we didn't design for.

## Assumption Validation
For each core assumption from the Soft Launch Readiness section:
- **Assumption:** [What we believed]
- **Result:** Validated / Invalidated / Inconclusive
- **Evidence:** [What data supports this]
- **Implication:** [What this means for the next phase]
```

### 2. Impact Assessment

For each learning, assess the impact:

```markdown
## Impact Assessment

| Learning | Category | Impact | Action |
|----------|----------|--------|--------|
| [What we learned] | Worked / Didn't / Surprise | High / Medium / Low | Iterate / Expand / Fix / Remove / Investigate |
```

### 3. Recommendations

Produce clear next-step recommendations:

```markdown
## Recommendations

### Immediate Fixes (do now)
Issues that are hurting the current experience and should be addressed
before any expansion. These don't need a full ensemble session — just fix them.

### Iteration Candidates (run /ensemble:design)
Features or flows that need redesign based on what we learned.
Each should be scoped as a new ensemble session.

### Full Launch Readiness
Based on the evidence:
- **Ready for Full Launch?** Yes / Not yet / Needs more data
- **Why:** [Evidence-based rationale]
- **What's missing:** [If not ready, what needs to happen first]

### Updated Activation Triggers
Revisit the deferred items from the original roadmap.
Which activation triggers have been met? Which need updating?

| Deferred Item | Original Trigger | Status | Updated Trigger |
|--------------|-----------------|--------|-----------------|
| [Item] | [Original condition] | Met / Not met / Revised | [New condition if changed] |
```

### 4. Decision Log Update

If the original session produced a Decision Log, update it:
- Which decisions proved right?
- Which need revisiting?
- What new decisions does the evidence demand?

## When to Use This

- After V1 has been live long enough to generate meaningful data (typically 2-4 weeks minimum)
- When you have user feedback, metrics, or observations to work with
- Before deciding whether to iterate on V1 or move to Full Launch
- Whenever you want to close the learning loop on a shipped feature

## When NOT to Use This

- V1 hasn't shipped yet — ship first, learn second
- You have no data or feedback yet — wait until you do
- You just want to add a new feature — use `/ensemble:design` instead
