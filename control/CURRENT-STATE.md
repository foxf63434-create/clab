# CLAB CURRENT STATE

STATUS: HQ_WP04_R03_QA_DISPATCH_READY
LAST_CONTROL_AUDIT: 2026-09-18
SOURCE_OF_TRUTH: GitHub state + actual scheduler observations + exact execution evidence
CURRENT_AUTHORITIES: `OWNER_2026-09-18_CONTINUE_TO_WP04`; `OWNER_2026-09-18_ARCHITECTURE_STRENGTHENING`
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
Earlier rejected WP03 candidates remain historical only and are not reopened by WP04.
KNOWN_CARRIED_LIMITATION: network-backed `GitHubApiSource` integration remained explicitly `NOT_TESTED` in WP03 independent QA and must not be represented as PASS without new evidence.

### WP04 R01 terminal history
R01_CANDIDATE: `50159a0c732e9dc212dbc8e4de18fc4bdefa7cfa`.
R01_TREE: `880ddda97bc46c77295e14e326b40e52eb5ed49c`.
R01_DEVELOPER_OUTCOME: `READY_FOR_QA`.
R01_QA_OUTCOME: `REJECT / HIGH`.
R01_QA_ROOT_CAUSE: `WP04_PROVENANCE_STRUCTURAL_VALIDATION_MISSING`.
R01_QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R01-QA.md`, commit `a74ebab91450f212eb06dc963fabf24243ca9e4a`, blob `991c64776da2d198d5e8275bb28ffa281df5c459`.
R01_QA_TESTS: private `EVIDENCE/HQ-WP04-R01-QA-TESTS.py`, commit `b8227aeb2ab0141ae01a043752b65d4bb5b74b5b`, blob `ed36373205f9f0f8e5b747eb00fc20f9962f9c20`.
R01_REVIEWER_OUTCOME: `NOT_STARTED / NOT_AUTHORIZED_AFTER_QA_REJECT`.
The rejected R01 candidate is frozen as evidence and must not be reactivated unchanged.

### WP04 R02 terminal history
R02_CANDIDATE: `2c5ff49495ac2b0db969c308f4a6b1b837ff7822`.
R02_TREE: `32d5533f33fe27bd857849b6769901edd93176d1`.
R02_DEVELOPER_OUTCOME: `READY_FOR_QA`.
R02_DEVELOPER_EVIDENCE: private `EVIDENCE/HQ-WP04-R02-DEVELOPER.md`, commit `d79a24b73eaf88e82bfb683911655681c23fcd9f`, blob `dd1b50b60a398b170a6acd076080e9190822558b`.
R02_QA_OUTCOME: `REJECT / HIGH`.
R02_QA_ROOT_CAUSE: `WP04_REVIEW_AUTHOR_INDEPENDENCE_NOT_ENFORCED`.
R02_QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R02-QA.md`, commit `381c0854840faa376e31b658a492d8a0337a22f5`, blob `d6b4b1fdc5722c352cccec54497a801db9a5ca0d`.
R02_QA_TESTS: private `EVIDENCE/HQ-WP04-R02-QA-TESTS.py`, commit `d37e9eecb7775b8036a528e94cb40fb2e7ca23ba`, blob `3714e1fb0253520fb2afbaab570329c4590f0edc`.
R02_QA_SUMMARY: returned R01 defect is closed; candidate suite `13/13 PASS`, preserved R01 independent regressions `10/10 PASS`, affected accepted WP01-WP03 regressions `15/15 PASS`; new independent R02 suite `15 tests = 13 PASS / 2 FAIL` because Developer-owned or QA-owned Review evidence can still expose authoritative PASS without independent Reviewer authority.
R02_REVIEWER_OUTCOME: `NOT_STARTED / NOT_AUTHORIZED_AFTER_QA_REJECT`.
The rejected R02 candidate is frozen as evidence and must not be reactivated unchanged.

