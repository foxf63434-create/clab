# CLAB CURRENT STATE

STATUS: ACTIVE_RECOVERY
LAST_CONTROL_AUDIT: 2026-09-17
SOURCE_OF_TRUTH: GitHub repository state + issue evidence

## Global control
CONTROL: NIGHTJET GLOBAL CONTROL
PRIVATE_CORE: `foxf63434-create/meta-sales-system`
PUBLIC_BUS: `foxf63434-create/clab`

## REMOTE-ADMIN-01
HISTORICAL_BOOTSTRAP_EVIDENCE: issue #1
PREVIOUS_CONTROL_TASK: issue #8 -> SUPERSEDED/CLOSED
ACTIVE_CONTROL_TASK: issue #10
STATUS: RESTART_REQUIRED / NOT_PROVEN_PERSISTENT
FACTUAL_EVIDENCE:
- external account previously entered CLAB and created GitHub Issue evidence;
- issue-backed operation is available;
- no recurring admin wakeup has yet been proven;
- no worker automation has yet been proven ONLINE.
RECOVERY_REQUIREMENTS:
1. existing REMOTE-ADMIN-01 chat receives one restart command;
2. Admin rereads CLAB from GitHub, not chat memory;
3. Admin creates/enables its own recurring hourly wakeup first when supported;
4. first successful admin wake/read-back is written to GitHub;
5. Admin itself creates the minimum functional worker set for real assignments;
6. at least one worker gets exact Issue binding, recurring wakeup when useful, and factual first wake/read-back evidence;
7. then normal Executor -> QA -> Reviewer execution continues.
NEXT_STEP: execute issue #10.

## Functional workforce rule
REMOTE-ADMIN creates and manages its own bounded functional team. GLOBAL CONTROL does not manually instantiate routine workers. Possible functions include Executor/Developer, Researcher, QA, Reviewer, Incident/Debug and Architect, but only when real work requires them. `AUTHOR != FINAL JUDGE` remains mandatory.

## REMOTE-ADMIN-02
BOOTSTRAP_ISSUE: #9
STATUS: READY_FOR_ONE_TIME_BOOTSTRAP / PAUSED_BY_CONTROL
CONTROL_DECISION: do not bootstrap REMOTE-ADMIN-02 until REMOTE-ADMIN-01 recovery path is factually proven or independently abandoned.

## REMOTE-PILOT-001
STATUS: ACTIVE_RECOVERY / RESTART_REQUIRED
MISSION: `missions/REMOTE-PILOT-001/MISSION.md`
CURRENT_CONTROL_ISSUE: #10
STATE_ISSUE: #7
WORKER_ASSIGNMENTS: #3, #4, #5, #6
MANUAL_ROLE_HUMAN_GATE: #2 superseded/closed.

## Known platform/integration constraints
1. External account evidence showed repository Contents API write attempt returning `403 Resource not accessible by integration`.
2. Therefore issue-backed task/evidence exchange is an explicitly supported mode.
3. A public repository does not grant arbitrary file-write permission to external GitHub accounts.
4. Scheduled wakeups are periodic, not continuous. Current design uses hourly recurring checks where supported.

## Control invariant
Do not declare any external Admin/team/worker ONLINE until there is factual evidence of:
- created automation/task;
- enabled recurring schedule where required;
- exact GitHub assignment binding;
- at least one successful wake/read-back.

## Restart invariant
A failed or unproven bootstrap is not patched indefinitely. GLOBAL CONTROL may supersede the prior control issue, open a clean recovery issue, preserve history as audit evidence, and require deterministic re-bootstrap from GitHub state.

This file is the reconciled read model. Historical issues remain audit evidence but are not current authority.