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
ACTIVE_PROJECTS: `PROJECT-CLAB-001`; current owner authority `OWNER_2026-09-18_CONTINUE_TO_WP04` under #18
CAPABILITIES: factual scheduled Registrar GitHub read/write execution; one active bounded implementation worker for WP04 core/API; distinct existing QA/Reviewer workers dependency-gated for independent same-candidate checks; bounded Control supervision
QUALIFICATION_EVIDENCE: #11 factual automated wake/read-back; accepted WP01 Reviewer PASS; accepted WP02 Reviewer PASS; #15 final `CONTROL_ACCEPTED / WP03_R02_BOUNDED_PASS` on exact WP03 R02 candidate; #18 current WP04 owner authority; private `HQ-WP04-LOOP-001.md` and reconciled `EXECUTION-STATE.md`; scheduler observations for the reused HQ workers
CURRENT_LOAD: BUILD-WP04 R01 development — minimal read-only Status / Evidence API based on accepted WP03 candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`
STATUS: `WP04_R01_DEVELOPMENT_ACTIVE`
WRITE_MODE: Registrar is sole routine WP04 loop/execution/public-HQ-state and worker-lifecycle writer; Developer/QA/Reviewer evidence remains role-owned; Control is final scoped judge only
ASSIGNMENT/CONTROL_ISSUE: #18 WP04 authority/work package
AUTOMATION_ID: `6aac1f2261a48191805ee42fa01ec632`
LAST_CONTACT_EVIDENCE: Registrar reconciled owner-authorized WP04 R01 DEVELOPMENT to private execution state and public HQ projection; no WP04 Developer terminal artifact/checkpoint existed at reconciliation
CURRENT_OWNER: `HQ-DEVELOPER-01`
CURRENT_TASK: `HQ-DEV-WP04-API-R01`
NEXT_STEP: Developer publishes one materially new immutable WP04 candidate plus `EVIDENCE/HQ-WP04-R01-DEVELOPER.md` with `READY_FOR_QA` or truthful `BLOCKED`; Registrar then performs dependency-safe lifecycle routing without owner relay
ROUND_BUDGET: WP04 rejected candidate rounds `0/3`; same-root rejects `0/2`
INPUT_BASE: frozen accepted WP03 candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`, tree `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`
KNOWN_LIMITATION: network-backed `GitHubApiSource` remains `NOT_TESTED` unless WP04 independently exercises it with evidence
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