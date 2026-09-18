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
QUALIFICATION_EVIDENCE: #11 factual automated wake/read-back; #16 R01-C02 developer terminal `READY_FOR_QA`; #13 R01 independent QA terminal `READY_FOR_REVIEW`; private repair-loop/execution-state read-back; scheduler observations under #12/#15
CURRENT_LOAD: `HQ-WP-001` / #12; WP03 identity repair `R01` now in independent Reviewer on exact candidate `be4868cd43e8bb8c26e26ecb9cffcc981491b0a2`
STATUS: `REPAIR_LOOP_ACTIVE / R01_REVIEW_ACTIVE`
WRITE_MODE: Registrar is sole ordinary loop/execution/public-HQ-state writer; role evidence remains role-owned in private core
ASSIGNMENT/CONTROL_ISSUE: #12 parent work package; #16 developer; #13 QA; #14 Reviewer; #15 bounded Control supervision
AUTOMATION_ID: `6aac1f2261a48191805ee42fa01ec632`
LAST_CONTACT_EVIDENCE: #13 R01 QA `READY_FOR_REVIEW`; private QA artifact commit `88e4b7bf5f0a883323546ee86a755f750f6c5048` / blob `bf79ef0b2c16842ca35dc5acfb77a8a6127038db`; persisted QA tests commit `b083cd7b8ebd57e9faf4d85642d54da4022a7a1c` / blob `1e4a579ce00b72677f6182490aa0fe01782c7cf8`; Registrar routed exact candidate to independent Reviewer after read-back
CURRENT_OWNER: `HQ-REVIEWER-01`
CURRENT_TASK: `HQ-REV-WP03-IDENTITY-R01`
NEXT_STEP: independent Reviewer produces one exact-candidate current-round terminal `PASS`, `REJECT` or `BLOCKED`; no developer/QA repeat work on unchanged R01 candidate
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
