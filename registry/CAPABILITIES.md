# CAPABILITY REGISTRY

STATUS: ACTIVE
LAST_RECONCILED: 2026-09-17

Capability states:
- UNKNOWN
- DISCOVERED
- TRAINING_REQUIRED
- SANDBOX_QUALIFIED
- QUALIFIED
- SUSPENDED

A capability is QUALIFIED only with evidence appropriate to the task. Self-report alone is insufficient.

For missing capability use:
REUSE EXISTING MATERIAL -> FIND TRUSTED MATERIAL -> CREATE MINIMAL TRAINING PACK -> SANDBOX TASK -> INDEPENDENT ASSESSMENT -> QUALIFIED/REJECTED.

Fields:
- CAPABILITY_ID
- DESCRIPTION
- TEAM/AGENT
- STATUS
- SOURCE/TRAINING
- ASSESSMENT
- EVIDENCE
- LIMITATIONS
- LAST_VERIFIED

## Discovered capabilities

### CAP-CLAB-READ
DESCRIPTION: read public CLAB files/issues and reconstruct assigned bootstrap context
TEAM/AGENT: `REMOTE-ADMIN-01`
STATUS: DISCOVERED
SOURCE/TRAINING: CLAB bootstrap
ASSESSMENT: factual bootstrap issue shows required CLAB files were read
EVIDENCE: issue #1
LIMITATIONS: successful recurring wake/read-back not yet proven
LAST_VERIFIED: 2026-09-17

### CAP-CLAB-ISSUE-WRITE
DESCRIPTION: create GitHub Issues in CLAB for bootstrap/assignments/state
TEAM/AGENT: `REMOTE-ADMIN-01`
STATUS: DISCOVERED
SOURCE/TRAINING: CLAB operating protocol
ASSESSMENT: issues #1-#7 were created by the external account path
EVIDENCE: issues #1-#7
LIMITATIONS: repository Contents write was not available in the evidenced session
LAST_VERIFIED: 2026-09-17

### CAP-RECURRING-WAKE-MANAGEMENT
DESCRIPTION: create, enable and operate recurring admin/worker wakeups
TEAM/AGENT: `REMOTE-ADMIN-01`, `REMOTE-ADMIN-02`
STATUS: UNKNOWN
SOURCE/TRAINING: `control/REMOTE-ADMIN-BOOTSTRAP-STANDARD.md`
ASSESSMENT: pending factual automation/task evidence
EVIDENCE: none yet
LIMITATIONS: product/tool availability must be proven per account
LAST_VERIFIED: 2026-09-17

No remote capability is QUALIFIED yet for production use. Qualification must follow mission-specific evidence and independent assessment.