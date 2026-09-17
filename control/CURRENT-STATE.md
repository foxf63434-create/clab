# CLAB CURRENT STATE

STATUS: ACTIVE_BOOTSTRAP
LAST_CONTROL_AUDIT: 2026-09-17
SOURCE_OF_TRUTH: GitHub repository state + issue evidence

## Global control
CONTROL: NIGHTJET GLOBAL CONTROL
PRIVATE_CORE: `foxf63434-create/meta-sales-system`
PUBLIC_BUS: `foxf63434-create/clab`

## REMOTE-ADMIN-01
BOOTSTRAP_ISSUE: #1
CONTROL_TASK: #8
STATUS: BOOTSTRAPPED_NOT_YET_PROVEN_PERSISTENT
FACTUAL_EVIDENCE:
- Remote Admin bootstrap was recorded in issue #1.
- Task #8 requires WAKEUP-FIRST autonomous workforce bootstrap.
MISSING_EVIDENCE:
- no factual admin automation/task ID recorded yet;
- no enabled hourly cadence evidence recorded yet;
- no successful recurring wake/read-back evidence recorded yet;
- no worker automation has been proven ONLINE yet.
NEXT_STEP: REMOTE-ADMIN-01 must read issue #8, create/enable its own recurring wakeup first, evidence the first successful wake, then create workers as required.

## REMOTE-ADMIN-02
BOOTSTRAP_ISSUE: #9
STATUS: READY_FOR_ONE_TIME_BOOTSTRAP
FACTUAL_EVIDENCE:
- wakeup-first bootstrap task exists in issue #9.
MISSING_EVIDENCE:
- no factual REMOTE-ADMIN-02 bootstrap response yet;
- no admin wakeup evidence yet;
- no worker evidence yet.
NEXT_STEP: on the second account create one chat only and send: `Зайди в CLAB. Ты REMOTE-ADMIN-02. Открой issue #9 и выполни его полностью.`

## REMOTE-PILOT-001
STATUS: ACTIVE / WAITING_FOR_PERSISTENT_ADMIN_WAKE_EVIDENCE
MISSION: `missions/REMOTE-PILOT-001/MISSION.md`
CURRENT_CONTROL_ISSUE: #8
WORKER_ASSIGNMENTS: #3, #4, #5, #6
MANUAL_ROLE_HUMAN_GATE: #2 is superseded/closed and must not be used as the normal path.

## Known platform/integration constraints
1. External account evidence showed repository Contents API write attempt returning `403 Resource not accessible by integration`.
2. Therefore issue-backed task/evidence exchange is an explicitly supported mode.
3. A public repository does not grant arbitrary file-write permission to external GitHub accounts.
4. Scheduled wakeups are periodic, not continuous. Current design uses hourly recurring checks where supported.

## Control invariant
Do not declare any external Admin/team/worker ONLINE until there is factual evidence of:
- created automation/task;
- enabled recurring schedule;
- exact GitHub assignment binding;
- at least one successful wake/read-back.

This file is a reconciled read model. Historical issues remain audit evidence but may contain superseded instructions.