---
description: "Simulate 6 real users walking through the product — each persona attempts a key task by tracing actual code paths, reports what breaks, confuses, or dead-ends"
---

You are running a **User Test** session.

## What This Does

This session simulates 6 diverse users attempting key tasks in the product. Unlike design reviews or code reviews, this tests **what actually happens** when someone uses the product — by reading the code that runs, not the spec that was written.

Each persona has a different profile (first-timer, consultant in a rush, non-technical user, power user, report builder, mobile user) and a specific task. The agent traces their journey through the actual codebase and reports every issue found.

## How to Use

Point the User Tester at the product. This can be:
- A directory path to the codebase
- A specific feature to focus on (e.g., "test the Report Builder")
- "Test everything" for a full sweep

The agent will read the actual source files, trace routes, check handlers, verify state flows, and produce a prioritized issue report.

## Process

Use the product-ensemble:user-tester skill. The agent will:

1. Identify the entry points and key routes in the application
2. Simulate all 6 personas attempting their tasks
3. Trace each persona's journey through the actual code (reading components, handlers, state management)
4. Report findings as a structured User Test Report with file paths and line numbers
5. Prioritize issues by impact and fix complexity

After the report is delivered, the user decides which issues to fix immediately and which to defer.

## When to Use

- **Before shipping** — catch issues before users do
- **After building a new feature** — verify it works end-to-end
- **After a retro** — validate that reported issues are actually fixed
- **Periodically** — as a quality gate before any release

## Output

A User Test Report containing:
- Test summary (pass/fail per persona)
- Critical issues (blocks the task)
- Friction issues (task completes but painfully)
- Missing states (empty/error/edge cases)
- Positive findings (what works well)
- Fix priority (ordered issue list)
