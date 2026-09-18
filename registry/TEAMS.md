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
CAPABILITIES: factual scheduled Registrar GitHub read/write execution; one bounded implementation worker for WP04 core/API; distinct existing QA/Reviewer workers for independent same-candidate checks; bounded Control supervision
QUALIFICATION_EVIDENCE: #11 factual automated wake/read-back; accepted WP01 Reviewer PASS; accepted WP02 Reviewer PASS; #15 final `CONTROL_ACCEPTED / WP03_R02_BOUNDED_PASS` on exact WP03 R02 candidate; #18 current WP04 owner authority; private `HQ-WP04-LOOP-001.md` and reconciled `EXECUTION-STATE.md`; WP04 R01 Developer `READY_FOR_QA`; independent WP04 R01 QA `REJECT / HIGH / WP04_PROVENANCE_STRUCTURAL_VALIDATION_MISSING`; immutable R01 QA report/tests; materially new WP04 R02 Developer `READY_FOR_QA` candidate/evidence with verified ahead-only two-path diff; no pre-existing R02 QA terminal artifact/checkpoint before routing
CURRENT_LOAD: BUILD-WP04 R02 independent QA by HQ-QA-01 on exact candidate `2c5ff49495ac2b0db969c308f4a6b1b837ff7822`; Developer terminal/stopped; Reviewer dependency-gated
STATUS: `WP04_R02_QA_ACTIVE`
WRITE_MODE: Registrar is sole routine WP04 loop/execution/public-HQ-state and worker-lifecycle writer; Developer/QA/Reviewer evidence remains role-owned; Control is final scoped judge only
ASSIGNMENT/CONTROL_ISSUE: #18 WP04 authority/work package
AUTOMATION_ID: `6aac1f2261a48191805ee42fa01ec632`
LAST_CONTACT_EVIDENCE: Registrar verified exact R02 Developer terminal `READY_FOR_QA`, candidate `2c5ff49495ac2b0db969c308f4a6b1b837ff7822` / tree `32d5533f33fe27bd857849b6769901edd93176d1`, Developer evidence commit `d79a24b73eaf88e82bfb683911655681c23fcd9f` / blob `dd1b50b60a398b170a6acd076080e9190822558b`, verified accepted-WP03-base lineage `ahead_by=7 / behind_by=0` with exactly two authorized WP04 paths and R01->R02 `ahead_by=2 / behind_by=0`, confirmed no R02 QA terminal report/tests/checkpoint existed, observed Developer already stopped, and routed the exact candidate to independent QA at `2026-09-18T15:56:50Z`
CURRENT_OWNER: `HQ-QA-01`
CURRENT_TASK: `HQ-QA-WP04-API-R02`
NEXT_STEP: HQ-QA-01 must publish exactly one independent same-candidate `READY_FOR_REVIEW`, `REJECT` or truthful `BLOCKED`; Reviewer stays disabled until exact QA `READY_FOR_REVIEW`
ROUND_BUDGET: WP04 rejected candidate rounds `1/3`; same-root rejects `1/2`
INPUT_BASE: frozen accepted WP03 candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`, tree `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`
R01_TERMINAL: candidate `50159a0c732e9dc212dbc8e4de18fc4bdefa7cfa`, tree `880ddda97bc46c77295e14e326b40e52eb5ed49c`; independent QA `REJECT / HIGH`; Reviewer not authorized
R01_QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R01-QA.md`, commit `a74ebab91450f212eb06dc963fabf24243ca9e4a`, blob `991c64776da2d198d5e8275bb28ffa281df5c459`; tests `EVIDENCE/HQ-WP04-R01-QA-TESTS.py`, commit `b8227aeb2ab0141ae01a043752b65d4bb5b74b5b`, blob `ed36373205f9f0f8e5b747eb00fc20f9962f9c20`
R02_DEVELOPER_TERMINAL: candidate `2c5ff49495ac2b0db969c308f4a6b1b837ff7822`, tree `32d5533f33fe27bd857849b6769901edd93176d1`; Developer `READY_FOR_QA`; evidence commit `d79a24b73eaf88e82bfb683911655681c23fcd9f`, blob `dd1b50b60a398b170a6acd076080e9190822558b`
KNOWN_LIMITATION: network-backed `GitHubApiSource` remains `NOT_TESTED` unless WP04 independent QA actually exercises it with reproducible evidence
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