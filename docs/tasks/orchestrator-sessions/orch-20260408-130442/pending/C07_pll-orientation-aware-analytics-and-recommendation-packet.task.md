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

Use PLL as the first concrete implementation target for orientation-aware modeling so the trainer can distinguish the same PLL by start orientation or AUF-sensitive context.

## Scope

- implement the approved PLL-first variant model
- capture or derive the relevant PLL orientation metadata
- store PLL variant-aware analytics separately from base-case aggregates
- enable recommendation hooks for algorithm or pre-turn guidance at the PLL-variant level

## Definition of Done

- PLL weakness analysis can distinguish meaningful start-state variants
- base-case analytics still remain available
- recommendation plumbing can target the exact variant

## Expected Artifacts

- PLL variant-aware implementation slice
- verification note for variant-level analytics
- doc updates describing the PLL-first cut

## Constraints

- do not claim perfect recommendation quality unless the supporting data exists
- preserve current PLL training behavior for users without variant-aware data

## Review Checkpoint

Orchestrator verifies that PLL-level orientation-aware tracking is real and not only a design placeholder.

