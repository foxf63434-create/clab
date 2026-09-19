# TEAM REGISTRY

STATUS: ACTIVE
LAST_RECONCILED: 2026-09-19

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
ACTIVE_PROJECTS: `PROJECT-CLAB-001`; current authorities `OWNER_2026-09-18_CONTINUE_TO_WP04` under #18, narrow recovery authority `HQ-CONTROL-WP04-RECOVERY-20260918-01` under #18 comment `5735952527`, and `OWNER_2026-09-18_ARCHITECTURE_STRENGTHENING` under #20-#23
CAPABILITIES: factual scheduled Registrar GitHub read/write execution; bounded implementation worker reuse; distinct existing QA/Reviewer workers for independent same-candidate checks; bounded Control supervision; post-WP04 disjoint lanes provisioned but gated by final WP04 Control acceptance
QUALIFICATION_EVIDENCE: #11 factual automated wake/read-back; accepted WP01 Reviewer PASS; accepted WP02 Reviewer PASS; #15 final `CONTROL_ACCEPTED / WP03_R02_BOUNDED_PASS`; #18 WP04 authority; private `HQ-WP04-LOOP-001.md` and reconciled `EXECUTION-STATE.md`; WP04 R01 independent QA `REJECT / HIGH / WP04_PROVENANCE_STRUCTURAL_VALIDATION_MISSING`; R02 `REJECT / HIGH / WP04_REVIEW_AUTHOR_INDEPENDENCE_NOT_ENFORCED`; R03 `REJECT / HIGH / WP04_HUMAN_GATE_CONFLICT_NOT_RECONCILED`; distinct recovery authority authorized exactly one R04; R04 independent QA `REJECT / HIGH / WP04_INVALID_CANONICAL_IDENTITY_CAN_AUTHORIZE_STATUS`
CURRENT_LOAD: BUILD-WP04 terminal hold after the single added R04 recovery candidate `5d92dd1455a1090546a6295adf394f96b0fb2881`, tree `397b6b920e915c7d1cff82d73996a3de51f359d4`, independently failed QA; no active WP04 Developer/QA/Reviewer worker; post-WP04 lanes remain gated
STATUS: `WP04_R04_RECOVERY_EXTENSION_EXHAUSTED`
WRITE_MODE: Registrar is sole routine WP04 loop/execution/public-HQ-state and worker-lifecycle writer; Developer/QA/Reviewer evidence remains role-owned; Control is final scoped WP04 judge only; separate freeze control owns Architecture Freeze state
ASSIGNMENT/CONTROL_ISSUE: #18 WP04 authority/work package; #20-#23 architecture-strengthening gates remain waiting final WP04 Control acceptance
AUTOMATION_ID: `6aac1f2261a48191805ee42fa01ec632`
LAST_CONTACT_EVIDENCE: Registrar verified terminal R04 independent QA `REJECT / HIGH` on exact candidate `5d92dd1455a1090546a6295adf394f96b0fb2881` / tree `397b6b920e915c7d1cff82d73996a3de51f359d4`, pinned QA report commit `c95f619025c3de05828ad968fc65720d38b752db` / blob `1674ec054acc8d8f80c1d7c8cf40336ec1fa1e5d` and tests commit `04244292681ccf2b3d4026e00473e2f134cc9dea` / blob `a51fcf5336f546b6e1702198a25a0e0d987a3dfd`, accounted the single added round exactly once to `4/4`, and stopped the recovery extension at `2026-09-19T00:45:49Z`
CURRENT_OWNER: `NONE`
CURRENT_TASK: `NONE / WP04_R04_TERMINAL_STOP`
NEXT_STEP: no R05 under current authority; any further WP04 code round requires later valid explicit owner/control authority. Registrar remains on read-only discovery and makes no duplicate write on stable hold. Post-WP04 fan-out remains forbidden until exact WP04 same-candidate QA `READY_FOR_REVIEW`, Reviewer PASS and final Control acceptance exist.
ROUND_BUDGET: original WP04 rejected candidate budget `3/3` exhausted historically after R03; recovery authority added exactly one R04; current rejected rounds `4/4`; R04 root-cause occurrences `1`; no R05
INPUT_BASE: frozen accepted WP03 candidate `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`, tree `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`
R01_TERMINAL: candidate `50159a0c732e9dc212dbc8e4de18fc4bdefa7cfa`, tree `880ddda97bc46c77295e14e326b40e52eb5ed49c`; independent QA `REJECT / HIGH / WP04_PROVENANCE_STRUCTURAL_VALIDATION_MISSING`; Reviewer not authorized
R02_TERMINAL: candidate `2c5ff49495ac2b0db969c308f4a6b1b837ff7822`, tree `32d5533f33fe27bd857849b6769901edd93176d1`; independent QA `REJECT / HIGH / WP04_REVIEW_AUTHOR_INDEPENDENCE_NOT_ENFORCED`; Reviewer not authorized
R02_QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R02-QA.md`, commit `381c0854840faa376e31b658a492d8a0337a22f5`, blob `d6b4b1fdc5722c352cccec54497a801db9a5ca0d`; tests `EVIDENCE/HQ-WP04-R02-QA-TESTS.py`, commit `d37e9eecb7775b8036a528e94cb40fb2e7ca23ba`, blob `3714e1fb0253520fb2afbaab570329c4590f0edc`
R03_TERMINAL: candidate `2c10e1772c87f3791850f4f7db17551d881db90c`, tree `4c88623c238902471a4976159367fa815bb3653c`; independent QA `REJECT / HIGH / WP04_HUMAN_GATE_CONFLICT_NOT_RECONCILED`; Reviewer not authorized; historical original 3/3 stop remains preserved
R03_DEVELOPER_EVIDENCE: private `EVIDENCE/HQ-WP04-R03-DEVELOPER.md`, commit `9b2d8c7d0b31b8be3b3cd34fba9060b02fad3a1d`, blob `d28e0d01ce876ec4ea92e1b0e83a707a8698b0c2`
R03_QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R03-QA.md`, commit `5af4362a53214c206d3e81b25f7910dfc2f7c95a`, blob `a12030977b44d23da9d25356199277a943537f71`; tests `EVIDENCE/HQ-WP04-R03-QA-TESTS.py`, commit `9d36df904fbd386154b8b85c96d36417c9a96b70`, blob `5ccef573ab8eb3d8e8c08fe0f42cc78e625fab19`
R04_TERMINAL: candidate `5d92dd1455a1090546a6295adf394f96b0fb2881`, tree `397b6b920e915c7d1cff82d73996a3de51f359d4`; independent QA `REJECT / HIGH / WP04_INVALID_CANONICAL_IDENTITY_CAN_AUTHORIZE_STATUS`; Reviewer not authorized; recovery extension exhausted; no R05
R04_DEVELOPER_EVIDENCE: private `EVIDENCE/HQ-WP04-R04-DEVELOPER.md`, commit `930d939751633f3249b92064f7decb0eb362438a`, blob `f65b44019420d0f546b8eb3327b4885a5bd1db5e`
R04_QA_EVIDENCE: private `EVIDENCE/HQ-WP04-R04-QA.md`, commit `c95f619025c3de05828ad968fc65720d38b752db`, blob `1674ec054acc8d8f80c1d7c8cf40336ec1fa1e5d`; tests `EVIDENCE/HQ-WP04-R04-QA-TESTS.py`, commit `04244292681ccf2b3d4026e00473e2f134cc9dea`, blob `a51fcf5336f546b6e1702198a25a0e0d987a3dfd`; QA executed 95 tests = 93 PASS / 2 FAIL plus compile PASS; C09 FAIL and C12 PARTIAL/FAIL
DEVELOPER_WORKER_STATE: existing worker `6aac9020d68c8191af4cee8bd53e374b` disabled/stopped; no further WP04 implementation authority under current recovery decision
QA_WORKER_STATE: existing worker `6aac3099fc9881919e9de980b9fd86a7` disabled/stopped after terminal R04 REJECT
REVIEWER_WORKER_STATE: existing worker `6aac30a8f27c819198aea8a734aeaf5a` disabled/not authorized after R04 QA REJECT
KNOWN_LIMITATION: network-backed `GitHubApiSource` remains `NOT_TESTED`; #22 is provisioned to close it only after WP04 Control acceptance
POST_WP04_GATES: #21 EvidenceRef hardening, #22 live GitHub source proof, #23 WP05 UI are provisioned but inactive because final exact WP04 Control acceptance does not exist
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