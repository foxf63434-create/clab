# REMOTE-PILOT-001 — MULTI-ACCOUNT TEAM BOOTSTRAP TEST

STATUS: ACTIVE_AUTONOMOUS_BOOTSTRAP
PROJECT_ID: PROJECT-CLAB-001
CONTROL: NIGHTJET GLOBAL CONTROL
PRODUCTION: FORBIDDEN
PUBLIC_REPO: YES
CANONICAL_STATE: `control/CURRENT-STATE.md` + Issue #7
CURRENT_ADMIN_CONTROL_TASK: Issue #8

## Goal
Prove that a ChatGPT account other than the current Global Control account can enter CLAB, assume REMOTE-ADMIN-01, establish a persistent recurring admin wakeup, create and coordinate a minimal local worker set, divide a bounded mission, collect evidence, use independent QA/Reviewer roles, and return a trustworthy result through GitHub without manual forwarding of long chat outputs.

## Remote Admin team target
Start with the minimum useful team:
- REMOTE-ADMIN-01
- REMOTE-EXECUTOR-01
- REMOTE-EXECUTOR-02
- REMOTE-QA-01
- REMOTE-REVIEWER-01

Maximum active roles for this pilot: 6 including admin unless GLOBAL CONTROL explicitly changes the limit.

## Mandatory bootstrap order
1. Admin reads canonical CLAB control/state.
2. Admin creates/enables its own recurring hourly wakeup and proves first successful CLAB read-back.
3. Only then Admin creates the minimum worker automations/tasks required by the mission.
4. Every worker receives an exact Issue assignment and recurring wakeup before ONLINE.
5. Executors work independently where safe; QA waits for a complete candidate; Reviewer waits for QA-backed candidate.
6. GLOBAL CONTROL reconciles final accepted public-safe state/artifacts.

## Work to divide
Create a public-safe `Multi-Account Project Bootstrap Pack` that another new project can reuse. The team must produce, through independent ownership:
1. canonical project onboarding template;
2. canonical agent registration/identity template;
3. mission/assignment template with scope, pinned inputs, evidence, stop conditions and escalation;
4. recovery/checkpoint template for context exhaustion/new chat continuation;
5. public-safe Human Gate template;
6. training/qualification template for missing capabilities;
7. QA evidence that the pack is internally consistent and public-safe;
8. independent Reviewer PASS or REJECT with exact defects.

This work is deliberately adjacent to the private Control Plane mission but does not modify or depend on private WP implementation. Do not copy private implementation/evidence into CLAB.

## GitHub write mode
External roles may operate in either mode defined by `control/EXTERNAL-WRITE-MODE.md`:
- ISSUE_WRITE — external roles publish exact candidates/evidence in Issues when Contents writes are unavailable;
- SCOPED_CONTENT_WRITE — only when actual file-write permission exists.

Issue-backed evidence is valid for execution/review. If final Definition of Done requires canonical repository files, GLOBAL CONTROL must reconcile accepted Issue evidence into canonical files before final PASS.

## Required Remote Admin behavior
REMOTE-ADMIN-01 must:
- follow `control/REMOTE-ADMIN-BOOTSTRAP-STANDARD.md` and Issue #8;
- maintain its own persistent wakeup;
- detect new GLOBAL CONTROL tasks from CLAB without owner forwarding;
- create workers only for real independent work;
- assign non-overlapping ownership;
- target bounded meaningful work rather than micro-tasks;
- preserve AUTHOR != FINAL JUDGE;
- ensure QA does not repair executor work and Reviewer does not author the pack it judges;
- publish factual status/evidence through the available GitHub write mode;
- stop only at a genuine Human Gate proven by actual tool/permission limits.

## Definition of Done
PASS requires all:
- actual REMOTE-ADMIN-01 bootstrap evidence;
- enabled recurring admin wakeup plus successful CLAB read-back evidence;
- factual worker roster/assignments/wakeup evidence;
- all 6 bootstrap-pack deliverables accepted and canonically reconciled into files;
- QA report bound to the exact candidate identity (file SHA where available, otherwise exact Issue/comment references before reconciliation);
- independent Reviewer PASS on the exact QA-backed candidate;
- no unresolved P0 defect;
- no private/confidential material in CLAB;
- recovery/read-back test showing a fresh chat can identify role, mission, current state and next step from GitHub alone;
- GLOBAL CONTROL final read-back.

Executor/Admin self-report alone cannot satisfy PASS.

## Forbidden
- production deploy;
- private/confidential payloads in CLAB;
- copying private repository contents into CLAB;
- claiming agents/automations exist without factual evidence;
- self-review/self-PASS;
- expanding into unrelated product development.