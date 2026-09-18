# CLAB CURRENT STATE

STATUS: HQ_REPAIR_R01_QA_ACTIVE
LAST_CONTROL_AUDIT: 2026-09-18
SOURCE_OF_TRUTH: GitHub state + actual scheduler observations + exact execution evidence
CONTROL_DECISION: CONTINUE_WITH_BOUNDED_REPAIR
AUTHORITY_VERSION: `HQ-REPAIR-AUTH-20260918-01`

## Global control
CONTROL: NIGHTJET GLOBAL CONTROL
PRIVATE_CORE: `foxf63434-create/meta-sales-system`
PUBLIC_BUS: `foxf63434-create/clab`
IDENTITY_STANDARD: `control/IDENTITY-NAMESPACE-STANDARD.md`
BOUNDED_CONTROL_ASSIGNMENT: #15 / `HQ-CONTROL-001`
CONTROL_AGENT: `NODE-HQ-01 / TEAM-HQ-001 / HQ-CONTROL-01`

## PRIMARY HQ TEAM — CURRENT PATH
NODE_ID: `NODE-HQ-01`
TEAM_ID: `TEAM-HQ-001`
ADMIN_AGENT_ID: `HQ-REGISTRAR-01`
PROJECT_ID: `PROJECT-CLAB-001`
MISSION_ID: `HQ-BOOTSTRAP-001`
BOOTSTRAP_ISSUE: #11 remains open until factual worker criteria and GLOBAL CONTROL acceptance.
ACTIVE_WORK_PACKAGE: #12 / `HQ-WP-001`
DEVELOPER_ISSUE: #16
QA_ISSUE: #13
REVIEWER_ISSUE: #14
CURRENT_PRIVATE_DISPATCH: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/HQ-REPAIR-LOOP-001.md`

### Current repair dispatch
PHASE: `QA`
ROUND: `R01`
ATTEMPT_ID: `R01-C02`
TASK_ID: `HQ-QA-WP03-IDENTITY-R01`
ACTIVE_OWNER: `HQ-QA-01`
RUN_STATUS: `QA_AUTHORIZED`
CANDIDATE_SHA: `be4868cd43e8bb8c26e26ecb9cffcc981491b0a2`
CANDIDATE_TREE: `621a30db4e95b5d7befe516cb78f1d424232deab`
CANDIDATE_DIFF_BASE: `c30b4f82bd91ed42492a6e06587340ea79fd682c`
DEVELOPER_RESULT: `READY_FOR_QA` at private `EVIDENCE/HQ-IDENTITY-R01-C02-DEVELOPER.md`.
DEVELOPER_EVIDENCE_COMMIT: `2e8c7d62cdf1bcca4ac85c77a8239624b564cad2`.
DEVELOPER_EVIDENCE_BLOB: `3f0671355335d349637c7fdf7526308d4c3e59db`.
CURRENT_QA_OUTPUT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/EVIDENCE/HQ-IDENTITY-R01-QA.md`.
CURRENT_QA_TESTS: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/EVIDENCE/HQ-IDENTITY-R01-QA-TESTS.py`.
CURRENT_BLOCKER: `NONE`.
REPAIR_BRANCH: `repair/hq-wp03-identity-001`.
REPAIR_BRANCH_BASE: `c30b4f82bd91ed42492a6e06587340ea79fd682c`.
OLD_REJECTED_CANDIDATE: `e823a05a799bc9a02cfe246c463b9f61fd9e4264` remains historical evidence only and is not an active target.
LAST_TRANSITION_AT: `2026-09-18T03:28:49Z`.

Registrar directly verified the R01-C02 developer terminal artifact, exact candidate/tree and baseline-to-candidate allow-list diff before routing. The current candidate differs from the repair baseline only in the authorized scanner, projection and HQ compatibility regression paths. Developer self-tests reported 37/37 PASS on verified bytes, but remain author evidence and are not independent QA acceptance.

The owner-approved authority `HQ-REPAIR-AUTH-20260918-01` resolves the former one-developer/team-capacity HOLD for this repair only. It authorizes exactly one HQ developer and the bounded Developer -> QA -> independent Reviewer -> correction loop. No second developer, WP04+, production, merge-to-main, permission change, legacy reactivation or remote-team activation is authorized.

### HQ-REGISTRAR-01
SCHEDULER_TASK_ID: `6aac1f2261a48191805ee42fa01ec632`
OBSERVATION: existing Registrar remains the sole routine writer of repair-loop/execution state and HQ public projection.
AUTHORITY: coordinate only the approved repair loop; do not implement, perform QA or write Reviewer verdicts.

### HQ-DEVELOPER-01
WORKER_ISSUE: #16
SCHEDULER_TASK_ID: `6aac9020d68c8191af4cee8bd53e374b`
ASSIGNMENT_STATE: `TERMINAL READY_FOR_QA / STOPPED FOR CURRENT CANDIDATE`.
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-DEVELOPER-01.md`.
PRIOR_R01_OUTPUT: `.../EVIDENCE/HQ-IDENTITY-R01-DEVELOPER.md` = `BLOCKED` and preserved.
CURRENT_ATTEMPT_OUTPUT: `.../EVIDENCE/HQ-IDENTITY-R01-C02-DEVELOPER.md` = `READY_FOR_QA` for candidate `be4868cd43e8bb8c26e26ecb9cffcc981491b0a2`.
OBSERVATION: repeat developer schedule is disabled after the terminal handoff.
NEXT_STEP: no further developer execution unless independent QA/Reviewer returns an authorized new repair round.