### Current WP04 dispatch
PHASE: `QA`
ROUND: `R03`
ATTEMPT_ID: `R03`
TASK_ID: `HQ-QA-WP04-API-R03`
ACTIVE_OWNER: `HQ-QA-01`
RUN_STATUS: `QA_DISPATCH_READY`
INPUT_CANDIDATE: `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`
INPUT_TREE: `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`
BUILD_BRANCH: `build/wp04-status-evidence-api-001`
CURRENT_CANDIDATE: `2c10e1772c87f3791850f4f7db17551d881db90c`.
CURRENT_CANDIDATE_TREE: `4c88623c238902471a4976159367fa815bb3653c`.
CANDIDATE_DIFF_BASE: rejected R02 `2c5ff49495ac2b0db969c308f4a6b1b837ff7822`.
CANDIDATE_DIFF_STATUS: `VERIFIED_MATERIALLY_NEW_R03` — R02→R03 `ahead_by=2 / behind_by=0`; accepted WP03→R03 `ahead_by=9 / behind_by=0`; exactly two WP04 allow-list paths.
CURRENT_CHANGED_BLOBS: `status_api.py@75ce8ac1b6e0e0808541a478c8008ea731558391`; `tests/test_status_api.py@c3753905455a0caa8e966cb3c4b7e90d0a3d6c8b`.
DEVELOPER_OUTCOME: `READY_FOR_QA`.
DEVELOPER_EVIDENCE: private `EVIDENCE/HQ-WP04-R03-DEVELOPER.md`, commit `9b2d8c7d0b31b8be3b3cd34fba9060b02fad3a1d`, blob `d28e0d01ce876ec4ea92e1b0e83a707a8698b0c2`.
DEVELOPER_CHECKPOINT: `NOT_PRESENT / TERMINAL_EVIDENCE_SUFFICIENT`.
QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R03-QA.md` — `PENDING`.
QA_TESTS: private `EVIDENCE/HQ-WP04-R03-QA-TESTS.py` — `PENDING`.
REVIEWER_EVIDENCE: private `EVIDENCE/HQ-WP04-R03-REVIEWER.md` — `NOT_STARTED`.
RETURNED_FROM_ROUND: `R02`.
RETURNED_QA_OUTCOME: `REJECT / HIGH`.
RETURNED_QA_ROOT_CAUSE: `WP04_REVIEW_AUTHOR_INDEPENDENCE_NOT_ENFORCED`.
REJECTED_ROUNDS: `2/3`.
SAME_ROOT_REJECT_COUNT: `1/2` for the current root cause.
CURRENT_BLOCKER: `NONE`.
LAST_TRANSITION_AT: `2026-09-18T17:20:00Z`.
QA_WORKER_STATE: `DISABLED / ENABLE_AFTER_REQUIRED_READBACK`.

HQ-REGISTRAR-01 verified the terminal R03 Developer `READY_FOR_QA` handoff, exact candidate/tree, materially new ahead-only lineage and two-path allow-list diff, pinned immutable Developer evidence commit/blob, and confirmed the Developer worker is already stopped. Dispatch is now pinned to independent HQ-QA-01; QA enable follows only after required private/public read-back. Reviewer remains dependency-gated.

### WP04 R03 QA boundary
R03 is the final candidate round. Independent QA must test exact candidate `2c10e1772c87f3791850f4f7db17551d881db90c` / tree `4c88623c238902471a4976159367fa815bb3653c` and must not implement fixes.
The returned R02 defect is `WP04_REVIEW_AUTHOR_INDEPENDENCE_NOT_ENFORCED`: Developer-owned or QA-owned valid Review evidence must not authorize independent-review PASS/REJECT and must fail closed to `UNKNOWN`; valid independently identified Reviewer evidence must remain compatible. Independence may not be inferred from filename/path alone.
Persisted R02 independent QA tests are mandatory unchanged returned input. R01 malformed-provenance regressions, candidate WP04 tests and affected accepted WP01-WP03 provenance/identity/security regressions must remain green.
Developer author verification reports compile PASS and `57/57` regressions green, but that is not independent QA.
Network-backed `GitHubApiSource` remains explicitly `NOT_TESTED` unless independently exercised with reproducible evidence.
Any R03 QA/Reviewer REJECT exhausts the max-three-round budget; a repeat of the R02 root cause also reaches the two-same-root stop rule.

### WP04 contract
Goal: minimal read-only Status / Evidence API over accepted WP01-WP03 derived state, exposing projects, agents, tasks, reviews, Human Gates, incidents/evidence and freshness/conflict flags.
Every outward status must have source/evidence provenance or explicit `UNKNOWN`.
GitHub remains source of truth; the API is derived/rebuildable; Scheduled Wake remains unchanged.
Preserve fail-closed provenance/identity/security and truthful `STALE_PROJECTION`, `MISSING_REVIEW`, `CONFLICT`, `UNKNOWN` semantics. No false READY/PASS.
No arbitrary repository-write endpoint, production/deploy, merge-to-main, WP05/WP06, permission/workflow change, provider/runtime replacement or legacy/remote activation is authorized during active WP04.

### Architecture-strengthening gate
#20 `ARCHITECTURE FREEZE v1` remains OPEN / gates pending under `OWNER_2026-09-18_ARCHITECTURE_STRENGTHENING`.
#21 `EVIDENCE-REF-01`, #22 `GITHUB-SOURCE-01`, and #23 `BUILD-WP05` remain provisioned behind final exact WP04 Control acceptance and are not active during R03 QA.
This Registrar does not declare Architecture Freeze PASS; the separate freeze control owns that gate.

### HQ-REGISTRAR-01
SCHEDULER_TASK_ID: `6aac1f2261a48191805ee42fa01ec632`
STATUS: `ACTIVE_WP04_REGISTRAR`
AUTHORITY: sole routine WP04 loop/execution/public-HQ-state and worker-lifecycle writer; no implementation, QA, Reviewer verdict, merge or Freeze-PASS authority.

### HQ-DEVELOPER-01
SCHEDULER_TASK_ID: `6aac9020d68c8191af4cee8bd53e374b`
ASSIGNMENT_STATE: `TERMINAL_READY_FOR_QA_WP04_R03`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-DEVELOPER-01-WP04.md`
CURRENT_TASK: terminal `HQ-DEV-WP04-API-R03`; exact candidate frozen.
SCHEDULER_STATE: disabled after terminal R03 handoff; must not repeat unchanged candidate.
NEXT_STEP: none unless Registrar later returns a permitted correction; no R04 is authorized after any R03 reject.

