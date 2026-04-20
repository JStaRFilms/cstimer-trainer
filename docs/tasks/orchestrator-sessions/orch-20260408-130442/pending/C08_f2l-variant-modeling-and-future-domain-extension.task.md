## 🔧 Agent Setup (DO THIS FIRST)

### Workflow to Follow
> Read `C:\Users\johno\.agents\skills\takomi\workflows\mode-architect.md`

### Prime Agent Context
> MANDATORY: Read `C:\Users\johno\.agents\skills\takomi\workflows\vibe-primeAgent.md`

### Required Skills
| Skill | Why |
|-------|-----|
| takomi | Task orchestration baseline |

## Objective

Define the F2L-forward extension of the variant-aware model so future work can track pair location, slot target, and related start-state differences cleanly.

## Scope

- define the F2L-facing variant descriptor expectations
- ensure compatibility with the PLL-first model from `C06` and `C07`
- identify which parts are implementation-ready now versus future-scoped
- record how recognition and execution should be represented for F2L variants

## Definition of Done

- F2L-forward modeling is documented well enough that future agents do not need to redesign the domain
- the trainer’s domain remains extensible beyond PLL

## Expected Artifacts

- F2L-forward modeling note
- domain extension guidance
- backlog or docs updates if needed

## Constraints

- this task should not force premature F2L UI implementation
- keep the model aligned with existing portable-domain rules

## Review Checkpoint

Orchestrator approves that the orientation-aware model now scales cleanly into F2L and future case families.

