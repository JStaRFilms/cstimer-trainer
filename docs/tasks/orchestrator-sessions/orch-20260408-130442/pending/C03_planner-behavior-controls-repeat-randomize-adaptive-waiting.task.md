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

Turn the remaining planner-related setup controls into real behavior, or remove or rename them if they are intentionally unsupported.

## Scope

- implement `Repeat Failed Cases` with clear semantics
- implement `Randomize Order` as a true planner option if retained
- decide whether `adaptive waiting` is a real feature and either implement it cleanly or remove misleading references
- preserve current queue guarantees such as repeat protection, coverage floor, and requested attempt count

## Definition of Done

- each exposed setup control maps to real behavior or is explicitly removed
- planner docs match the shipped behavior
- regression coverage exists for any changed planner logic

## Expected Artifacts

- planner or integration changes
- updated tests
- docs note for new or removed behavior

## Constraints

- do not silently weaken existing queue guarantees
- recognition and execution metrics must stay conceptually separate

## Review Checkpoint

Orchestrator verifies that no remaining setup control is just decorative.

