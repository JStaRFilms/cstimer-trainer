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

Turn the new orientation-aware start-state idea into an implementation-grade architecture contract before code agents extend the trainer.

## Scope

- define the variant key contract
- define the minimum start-state descriptor contract
- define how recognition and execution stay separate
- define storage and export implications for variant-aware stats
- define fallback rules when variant data is sparse

## Definition of Done

- the feature can be implemented without guessing the domain shape
- PLL-first work has a clean contract
- F2L-forward work has a compatible future shape

## Expected Artifacts

- architecture note or doc update
- variant-model contract
- planner fallback rules

## Constraints

- keep the domain portable
- do not couple the contract to DOM or csTimer globals
- avoid silently distorting existing case-level stats

## Review Checkpoint

Orchestrator approves the variant-model contract before PLL-specific implementation starts.

