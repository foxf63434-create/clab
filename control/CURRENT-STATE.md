# CLAB CURRENT STATE

STATUS: HQ_WP04_R02_QA_ACTIVE
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

### WP04 R01 terminal history
R01_CANDIDATE: `50159a0c732e9dc212dbc8e4de18fc4bdefa7cfa`.
R01_TREE: `880ddda97bc46c77295e14e326b40e52eb5ed49c`.
R01_DEVELOPER_OUTCOME: `READY_FOR_QA`.
R01_DEVELOPER_EVIDENCE: private `EVIDENCE/HQ-WP04-R01-DEVELOPER.md`, commit `bc20bf15ce02995240898cef88862b0c98432137`, blob `d6447a6eaebbfcad687dfa931c71dfae2a932b92`.
R01_QA_OUTCOME: `REJECT / HIGH`.
R01_QA_ROOT_CAUSE: `WP04_PROVENANCE_STRUCTURAL_VALIDATION_MISSING`.
R01_QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R01-QA.md`, commit `a74ebab91450f212eb06dc963fabf24243ca9e4a`, blob `991c64776da2d198d5e8275bb28ffa281df5c459`.
R01_QA_TESTS: private `EVIDENCE/HQ-WP04-R01-QA-TESTS.py`, commit `b8227aeb2ab0141ae01a043752b65d4bb5b74b5b`, blob `ed36373205f9f0f8e5b747eb00fc20f9962f9c20`.
R01_REVIEWER_OUTCOME: `NOT_STARTED / NOT_AUTHORIZED_AFTER_QA_REJECT`.
The rejected R01 candidate is frozen as evidence and must not be reactivated unchanged.

### WP04 R02 Developer terminal handoff
R02_CANDIDATE: `2c5ff49495ac2b0db969c308f4a6b1b837ff7822`.
R02_TREE: `32d5533f33fe27bd857849b6769901edd93176d1`.
R02_DEVELOPER_OUTCOME: `READY_FOR_QA`.
R02_DEVELOPER_EVIDENCE: private `EVIDENCE/HQ-WP04-R02-DEVELOPER.md`, commit `d79a24b73eaf88e82bfb683911655681c23fcd9f`, blob `dd1b50b60a398b170a6acd076080e9190822558b`.
R02_DIFF_FROM_ACCEPTED_WP03: `ahead_by=7 / behind_by=0 / exactly 2 authorized paths`.
R02_DIFF_FROM_REJECTED_R01: `ahead_by=2 / behind_by=0 / same 2 WP04 paths only`.
R02_CHANGED_BLOBS: `meta-orchestrator/control-plane-v0/status_api.py@bea29287076e96d0f36164af25eb23215f66350b`; `meta-orchestrator/control-plane-v0/tests/test_status_api.py@465458e12cfb29df1ee56a2728a0ae3bce1f9128`.
R02_PREEXISTING_QA_TERMINAL: none found before routing; no R02 QA report, persisted QA tests or QA checkpoint existed.
Developer verification is author evidence only and does not constitute independent QA, Reviewer PASS or Control acceptance.

### Current WP04 dispatch
PHASE: `QA`
ROUND: `R02`
ATTEMPT_ID: `R02`
TASK_ID: `HQ-QA-WP04-API-R02`
ACTIVE_OWNER: `HQ-QA-01`
RUN_STATUS: `QA_ACTIVE`
INPUT_CANDIDATE: `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`
INPUT_TREE: `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`
BUILD_BRANCH: `build/wp04-status-evidence-api-001`
CURRENT_CANDIDATE: `2c5ff49495ac2b0db969c308f4a6b1b837ff7822`
CURRENT_CANDIDATE_TREE: `32d5533f33fe27bd857849b6769901edd93176d1`.
CANDIDATE_DIFF_BASE: `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`.
CANDIDATE_DIFF_STATUS: `VERIFIED_AHEAD_ONLY_7_COMMITS_2_AUTHORIZED_PATHS`.
CURRENT_CHANGED_BLOBS: `status_api.py@bea29287076e96d0f36164af25eb23215f66350b`; `tests/test_status_api.py@465458e12cfb29df1ee56a2728a0ae3bce1f9128`.
DEVELOPER_EVIDENCE: private `EVIDENCE/HQ-WP04-R02-DEVELOPER.md`, commit `d79a24b73eaf88e82bfb683911655681c23fcd9f`, blob `dd1b50b60a398b170a6acd076080e9190822558b`; outcome `READY_FOR_QA`.
QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R02-QA.md` — `PENDING`.
QA_TESTS: private `EVIDENCE/HQ-WP04-R02-QA-TESTS.py` — `PENDING`.
REVIEWER_EVIDENCE: private `EVIDENCE/HQ-WP04-R02-REVIEWER.md` — `NOT_STARTED`.
RETURNED_FROM_ROUND: `R01`.
RETURNED_QA_OUTCOME: `REJECT`.
RETURNED_QA_ROOT_CAUSE: `WP04_PROVENANCE_STRUCTURAL_VALIDATION_MISSING`.
REJECTED_ROUNDS: `1/3`.
SAME_ROOT_REJECT_COUNT: `1/2`.
CURRENT_BLOCKER: `NONE`.
LAST_TRANSITION_AT: `2026-09-18T15:56:50Z`.

