# CLAB CURRENT STATE

STATUS: ACTIVE_RECOVERY_AND_HQ_BOOTSTRAP
LAST_CONTROL_AUDIT: 2026-09-17
SOURCE_OF_TRUTH: GitHub repository state + issue evidence

## Global control
CONTROL: NIGHTJET GLOBAL CONTROL
PRIVATE_CORE: `foxf63434-create/meta-sales-system`
PUBLIC_BUS: `foxf63434-create/clab`
IDENTITY_STANDARD: `control/IDENTITY-NAMESPACE-STANDARD.md`

## PRIMARY HQ TEAM — NEW CLEAN PATH
NODE_ID: `NODE-HQ-01`
TEAM_ID: `TEAM-HQ-001`
ADMIN_AGENT_ID: `HQ-REGISTRAR-01`
BOOTSTRAP_ISSUE: #11
STATUS: `READY_FOR_BOOTSTRAP_NOT_ONLINE`
PURPOSE: clean primary NIGHTJET team inside Njet Club with unique namespace and no ambiguous legacy role names.
NEXT_STEP: create one new clean Njet Club chat for `HQ-REGISTRAR-01`, send the issue #11 bootstrap command, establish Registrar recurring wakeup first, then let Registrar create only the minimum functional workers needed for real assignments.
LEGACY_LOCAL_POLICY: old NIGHTJET/Njet Club chats are preserved as history but receive no new routine assignments unless explicitly reactivated and mapped to a unique HQ identity.

## REMOTE-ADMIN-01
NODE_ID: `NODE-REMOTE-01`
TEAM_ID: `TEAM-REMOTE-001`
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
NEXT_STEP: execute issue #10 only if/when GLOBAL CONTROL continues the remote pilot independently of HQ bootstrap.

## Functional workforce rule
Each Registrar/Admin creates and manages only its own bounded functional team. GLOBAL CONTROL does not manually instantiate routine workers. Possible functions include Executor/Developer, Researcher, QA, Reviewer, Incident/Debug and Architect, but only when real work requires them. `AUTHOR != FINAL JUDGE` remains mandatory.

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
Every active assignment must carry NODE_ID + TEAM_ID + AGENT_ID + PROJECT_ID + MISSION_ID. Bare names such as `Reviewer`, `Developer 02`, `Agent 01` are not canonical identities. HQ and remote teams are isolated by namespace and authority; cross-team authority requires explicit GLOBAL CONTROL routing.

## Known platform/integration constraints
1. External account evidence showed repository Contents API write attempt returning `403 Resource not accessible by integration`.
2. Therefore issue-backed task/evidence exchange is an explicitly supported mode.
3. A public repository does not grant arbitrary file-write permission to external GitHub accounts.
4. Scheduled wakeups are periodic, not continuous. Current design uses recurring checks where supported.

## Control invariant
Do not declare any Admin/Registrar/team/worker ONLINE until there is factual evidence of:
- created automation/task where applicable;
- enabled recurring schedule where required;
- exact GitHub assignment binding;
- at least one successful wake/read-back.

## Restart invariant
A failed or unproven bootstrap is not patched indefinitely. GLOBAL CONTROL may supersede the prior control issue, open a clean recovery issue, preserve history as audit evidence, and require deterministic re-bootstrap from GitHub state.

This file is the reconciled read model. Historical issues remain audit evidence but are not current authority.