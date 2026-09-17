# CLAB CURRENT STATE

STATUS: HQ_WAKE_ENABLED_EXECUTION_PENDING
LAST_CONTROL_AUDIT: 2026-09-17
SOURCE_OF_TRUTH: GitHub repository state + issue evidence + actual scheduler observations
CONTROL_DECISION: FIX_REQUIRED

## Global control
CONTROL: NIGHTJET GLOBAL CONTROL
PRIVATE_CORE: `foxf63434-create/meta-sales-system`
PUBLIC_BUS: `foxf63434-create/clab`
IDENTITY_STANDARD: `control/IDENTITY-NAMESPACE-STANDARD.md`

## PRIMARY HQ TEAM — CURRENT PATH
NODE_ID: `NODE-HQ-01`
TEAM_ID: `TEAM-HQ-001`
ADMIN_AGENT_ID: `HQ-REGISTRAR-01`
BOOTSTRAP_ISSUE: #11 (reopened; prior closeout not accepted as proof of autonomous operation)
ACTIVE_WORK_PACKAGE: #12 / `HQ-WP-001`
STATUS: `MANUAL_BOOTSTRAP_PROVEN / WAKE_ENABLED / AUTOMATED_EXECUTION_NOT_YET_PROVEN`
SCHEDULER_TASK_ID: `6aac1f2261a48191805ee42fa01ec632`
SCHEDULER_OBSERVATION: enabled=true; hourly recurrence; last_run_time=null at this control inspection.
EVIDENCE: #11 comment 5718377211 explicitly distinguishes manual bootstrap read-back from a future scheduled invocation. Comment 5718400476 closed the task without an actual scheduled-run record; this is not accepted as runtime proof.
WORKERS: none created/proven in the observed HQ scheduler state.
NEXT_STEP: on the existing Registrar's next scheduled wake, read #11 and #12 directly, publish truthful first automated read-back, and continue #12 in the same invocation when supported. #12 supplies actual handoff/recovery work and supersedes the earlier 'no HQ work package' observation.
NO_NEW_ADMIN_CHAT: do not create another Registrar or duplicate the enabled schedule.
LEGACY_LOCAL_POLICY: preserve old chats/history; legacy execution schedules remain disabled. Verify no overlapping active legacy run before transferring shared-state ownership.

## HQ acceptance correction
Created automation != scheduled execution != successful worker output != completed mission.
Absence of a synchronous run-now tool is not successful autonomous bootstrap. A proven limitation produces BLOCKED / LIMITATION_CONFIRMED, never PASS.
HQ-REGISTRAR-01 may submit READY_FOR_CONTROL_REVIEW; GLOBAL CONTROL checks actual scheduled read-back and required worker execution before closing #11. #12 is assigned but delivery/execution is not claimed until its own evidence exists.

## REMOTE-ADMIN-01
NODE_ID: `NODE-REMOTE-01`
TEAM_ID: `TEAM-REMOTE-001`
HISTORICAL_BOOTSTRAP_EVIDENCE: issue #1
PREVIOUS_CONTROL_TASK: issue #8 -> SUPERSEDED/CLOSED
CONTROL_TASK: issue #10
STATUS: RESTART_REQUIRED / NOT_PROVEN_PERSISTENT
FACTUAL_EVIDENCE:
- external account previously entered CLAB and created GitHub Issue evidence;
- issue-backed operation was available in that session;
- recurring admin wakeup and worker automation remain unproven in this control snapshot.
NEXT_STEP: execute issue #10 only if/when GLOBAL CONTROL continues the remote pilot independently of HQ bootstrap. HQ must not take remote-team assignments.

## Functional workforce rule
Each Registrar/Admin manages only its own bounded team using actual available tools. Start from an exact assignment and verify capabilities in the scheduled execution context. A role label or scheduled task is not proof of a distinct chat/isolated process. `AUTHOR != FINAL JUDGE` remains mandatory. Missing tools or permissions must be reported truthfully, not bypassed or simulated.

## REMOTE-ADMIN-02
NODE_ID: `NODE-REMOTE-02`
TEAM_ID: `TEAM-REMOTE-002`
BOOTSTRAP_ISSUE: #9
STATUS: PAUSED_BY_CONTROL / NOT_ONLINE
CONTROL_DECISION: do not bootstrap REMOTE-ADMIN-02 until GLOBAL CONTROL explicitly reactivates it.

## REMOTE-PILOT-001
STATUS: ACTIVE_RECOVERY / NOT_PROVEN_PERSISTENT
MISSION: `missions/REMOTE-PILOT-001/MISSION.md`
CURRENT_CONTROL_ISSUE: #10
STATE_ISSUE: #7
WORKER_ASSIGNMENTS: #3, #4, #5, #6
MANUAL_ROLE_HUMAN_GATE: #2 superseded/closed.

## Multi-account namespace invariant
Every active assignment must carry NODE_ID + TEAM_ID + AGENT_ID + PROJECT_ID + MISSION_ID. Bare names are not canonical identities. HQ and remote teams remain isolated; cross-team authority requires explicit routing.

## Known integration boundaries
External Contents API writes previously returned 403. Issue-backed task/evidence exchange is supported when actually available. Public visibility does not grant file-write permissions. Never export private code, logs, credentials, customer data or confidential reports into CLAB; use public-safe status and private artifact pointers. Recurring wakeups are periodic, not continuous.

## Progress and recovery
Keep existing useful work and accepted evidence. Do not reboot teams or recreate schedules merely because a scheduled invocation has not yet been recorded. Examine actual elapsed cadence, run evidence, tool availability and assignments first. Missing evidence is UNKNOWN, not proof of successful or failed execution.

This is a reconciled snapshot. Later actual evidence must be read before changing state. No full-system PASS or MISSION_COMPLETE is declared.
