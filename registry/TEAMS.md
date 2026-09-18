# TEAM REGISTRY

STATUS: ACTIVE
LAST_RECONCILED: 2026-09-18

No team is considered ONLINE or QUALIFIED without factual evidence.

Fields per team:
- NODE_ID
- TEAM_ID
- ADMIN_AGENT_ID
- ACTIVE_PROJECTS
- CAPABILITIES
- QUALIFICATION_EVIDENCE
- CURRENT_LOAD
- STATUS
- WRITE_MODE
- ASSIGNMENT/CONTROL_ISSUE
- LAST_CONTACT_EVIDENCE

## Teams

### TEAM-HQ-001
NODE_ID: `NODE-HQ-01`
ADMIN_AGENT_ID: `HQ-REGISTRAR-01`
ACTIVE_PROJECTS: `PROJECT-CLAB-001`; scoped private-core handoff through issue #12 and bounded repair authority `HQ-REPAIR-AUTH-20260918-01`
CAPABILITIES: factual scheduled Registrar GitHub read/write execution; one bounded HQ developer runtime with private branch/evidence writes and executed tests; distinct existing QA/Reviewer workers with dependency-gated schedules and current-round independent evidence
QUALIFICATION_EVIDENCE: #11 factual automated wake/read-back; #16 R02 developer terminal `READY_FOR_QA` for exact candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`; #13 R02 independent QA terminal `READY_FOR_REVIEW` with persisted current-round tests; prior #14 R01 independent Reviewer terminal `REJECT / HIGH`; private repair-loop/execution-state read-back; scheduler observations under #12/#15
CURRENT_LOAD: `HQ-WP-001` / #12; WP03 identity repair `R02` in bounded independent Reviewer recheck on exact candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`
STATUS: `REPAIR_LOOP_ACTIVE / R02_REVIEW_ACTIVE`
WRITE_MODE: Registrar is sole ordinary loop/execution/public-HQ-state writer; role evidence remains role-owned in private core
ASSIGNMENT/CONTROL_ISSUE: #12 parent work package; #16 developer; #13 QA; #14 Reviewer; #15 bounded Control supervision
AUTOMATION_ID: `6aac1f2261a48191805ee42fa01ec632`
LAST_CONTACT_EVIDENCE: Registrar directly verified the R02 independent QA terminal `READY_FOR_REVIEW`, exact candidate-bound report/test artifact identities and absence of an R02 Reviewer terminal artifact/checkpoint, activated and remotely read back the Reviewer assignment, then enabled only the existing Reviewer worker
CURRENT_OWNER: `HQ-REVIEWER-01`
CURRENT_TASK: `HQ-REV-WP03-IDENTITY-R02`
NEXT_STEP: independent Reviewer publishes one exact-candidate `PASS`, `REJECT` or truthful `BLOCKED`; schedule enablement alone is not execution proof and Registrar owns the next bounded transition
ROUND_BUDGET: rejected candidate rounds `1/3`; same-root rejects `1/2`
NAMESPACE: all current HQ agents use `HQ-` IDs under `NODE-HQ-01 / TEAM-HQ-001`
LEGACY_LOCAL_POLICY: old ambiguous NIGHTJET/Njet Club chats are history-only; old execution stays disabled unless explicitly reauthorized

### TEAM-REMOTE-001
NODE_ID: `NODE-REMOTE-01`
ADMIN_AGENT_ID: `REMOTE-ADMIN-01`
ACTIVE_PROJECTS: `PROJECT-CLAB-001` / `REMOTE-PILOT-001`
CAPABILITIES: orchestration bootstrap discovered; worker automation capability not yet proven
QUALIFICATION_EVIDENCE: issue #1 proves factual admin bootstrap only
CURRENT_LOAD: recovery/control issue #10
STATUS: `RESTART_REQUIRED_NOT_ONLINE`
WRITE_MODE: `ISSUE_WRITE` currently evidenced; Contents write previously returned 403
ASSIGNMENT/CONTROL_ISSUE: #10
LAST_CONTACT_EVIDENCE: issue #1 historical bootstrap
MISSING_FOR_ONLINE: enabled recurring admin wakeup + successful wake/read-back + factual worker evidence

### TEAM-REMOTE-002
NODE_ID: `NODE-REMOTE-02`
ADMIN_AGENT_ID: `REMOTE-ADMIN-02`
ACTIVE_PROJECTS: none
CAPABILITIES: UNKNOWN
QUALIFICATION_EVIDENCE: none yet
CURRENT_LOAD: none; bootstrap paused
STATUS: `PAUSED_NOT_ONLINE`
WRITE_MODE: UNKNOWN until factual bootstrap
ASSIGNMENT/CONTROL_ISSUE: #9 paused by GLOBAL CONTROL
LAST_CONTACT_EVIDENCE: none from REMOTE-ADMIN-02 yet
MISSING_FOR_ONLINE: factual bootstrap + enabled recurring admin wakeup + successful CLAB read-back

## Identity rule
All teams and agents follow `control/IDENTITY-NAMESPACE-STANDARD.md`.
Registration is not ONLINE. Enabled scheduling, actual invocation, successful GitHub execution and accepted work are separate facts. Observe actual evidence before promotion; a product limitation is BLOCKED, not PASS.
