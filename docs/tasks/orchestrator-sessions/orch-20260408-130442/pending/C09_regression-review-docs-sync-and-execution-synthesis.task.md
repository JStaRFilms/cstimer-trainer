## 🔧 Agent Setup (DO THIS FIRST)

### Workflow to Follow
> Read `C:\Users\johno\.agents\skills\takomi\workflows\vibe-syncDocs.md`

### Prime Agent Context
> MANDATORY: Read `C:\Users\johno\.agents\skills\takomi\workflows\vibe-primeAgent.md`

### Required Skills
| Skill | Why |
|-------|-----|
| takomi | Final carry-forward orchestration synthesis |
| sync-docs | Keep docs aligned with the real implementation |

## Objective

Run the final review and synthesis pass for this carry-forward session so another orchestrator can verify subagent work against one clean source of truth.

## Scope

- verify changed behavior against planner, persistence, export/import, and UI expectations
- update docs impacted by completed tasks
- summarize completed versus deferred carry-forward work
- produce the execution synthesis for the next orchestrator loop

## Definition of Done

- completed work is verified
- docs reflect reality
- the next orchestrator can review the wave without reconstructing intent

## Expected Artifacts

- regression note
- docs sync
- execution summary

## Review Checkpoint

User or orchestrator signs off on the verified carry-forward wave.