### HQ-QA-01
WORKER_ISSUE: #13
SCHEDULER_TASK_ID: `6aac3099fc9881919e9de980b9fd86a7`
OBSERVATION: existing QA task is enabled only after private QA phase/assignment read-back.
ASSIGNMENT_STATE: `ACTIVE / R01`.
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-QA-IDENTITY-001.md`.
PINNED_CANDIDATE: `be4868cd43e8bb8c26e26ecb9cffcc981491b0a2` / tree `621a30db4e95b5d7befe516cb78f1d424232deab`.
PINNED_DEVELOPER_EVIDENCE: commit `2e8c7d62cdf1bcca4ac85c77a8239624b564cad2` / blob `3f0671355335d349637c7fdf7526308d4c3e59db`.
REQUIRED_OUTPUTS: `.../EVIDENCE/HQ-IDENTITY-R01-QA.md` plus persisted `.../EVIDENCE/HQ-IDENTITY-R01-QA-TESTS.py`.
NEXT_STEP: independently execute the full current-round QA contract on the exact pinned candidate and produce one terminal `READY_FOR_REVIEW`, `REJECT` or `BLOCKED`; schedule enablement itself is not execution proof.

### HQ-REVIEWER-01
WORKER_ISSUE: #14
SCHEDULER_TASK_ID: `6aac30a8f27c819198aea8a734aeaf5a`
OBSERVATION: existing Reviewer task remains disabled while waiting for new same-candidate independent QA.
ASSIGNMENT_STATE: `ARMED_CONDITIONAL`.
PRIVATE_ASSIGNMENT: `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/ASSIGNMENTS/HQ-REVIEWER-IDENTITY-001.md`.
ACTIVATION: only after the loop enters `PHASE=REVIEW`, assigns `HQ-REVIEWER-01`, and pins materially complete current-round independent QA `READY_FOR_REVIEW` for candidate `be4868cd43e8bb8c26e26ecb9cffcc981491b0a2`. Historical Reviewer REJECT on the old candidate remains immutable evidence and cannot be bypassed.

### HQ-CONTROL-01
CONTROL_ISSUE: #15 / `HQ-CONTROL-001`.
ROLE: bounded supervision and final acceptance only; not an executor and not a competing routine state writer.
CURRENT_AUTHORITY: supervise the owner-approved repair loop and verify final scoped readiness. Registrar does not wait for a separate Control ACK for routine in-scope Developer -> QA -> Reviewer transitions already authorized by #12/#16.
LATEST_MATERIAL_DIAGNOSIS: #15 comment 5724086673 identified the prior R01 write-path collision and authorized the R01-C02 coordination continuation that has now produced the new QA candidate.

## Repair-loop lifecycle
Current candidate round remains `R01` of maximum three materially new candidate rounds. `R01-C02` was a coordination continuation and did not increment rejected-round counters. Registrar checks current-attempt/current-round terminal evidence before any worker activation. On developer `READY_FOR_QA`, disable developer repeat work, pin exact candidate/tree/diff/developer evidence, publish/read back QA ownership/phase, then enable existing QA; this transition has now occurred for R01. On QA `READY_FOR_REVIEW`, disable QA, pin exact QA report and persisted tests, publish/read back Reviewer ownership/phase, then enable existing Reviewer. An in-scope QA/Reviewer `REJECT` returns one new candidate round to the same developer, preserving immutable prior evidence. Stop automatic correction after three candidate rounds or two rejected rounds with the same root cause, or immediately on a new scope/security/architecture conflict. `BLOCKED` is never acceptance and does not justify blind rerun.

Reviewer PASS on a new pinned QA-backed candidate moves only this bounded repair toward `READY_FOR_CONTROL_REVIEW`; GLOBAL CONTROL performs final package acceptance. No automatic merge, production, WP04 or full-system `MISSION_COMPLETE` follows.

## Historical WP03 evidence boundary
The old candidate `e823a05a799bc9a02cfe246c463b9f61fd9e4264` has historical independent HQ QA `READY_FOR_REVIEW` followed by independent Reviewer `REJECT / REV-WP03-HQ-ID-001 / HIGH`. Both reports remain valid evidence for their tested candidate. The positive old QA does not override the Reviewer REJECT and does not authorize rerunning that candidate. Current work is on the materially new candidate pinned above.

## Legacy local policy
Preserve old chats/history; old NIGHTJET execution schedules remain disabled and receive no new work. No reactivation/repurposing without explicit current owner/control authority. Verify no overlapping active writer before shared-state transfer. Other accounts and unrelated automations are untouched.

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
This HQ control task does not grant authority over remote teams.

## Functional workforce and namespaces
Every participant/task has NODE_ID + TEAM_ID + AGENT_ID + PROJECT_ID + MISSION_ID. Unique names and actual assignment bindings are mandatory. A role label or schedule is not proof of an isolated process or independent review. AUTHOR != FINAL JUDGE.

The current repair uses one Registrar, exactly one authorized developer, the existing independent QA and Reviewer, plus #15 Control supervision. Do not create idle staff, duplicate workers, repeat terminal work or expand scope to keep schedules busy.

## Security and integration boundaries
CLAB is PUBLIC. Private source/logs/diagnostics/report contents, credentials, customer data and secrets stay private. Use sanitized identifiers/pointers. External Contents writes previously returned 403; issue-backed exchange is valid when actually available. Public visibility is not file-write permission.

Verify capabilities separately in each scheduled context. A tool available during interactive provisioning may not exist during a scheduled run. Failed writes must be reported in task output when GitHub reporting itself is unavailable.

## Progress and recovery
Use existing accepted work/checkpoints. No reboot merely because execution is pending. Read actual elapsed cadence and evidence before inferring a failure. Missing evidence is UNKNOWN/PENDING until the relevant observation justifies more. Hourly checks are periodic, not continuous.

This is a reconciled snapshot for the owner-authorized R01 independent QA transition. Later actual evidence must be read before changing state. No full-system PASS or MISSION_COMPLETE is declared.