### HQ-QA-01
SCHEDULER_TASK_ID: `6aac3099fc9881919e9de980b9fd86a7`
ASSIGNMENT_STATE: `ASSIGNED_WP04_R03_QA`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-QA-WP04.md`
CURRENT_TASK: `HQ-QA-WP04-API-R03` on exact candidate `2c10e1772c87f3791850f4f7db17551d881db90c` / tree `4c88623c238902471a4976159367fa815bb3653c`.
SCHEDULER_STATE: disabled pending required private/public read-back; Registrar may then enable the existing worker.
NEXT_STEP: one independent terminal R03 QA result only, then stop.

### HQ-REVIEWER-01
SCHEDULER_TASK_ID: `6aac30a8f27c819198aea8a734aeaf5a`
ASSIGNMENT_STATE: `ARMED_CONDITIONAL_WP04`
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-REVIEWER-WP04.md`
SCHEDULER_STATE: disabled until exact same-candidate independent R03 QA is `READY_FOR_REVIEW` and Registrar moves dispatch to REVIEW.

### HQ-DEVELOPER-02
STATUS: disabled for WP04 core/API. #23 is provisioned but remains gated by final WP04 Control acceptance and may not edit backend/API.

### HQ-CONTROL-01
ROLE: bounded supervisor and final scoped WP04 judge only; Registrar owns routine lifecycle/state transitions.
CURRENT_STATE: WP04 R03 has a materially new exact Developer `READY_FOR_QA` candidate and is dispatched to independent QA; no R03 QA, Reviewer or Control PASS exists yet.

## WP04 lifecycle
Developer `READY_FOR_QA` -> Registrar pins exact materially new candidate/tree/diff/evidence, disables Developer, moves to QA, reads back, then enables existing QA.
Independent same-candidate QA `READY_FOR_REVIEW` -> Registrar disables QA, pins report/tests, moves to REVIEW, reads back, then enables existing Reviewer.
In-scope QA/Reviewer `REJECT` -> same Developer receives a materially new round only while the max-three-candidate-round budget remains. R03 is final; any R03 reject stops the correction loop.
Reviewer `PASS` -> workers stop and Registrar routes `READY_FOR_CONTROL_REVIEW`. Final WP04 acceptance belongs to Control only.
After final WP04 Control acceptance only, the separately prepared post-WP04 disjoint lanes may be reconciled and activated under #21-#23; not before.

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
WP04 R01 and R02 are terminal independent-QA REJECT and frozen as evidence. WP04 R03 now has a materially new exact Developer `READY_FOR_QA` candidate and is dispatched to independent QA. Independent same-candidate R03 QA `READY_FOR_REVIEW`, independent Reviewer PASS and final Control acceptance are still required. No full-system `MISSION_COMPLETE`, merge, production, WP06 or Architecture Freeze PASS is declared.
