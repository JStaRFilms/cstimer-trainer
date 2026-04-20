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

Replace the blank active-session case visual with a real case image or state rendering aligned with csTimer, and wire the hint toggle to actual active-session behavior.

## Scope

- inspect csTimer-native visual or case-rendering capabilities
- render real PLL or OLL case imagery in the active session instead of a blank placeholder square
- wire `Show Algorithm Hints` so the UI toggle controls whether hints are shown
- preserve scramble correctness and current timing flow

## Definition of Done

- active session shows a real visual for supported cases
- hint visibility follows the saved session setting
- no regression in scramble generation, timing, or layout

## Expected Artifacts

- active-session visual update
- hint-control behavior
- verification note for supported case families

## Constraints

- prefer following csTimer’s existing rendering approach instead of building a separate visual system
- do not regress keyboard timing behavior

## Review Checkpoint

Orchestrator verifies that the active-session center visual is no longer a placeholder and that the hint toggle is functional.

