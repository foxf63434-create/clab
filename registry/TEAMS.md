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
CAPABILITIES: factual scheduled Registrar GitHub read/write execution; one bounded HQ developer repair runtime with private branch/evidence writes and executed tests; distinct existing QA/Reviewer workers with dependency-gated schedules and current-round independent evidence
QUALIFICATION_EVIDENCE: #11 factual automated wake/read-back; #16 R02 developer terminal `READY_FOR_QA` for exact candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`; #13 R02 independent QA terminal `READY_FOR_REVIEW` with persisted current-round tests; #14 R02 independent Reviewer terminal `PASS` for the same candidate; private repair-loop/execution-state read-back; scheduler observations under #12/#15
CURRENT_LOAD: `HQ-WP-001` / #12; frozen WP03 R02 bounded repair package awaiting final Control review on exact candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`
STATUS: `READY_FOR_CONTROL_REVIEW / FINAL_BOUNDED_ACCEPTANCE_PENDING`
WRITE_MODE: Registrar is sole ordinary loop/execution/public-HQ-state writer; role evidence remains role-owned in private core; Control owns final bounded acceptance
ASSIGNMENT/CONTROL_ISSUE: #12 parent work package; #16 developer; #13 QA; #14 Reviewer; #15 bounded Control supervision/final acceptance
AUTOMATION_ID: `6aac1f2261a48191805ee42fa01ec632`
LAST_CONTACT_EVIDENCE: Registrar directly verified and pinned the R02 independent Reviewer terminal `PASS` at commit `2b1247b32619040a3708bcd94d4d052f616d2519` / blob `7a859d5225b8915be9511c34e321c0a77bc6ab01`, confirmed Developer/QA/Reviewer repeat workers are disabled, froze the exact candidate/evidence chain and submitted `READY_FOR_CONTROL_REVIEW`
CURRENT_OWNER: `HQ-CONTROL-01`
CURRENT_TASK: `HQ-CONTROL-001`
NEXT_STEP: Control independently verifies the frozen R02 developer -> QA -> Reviewer chain and makes the final bounded acceptance decision; no merge, production, WP04 or full-system completion follows from Reviewer PASS alone
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