HQ-REGISTRAR-01 verified the exact materially new R02 Developer `READY_FOR_QA`, exact candidate/tree and immutable Developer evidence, independently verified ahead-only candidate lineage and bounded two-path diff, confirmed the Developer worker had already stopped and that no R02 QA terminal artifact/checkpoint existed, then moved private/public dispatch to independent QA. This does not imply QA PASS, Reviewer PASS, Control acceptance, merge or deployment.

### WP04 R02 QA boundary
Independent HQ-QA-01 must test the exact pinned R02 candidate and complete source/dependency bytes against the WP04 contract. Mandatory coverage includes the persisted R01 malformed-provenance regressions, remaining R01 independent regressions, candidate-authored WP04 tests, affected accepted WP01-WP03 provenance/identity/security regressions, deterministic schemas/rebuild, truthful `UNKNOWN`, `CONFLICT`, `STALE_PROJECTION`, `MISSING_REVIEW`, no false READY/PASS, read-only behavior, source immutability and secret suppression.
Network-backed `GitHubApiSource` remains explicitly `NOT_TESTED` unless independently exercised with reproducible evidence.
Reviewer remains dependency-gated until same-candidate independent R02 QA is `READY_FOR_REVIEW`.

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
ASSIGNMENT_STATE: `TERMINAL_READY_FOR_QA_WP04_R02`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-DEVELOPER-01-WP04.md`
CURRENT_TASK: terminal handoff for `HQ-DEV-WP04-API-R02`; exact candidate/evidence pinned above.
SCHEDULER_STATE: disabled after terminal R02 Developer handoff; unchanged candidate must not repeat.
NEXT_STEP: none unless a later in-scope QA/Reviewer REJECT authorizes a materially new round.

### HQ-QA-01
SCHEDULER_TASK_ID: `6aac3099fc9881919e9de980b9fd86a7`
ASSIGNMENT_STATE: `ACTIVE_WP04_R02_QA`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-QA-WP04.md`
CURRENT_TASK: `HQ-QA-WP04-API-R02` on exact candidate `2c5ff49495ac2b0db969c308f4a6b1b837ff7822` / tree `32d5533f33fe27bd857849b6769901edd93176d1`.
SCHEDULER_STATE: existing worker is authorized for one independent R02 terminal result only after this private/public dispatch is remotely read back; no prior R02 QA terminal artifact exists.
NEXT_STEP: publish exactly one independent same-candidate `READY_FOR_REVIEW`, `REJECT` or truthful `BLOCKED`, then stop.

### HQ-REVIEWER-01
SCHEDULER_TASK_ID: `6aac30a8f27c819198aea8a734aeaf5a`
ASSIGNMENT_STATE: `ARMED_CONDITIONAL_WP04`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-REVIEWER-WP04.md`
SCHEDULER_STATE: disabled until same-candidate independent R02 QA is `READY_FOR_REVIEW` and Registrar moves dispatch to REVIEW.

### HQ-DEVELOPER-02
STATUS: disabled / unassigned for WP04 core/API. It must not duplicate WP04 work; only a separately authorized disjoint package may activate it.

### HQ-CONTROL-01
ROLE: bounded supervisor and final scoped WP04 judge only; Registrar owns routine lifecycle/state transitions.
CURRENT_STATE: WP04 R01 ended in independent QA REJECT; materially new R02 candidate is now routed to independent QA and has no QA, Reviewer or Control PASS.

## WP04 lifecycle
Developer `READY_FOR_QA` -> Registrar pins exact materially new candidate/tree/diff/evidence, disables Developer, moves to QA, reads back, then enables existing QA.
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
WP04 R01 is terminal QA REJECT and frozen as evidence. WP04 R02 has a materially new exact Developer `READY_FOR_QA` candidate and is now in independent QA. Independent same-candidate R02 QA `READY_FOR_REVIEW`, independent Reviewer PASS and final Control acceptance are still required. No full-system `MISSION_COMPLETE` is declared.