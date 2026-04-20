## 🔧 Agent Setup (DO THIS FIRST)

### Workflow to Follow
> Read `C:\Users\johno\.agents\skills\takomi\workflows\mode-code.md`

### Prime Agent Context
> MANDATORY: Read `C:\Users\johno\.agents\skills\takomi\workflows\vibe-primeAgent.md`

### Required Skills
| Skill | Why |
|-------|-----|
| takomi | Task orchestration baseline |

## Objective

Review and improve trainer state restoration so restarts, returns to setup, and session re-entry behave intentionally.

## Scope

- inspect active plan, saved plan, and setup restore expectations
- clarify or implement restart and re-entry behavior
- verify whether any additional trainer state should persist locally
- preserve export/import semantics unless a documented change is approved

## Definition of Done

- restore behavior is intentional rather than accidental
- resumed or reopened flows do not contradict the UI
- persistence docs reflect the real behavior

## Expected Artifacts

- state restoration changes if needed
- persistence note
- verification note for restart and re-entry cases

## Constraints

- do not corrupt trainer data
- do not mutate raw solve-history records

## Review Checkpoint

Orchestrator verifies that session re-entry and restore expectations are explicit and stable.

