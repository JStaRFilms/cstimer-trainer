# Carry-Forward Orchestrator Session Master Plan

**Session ID:** `orch-20260408-130442`  
**Mode:** Takomi execution orchestrator  
**Project:** csTimer Trainer carry-forward session

## Purpose

Run the next orchestration cycle against the unfinished trainer work without reopening settled scope or losing the implementation already completed.

This session is for:
- carrying forward every unfinished trainer item in one continuous queue
- converting the remaining backlog into delegable, reviewable task packets
- preserving architecture, persistence, export/import, and planner guarantees already in place
- adding the newly requested orientation-aware start-state modeling and real case imagery requirements

This session is not for:
- replacing prior completed sessions
- inventing a new batch boundary
- rewriting v1 into a backend-dependent product

## Baseline Inputs

- `docs/project_requirements.md`
- `docs/Coding_Guidelines.md`
- `docs/features/TrainerV1.md`
- `docs/features/TrainerNativeIntegration.md`
- `docs/features/OrientationAwareStartStateModel.md`
- `docs/futures/trainer-backlog.md`
- `docs/architecture/domain-boundaries.md`
- `docs/architecture/persistence-plan.md`
- `docs/architecture/export-import-compatibility.md`
- `docs/architecture/planner-logic-spec.md`
- `docs/mockups/*.html`
- prior build session `orch-20260402-202305`

## Carry-Forward Scope

- setup-state rehydration
- real reusable templates
- active-session hint control
- repeat-failed and randomize-order behavior
- adaptive-waiting decision or implementation
- cross drill realism
- active-session case visuals using csTimer-aligned imagery or rendering
- mobile polish
- state restoration and re-entry review
- regression coverage updates
- orientation-aware start-state modeling
- PLL orientation-aware analytics and recommendations
- F2L-ready variant modeling rules

## Execution Order

`C00 preflight -> C01 setup persistence/templates -> C02 active-session visuals/hints -> C03 planner behavior controls -> C04 cross/mobile polish -> C05 state restoration -> C06 orientation-aware architecture -> C07 PLL variant packet -> C08 F2L variant packet -> C09 regression/docs synthesis`

## Parallelism Rules

- Default mode for this session is sequential, one task at a time.
- No downstream task should start until its upstream assumptions are reviewed.
- `C06`, `C07`, and `C08` are tightly related and should be treated as an architecture-first sequence, not three disconnected experiments.
- Review and regression work may be revisited after any major merge, but `C09` is the final synthesis gate.

## Task Registry

| ID | Task | Depends On | Workflow | Review Gate |
| :--- | :--- | :--- | :--- | :--- |
| C00 | Carry-forward preflight and architecture guardrails | none | `mode-orchestrator` + `vibe-primeAgent` | confirm unfinished scope and preserved guarantees |
| C01 | Setup rehydration and real reusable templates | C00 | `mode-code` / build | approve setup truthfulness and plan restore flow |
| C02 | Active-session case visuals and hint-control wiring | C01 | `mode-code` / build | approve real case imagery and hint behavior |
| C03 | Planner behavior controls for repeat, randomize, and adaptive waiting | C02 | `mode-code` / build | approve behavior semantics before merge |
| C04 | Cross drill realism and mobile polish | C03 | `vibe-design` reference + build | approve usability improvements |
| C05 | State restoration and session re-entry review | C04 | `mode-code` / build | approve restart and resume expectations |
| C06 | Orientation-aware start-state architecture and persistence design | C05 | `mode-architect` | approve variant model contract |
| C07 | PLL orientation-aware analytics and recommendation packet | C06 | `mode-code` / build | approve PLL-first implementation cut |
| C08 | F2L-ready variant modeling packet and future-proof domain extension | C07 | `mode-architect` | approve F2L carry-forward shape |
| C09 | Regression review, docs sync, and execution synthesis | C01-C08 | `mode-review` + `vibe-syncDocs` | approve full carry-forward session |

## Review Policy

- Nothing is complete until reviewed against the PRD, coding rules, feature docs, and backlog.
- Completed work must preserve:
  - local-first persistence
  - export/import behavior
  - current planner guarantees
  - isolation from raw solve-history mutation
- Any task that changes planner or persistence behavior must update docs in the same wave.

## Additional Execution Rules

- Do not split unfinished work into a new batch; keep appending to the same carry-forward truth.
- Use csTimer-native capabilities for case imagery wherever possible instead of inventing a parallel renderer.
- Variant-aware modeling must keep recognition and execution separate.
- PLL orientation-aware work is the first target; F2L modeling should be designed now so later work lands cleanly.
