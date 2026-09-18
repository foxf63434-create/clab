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
ACTIVE_PROJECTS: `PROJECT-CLAB-001`; current authorities `OWNER_2026-09-18_CONTINUE_TO_WP04` under #18 and `OWNER_2026-09-18_ARCHITECTURE_STRENGTHENING` under #20-#23
CAPABILITIES: factual scheduled Registrar GitHub read/write execution; one bounded implementation worker for active WP04 core/API; distinct existing QA/Reviewer workers for independent same-candidate checks; bounded Control supervision; post-WP04 disjoint lanes provisioned but gated by final WP04 Control acceptance
QUALIFICATION_EVIDENCE: #11 factual automated wake/read-back; accepted WP01 Reviewer PASS; accepted WP02 Reviewer PASS; #15 final `CONTROL_ACCEPTED / WP03_R02_BOUNDED_PASS`; #18 WP04 authority; private `HQ-WP04-LOOP-001.md` and reconciled `EXECUTION-STATE.md`; WP04 R01 Developer `READY_FOR_QA` then independent QA `REJECT / HIGH / WP04_PROVENANCE_STRUCTURAL_VALIDATION_MISSING`; materially new WP04 R02 Developer `READY_FOR_QA`; independent R02 QA `REJECT / HIGH / WP04_REVIEW_AUTHOR_INDEPENDENCE_NOT_ENFORCED`; immutable R02 QA report/tests; no Reviewer authorization for either rejected candidate
CURRENT_LOAD: BUILD-WP04 final bounded R03 correction active with HQ-DEVELOPER-01; no R03 candidate yet; QA terminal/stopped after R02 reject; Reviewer dependency-gated
STATUS: `WP04_R03_DEVELOPMENT_ACTIVE`
WRITE_MODE: Registrar is sole routine WP04 loop/execution/public-HQ-state and worker-lifecycle writer; Developer/QA/Reviewer evidence remains role-owned; Control is final scoped WP04 judge only; separate freeze control owns Architecture Freeze state
ASSIGNMENT/CONTROL_ISSUE: #18 WP04 authority/work package; #20-#23 architecture-strengthening gates remain waiting final WP04 Control acceptance
AUTOMATION_ID: `6aac1f2261a48191805ee42fa01ec632`
LAST_CONTACT_EVIDENCE: Registrar verified exact R02 independent QA terminal `REJECT / HIGH` on candidate `2c5ff49495ac2b0db969c308f4a6b1b837ff7822` / tree `32d5533f33fe27bd857849b6769901edd93176d1`, preserved QA report commit `381c0854840faa376e31b658a492d8a0337a22f5` / blob `d6b4b1fdc5722c352cccec54497a801db9a5ca0d` and persisted tests commit `d37e9eecb7775b8036a528e94cb40fb2e7ca23ba` / blob `3714e1fb0253520fb2afbaab570329c4590f0edc`, routed final R03 correction at `2026-09-18T16:36:15Z`, completed required read-back, and enabled the existing HQ-DEVELOPER-01 worker at `2026-09-18T16:39:56Z`
CURRENT_OWNER: `HQ-DEVELOPER-01`
CURRENT_TASK: `HQ-DEV-WP04-API-R03`
NEXT_STEP: HQ-DEVELOPER-01 must publish exactly one materially new R03 `READY_FOR_QA` candidate or truthful `BLOCKED`, then stop; QA and Reviewer remain stopped until dependency-safe routing
ROUND_BUDGET: WP04 rejected candidate rounds `2/3`; current root-cause occurrences `1/2`; R03 is the final available candidate round
INPUT_BASE: frozen accepted WP03 candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`, tree `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`
R01_TERMINAL: candidate `50159a0c732e9dc212dbc8e4de18fc4bdefa7cfa`, tree `880ddda97bc46c77295e14e326b40e52eb5ed49c`; independent QA `REJECT / HIGH / WP04_PROVENANCE_STRUCTURAL_VALIDATION_MISSING`; Reviewer not authorized
R02_TERMINAL: candidate `2c5ff49495ac2b0db969c308f4a6b1b837ff7822`, tree `32d5533f33fe27bd857849b6769901edd93176d1`; independent QA `REJECT / HIGH / WP04_REVIEW_AUTHOR_INDEPENDENCE_NOT_ENFORCED`; Reviewer not authorized
R02_QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R02-QA.md`, commit `381c0854840faa376e31b658a492d8a0337a22f5`, blob `d6b4b1fdc5722c352cccec54497a801db9a5ca0d`; tests `EVIDENCE/HQ-WP04-R02-QA-TESTS.py`, commit `d37e9eecb7775b8036a528e94cb40fb2e7ca23ba`, blob `3714e1fb0253520fb2afbaab570329c4590f0edc`
R03_CANDIDATE: `PENDING_MATERIALLY_NEW`
DEVELOPER_WORKER_STATE: existing worker `6aac9020d68c8191af4cee8bd53e374b` enabled at `2026-09-18T16:39:56Z` after required read-back
QA_WORKER_STATE: existing worker `6aac3099fc9881919e9de980b9fd86a7` disabled after terminal R02 QA
REVIEWER_WORKER_STATE: existing worker `6aac30a8f27c819198aea8a734aeaf5a` disabled/dependency-gated
KNOWN_LIMITATION: network-backed `GitHubApiSource` remains `NOT_TESTED`; #22 is provisioned to close it only after WP04 Control acceptance
POST_WP04_GATES: #21 EvidenceRef hardening, #22 live GitHub source proof, #23 WP05 UI are provisioned but inactive until final exact WP04 Control acceptance
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
