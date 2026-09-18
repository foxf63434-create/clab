# CLAB CURRENT STATE

STATUS: HQ_WP04_R01_QA_ACTIVE
LAST_CONTROL_AUDIT: 2026-09-18
SOURCE_OF_TRUTH: GitHub state + actual scheduler observations + exact execution evidence
CURRENT_AUTHORITY: `OWNER_2026-09-18_CONTINUE_TO_WP04`
PUBLIC_WORK_ISSUE: #18 / `BUILD-WP04`

## Global control
CONTROL: NIGHTJET GLOBAL CONTROL
PRIVATE_CORE: `foxf63434-create/meta-sales-system`
PUBLIC_BUS: `foxf63434-create/clab`
IDENTITY_STANDARD: `control/IDENTITY-NAMESPACE-STANDARD.md`
CONTROL_AGENT: `NODE-HQ-01 / TEAM-HQ-001 / HQ-CONTROL-01`

## PRIMARY HQ TEAM — CURRENT PATH
NODE_ID: `NODE-HQ-01`
TEAM_ID: `TEAM-HQ-001`
ADMIN_AGENT_ID: `HQ-REGISTRAR-01`
PROJECT_ID: `PROJECT-CLAB-001`
MISSION_ID: `HQ-BOOTSTRAP-001`
BOOTSTRAP_ISSUE: #11 remains a separate bootstrap-acceptance lifecycle.
ACTIVE_WORK_PACKAGE: #18 / `BUILD-WP04` — owner-authorized minimal read-only Status / Evidence API.
CURRENT_PRIVATE_DISPATCH: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/HQ-WP04-LOOP-001.md`

### Preserved accepted history
WP01: Reviewer PASS on `14872635c8c857ed33384975cd20f18cf7a8f5d9`.
WP02: Reviewer PASS on `b2f18f96a91fb44a60f303303bbd0139e3b6d425`.
WP03: bounded R02 repair is frozen at `CONTROL_ACCEPTED / WP03_R02_BOUNDED_PASS` for exact candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`, tree `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`.
The earlier rejected `e823a05a799bc9a02cfe246c463b9f61fd9e4264` and R01 Reviewer-REJECT candidate remain historical only and are not reopened by WP04.
KNOWN_CARRIED_LIMITATION: network-backed `GitHubApiSource` integration remained explicitly `NOT_TESTED` in WP03 independent QA and must not be represented as PASS without new evidence.

### Current WP04 dispatch
PHASE: `QA`
ROUND: `R01`
ATTEMPT_ID: `R01`
TASK_ID: `HQ-QA-WP04-API-R01`
ACTIVE_OWNER: `HQ-QA-01`
RUN_STATUS: `QA_ACTIVE`
INPUT_CANDIDATE: `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`
INPUT_TREE: `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`
BUILD_BRANCH: `build/wp04-status-evidence-api-001`
CURRENT_CANDIDATE: `50159a0c732e9dc212dbc8e4de18fc4bdefa7cfa`
CURRENT_CANDIDATE_TREE: `880ddda97bc46c77295e14e326b40e52eb5ed49c`
CANDIDATE_DIFF_BASE: `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`
CANDIDATE_DIFF_STATUS: ahead-only, `behind_by=0`, exactly two authorized changed paths.
CURRENT_CHANGED_BLOBS: `meta-orchestrator/control-plane-v0/status_api.py`=`20462266e449115c06285f741187d02381c19d07`; `meta-orchestrator/control-plane-v0/tests/test_status_api.py`=`a212f7be1b5b333f63e60767dde0f2e30967e3e0`.
DEVELOPER_OUTCOME: `READY_FOR_QA`.
DEVELOPER_EVIDENCE: private `EVIDENCE/HQ-WP04-R01-DEVELOPER.md`, commit `bc20bf15ce02995240898cef88862b0c98432137`, blob `d6447a6eaebbfcad687dfa931c71dfae2a932b92`.
DEVELOPER_CHECKPOINT: not present before routing.
QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R01-QA.md` — `PENDING`.
QA_TESTS: private `EVIDENCE/HQ-WP04-R01-QA-TESTS.py` — `PENDING`.
QA_CHECKPOINT: none existed before QA activation.
REVIEWER_EVIDENCE: `NOT_STARTED`.
REJECTED_ROUNDS: `0/3`.
SAME_ROOT_REJECT_COUNT: `0/2`.
CURRENT_BLOCKER: `NONE_PROVEN`.
LAST_TRANSITION_AT: `2026-09-18T12:59:28Z`.

HQ-REGISTRAR-01 verified the Developer terminal `READY_FOR_QA` against the immutable candidate/tree, exact accepted-WP03-base compare, exact two changed blobs and immutable Developer evidence; confirmed there was no pre-existing R01 QA terminal result/tests/checkpoint; moved dispatch to QA, remotely read it back, then enabled the existing HQ-QA-01 worker. This does not imply QA PASS, Reviewer PASS, Control acceptance, merge or deployment.

### WP04 contract
Goal: minimal read-only Status / Evidence API over accepted WP01-WP03 derived state, exposing projects, agents, tasks, reviews, Human Gates, incidents/evidence and freshness/conflict flags.
Every outward status must have source/evidence provenance or explicit `UNKNOWN`.
GitHub remains source of truth; the API is derived/rebuildable; Scheduled Wake remains unchanged.
Preserve fail-closed provenance/identity/security and truthful `STALE_PROJECTION`, `MISSING_REVIEW`, `CONFLICT`, `UNKNOWN` semantics. No false READY/PASS.
No arbitrary repository-write endpoint, production/deploy, merge-to-main, WP05/WP06, permission/workflow change, provider/runtime replacement or legacy/remote activation is authorized.

### HQ-REGISTRAR-01
SCHEDULER_TASK_ID: `6aac1f2261a48191805ee42fa01ec632`
STATUS: `ACTIVE_WP04_REGISTRAR`
AUTHORITY: sole routine WP04 loop/execution/public-HQ-state and worker-lifecycle writer; no implementation, QA, Reviewer verdict or merge authority.

### HQ-DEVELOPER-01
SCHEDULER_TASK_ID: `6aac9020d68c8191af4cee8bd53e374b`
ASSIGNMENT_STATE: `TERMINAL_READY_FOR_QA_WP04_R01`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-DEVELOPER-01-WP04.md`
CURRENT_TASK: terminal `HQ-DEV-WP04-API-R01` on candidate `50159a0c732e9dc212dbc8e4de18fc4bdefa7cfa`.
SCHEDULER_STATE: disabled after terminal handoff; unchanged candidate must not be re-executed.
NEXT_STEP: none unless a bounded QA/Reviewer REJECT creates a materially new authorized round.

