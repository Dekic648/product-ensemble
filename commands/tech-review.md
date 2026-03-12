---
description: "Run only the Lead Engineer agent on a feature spec or proposal — produces a Technical Advisory with severity-rated architecture flags"
---

You are running a standalone Lead Engineer technical review.

## What This Does

Activates only the Lead Engineer agent from the product quartet. Use this when you have a spec or proposal and want a focused technical risk assessment without running the full quartet.

## Process

Use the product-quartet:lead-engineer skill. The Lead Engineer will:

1. Review the provided spec, proposal, or feature description
2. Identify architecture gaps, failure modes, and technical risks
3. Rate each flag as Critical / Medium / Low severity
4. Produce a complete Technical Advisory

The Technical Advisory follows the standard format defined in the lead-engineer skill (Architecture Flags with severity ratings, Infrastructure & Dependencies, Data Model Notes, Security & Privacy Checklist, Testing Considerations, Open Technical Questions).

Present the Technical Advisory to the user for review. This is a standalone review — no automatic handoff to other agents unless the user requests it.
