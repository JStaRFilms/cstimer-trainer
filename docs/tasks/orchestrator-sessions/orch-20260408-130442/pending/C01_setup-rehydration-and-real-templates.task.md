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

Make the training setup flow truthful and reusable by restoring saved state and turning templates into a real reusable feature.

## Scope

- rehydrate setup controls from saved plan or active plan state where appropriate
- make `Save as Template` create a real reusable template artifact
- load saved templates back into the setup picker
- keep current setup, plan-save, and session-start behavior stable

## Definition of Done

- setup controls restore meaningful prior state
- saved templates can be selected later from the UI
- misleading “settings are saved between sessions” behavior is fixed by implementation, wording, or both

## Expected Artifacts

- updated setup flow
- template persistence behavior
- verification notes for plan restore and template reuse

## Constraints

- do not break existing plan persistence
- do not introduce backend dependencies
- update docs if persistence semantics change

## Review Checkpoint

Orchestrator verifies that setup state and template behavior are now real, not only stored data without retrieval.

