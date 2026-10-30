# AGENTS.md - Ralph Loop State

## Current Iteration: 5
## Phase: Core Development
## Completion Status: IN_PROGRESS

### Features Complete
- [x] Validation harness
- [x] CI workflow
- [x] Gitignore setup
- [x] Core HTML structure
- [x] localStorage implementation
- [ ] Fighter database
- [ ] Combat engine
- [ ] XP system
- [ ] Export function
- [ ] Import function
- [ ] Reset function
- [ ] Offline capable (no network calls)
- [x] Tap targets 44px+
- [x] Zero dependencies (verified)
- [ ] Termux validated

### Last Iteration Summary
Objective: Implement fighter database
Result: IN PROGRESS (normalized loaded localStorage state)
Tests: npm run check (failed: missing type definition files for node and vite/client)
Next: Fighter database

### Current Objective
Implement fighter database

### Blocking Issues
None

### Circuit Breaker Status
- No-progress count: 0/3
- Same-error count: 1/5
- Rollback count: 0/5
- Last rollback: None
- Status: ACTIVE

### Last Error (if any)
```
error TS2688: Cannot find type definition file for 'node'.
error TS2688: Cannot find type definition file for 'vite/client'.
```

### Next Action
Define fighter database entries and wire them into the loop state.

## NGL-wide operating contract

Before any work, read the [canonical shared Ralph-style protocol](https://github.com/ngl-damien/No-Gas-Labs-Alpha-1/blob/main/docs/operations/RALPH_SHARED_HOURLY_SCHEDULER_PROTOCOL.md). It supplements this repository's existing Ralph-loop state; it does not replace or reset the current iteration, objective, error counters, or next action above.

Every run must rehydrate from current source, PRs, checks, and durable state; observe and rank real opportunities; challenge whether work is already fixed or duplicated; make a bounded change; verify the exact commit; review for regressions; preserve factual results; hand off cross-repository work; and repeat when safe. Keep the $0 additional-cost constraint.

A model assertion is not evidence. Distinguish source presence, tests, hosted CI, deployment, and user outcome. Do not invent completion, progress, authority, or functionality. Do not merge, release, deploy, spend, publish externally, change secrets/permissions, or take destructive actions without explicit authorization from Damien Featherstone. If the canonical protocol cannot be read, stop and report the blocker.
