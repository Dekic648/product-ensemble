# Release Notes

## v1.0.0 — Initial Release

### What's New

**Four composable product agents:**
- **UX Designer** — leads new feature design with flows, friction analysis, and information architecture
- **Product Manager** — shapes UX briefs into buildable specs with scope boundaries and acceptance criteria
- **CPO / Product Strategist** — validates strategic fit at portfolio level with GO/REDIRECT/DEFER/KILL verdicts
- **Lead Engineer** — flags technical risks with severity-rated architecture advisories

**Orchestrator:**
- Sequential routing: UX Designer → PM → CPO → Lead Engineer
- CPO redirect loop handling (max 3 iterations)
- User approval gates between every agent
- Full artifact chain passed to each subsequent agent

**Commands:**
- `/quartet:design` — full quartet session for new feature ideas
- `/quartet:critique` — run all four agents on an existing proposal
- `/quartet:ux-review` — standalone UX Designer review
- `/quartet:tech-review` — standalone Lead Engineer technical review

**Plugin compatibility:**
- `.claude-plugin` manifest for Claude Code plugin marketplace
- Standard SKILL.md conventions and plugin architecture