### HQ-QA-01
SCHEDULER_TASK_ID: `6aac3099fc9881919e9de980b9fd86a7`
ASSIGNMENT_STATE: `ACTIVE_WP04_R01_QA`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-QA-WP04.md`
CURRENT_TASK: `HQ-QA-WP04-API-R01` on exact candidate `50159a0c732e9dc212dbc8e4de18fc4bdefa7cfa`.
SCHEDULER_STATE: enabled only after Registrar read back the QA dispatch and verified no current-round terminal QA evidence/checkpoint existed.
NEXT_STEP: independently test exact candidate/dependencies and publish one terminal `READY_FOR_REVIEW`, `REJECT` or `BLOCKED`, then stop.

### HQ-REVIEWER-01
SCHEDULER_TASK_ID: `6aac30a8f27c819198aea8a734aeaf5a`
ASSIGNMENT_STATE: `ARMED_CONDITIONAL_WP04`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-REVIEWER-WP04.md`
SCHEDULER_STATE: disabled until same-candidate independent QA is `READY_FOR_REVIEW` and Registrar moves dispatch to REVIEW.

### HQ-DEVELOPER-02
STATUS: disabled / unassigned for WP04 core/API. It must not duplicate WP04 work; only a separately authorized disjoint package may activate it.

### HQ-CONTROL-01
ROLE: bounded supervisor and final scoped WP04 judge only; Registrar owns routine lifecycle/state transitions.
CURRENT_STATE: WP04 R01 is in independent QA and has no Reviewer or Control PASS.

## WP04 lifecycle
Developer `READY_FOR_QA` -> Registrar pins exact candidate/tree/diff/evidence, disables Developer, moves to QA, reads back, then enables existing QA.
Independent same-candidate QA `READY_FOR_REVIEW` -> Registrar disables QA, pins report/tests, moves to REVIEW, reads back, then enables existing Reviewer.
In-scope QA/Reviewer `REJECT` -> same Developer receives a materially new round, max 3 rounds; stop after two same-root rejects or any architecture/security conflict.
Reviewer `PASS` -> workers stop and Registrar routes `READY_FOR_CONTROL_REVIEW`. Final WP04 acceptance belongs to Control only.

## Legacy local policy
Preserve old chats/history; old NIGHTJET execution schedules remain disabled and receive no new work. No reactivation/repurposing without explicit current owner/control authority. Verify no overlapping active writer before shared-state transfer.

## REMOTE-ADMIN-01
NODE_ID: `NODE-REMOTE-01`
TEAM_ID: `TEAM-REMOTE-001`
HISTORICAL_BOOTSTRAP_EVIDENCE: issue #1
PREVIOUS_CONTROL_TASK: #8 superseded/closed.
CONTROL_TASK: issue #10
STATUS: RESTART_REQUIRED / NOT_PROVEN_PERSISTENT in the last remote snapshot; this HQ inspection did not verify a remote scheduler.
FACTS: prior external bootstrap and issue writing were recorded; persistent remote-worker runtime remains unproven here.
NEXT_STEP: execute #10 only if GLOBAL CONTROL separately continues the remote pilot. HQ must not take remote assignments.

## REMOTE-ADMIN-02
NODE_ID: `NODE-REMOTE-02`
TEAM_ID: `TEAM-REMOTE-002`
BOOTSTRAP_ISSUE: #9
STATUS: PAUSED_BY_CONTROL / NOT_ONLINE.
Do not bootstrap until explicitly reactivated.

## REMOTE-PILOT-001
STATUS: ACTIVE_RECOVERY / NOT_PROVEN_PERSISTENT in its separate recorded snapshot.
MISSION: `missions/REMOTE-PILOT-001/MISSION.md`
CONTROL_ISSUE: #10
STATE_ISSUE: #7
WORKER_ASSIGNMENTS: #3, #4, #5, #6.
MANUAL_ROLE_HUMAN_GATE: #2 superseded/closed.
This HQ work does not grant authority over remote teams.

## Functional workforce and namespaces
Every participant/task has NODE_ID + TEAM_ID + AGENT_ID + PROJECT_ID + MISSION_ID. Unique names and actual assignment bindings are mandatory. A role label or schedule is not proof of an isolated process or independent review. AUTHOR != FINAL JUDGE.

## Security and integration boundaries
CLAB is PUBLIC. Private source/logs/diagnostics/report contents, credentials, customer data and secrets stay private. Use sanitized identifiers/pointers.
Verify capabilities separately in each scheduled context. Missing evidence is `UNKNOWN/PENDING`, not PASS.

## Completion boundary
WP04 R01 has a pinned Developer candidate and is now in independent QA. Independent same-candidate QA, independent Reviewer PASS and final Control acceptance are still required. No full-system `MISSION_COMPLETE` is declared.