# PROJECT REGISTRY

STATUS: ACTIVE
LAST_RECONCILED: 2026-09-17

Public-safe registry of projects participating in CLAB.

Required fields per project:
- PROJECT_ID
- NAME
- REPOSITORY / WORKSPACE POINTER
- VISIBILITY
- OWNER/CONTROL
- PROJECT_CONTROLLER / REMOTE_ADMIN
- PRIORITY
- STATUS
- REQUIRED_CAPABILITIES
- ACTIVE_MISSION
- HUMAN_GATE_STATE
- LAST_VERIFIED_EVIDENCE

## Registered

### PROJECT-CLAB-001
NAME: CLAB multi-account agent coordination pilot
REPOSITORY: `foxf63434-create/clab`
VISIBILITY: PUBLIC
OWNER/CONTROL: NIGHTJET GLOBAL CONTROL
PROJECT_CONTROLLER / REMOTE_ADMIN: `REMOTE-ADMIN-01` for `REMOTE-PILOT-001`; `REMOTE-ADMIN-02` is a separate account bootstrap node awaiting proof
PRIORITY: P0 pilot
STATUS: `ACTIVE_BOOTSTRAP`
REQUIRED_CAPABILITIES: orchestration, GitHub coordination, task decomposition, recurring wake management, QA, independent review
ACTIVE_MISSION: `missions/REMOTE-PILOT-001/`
HUMAN_GATE_STATE: NONE currently proven; historical issue #2 is superseded/closed
LAST_VERIFIED_EVIDENCE:
- repository visibility verified PUBLIC;
- REMOTE-ADMIN-01 factual bootstrap exists in issue #1;
- control task #8 requires wakeup-first persistent orchestration;
- REMOTE-ADMIN-02 bootstrap issue #9 exists but has no factual admin response yet;
- no external admin is ONLINE until recurring wake evidence exists.

Private projects may be represented only by sanitized identifiers and safe pointers. Do not copy confidential content here.