# REMOTE-PILOT-001 — MULTI-ACCOUNT TEAM BOOTSTRAP TEST

STATUS: READY_FOR_REMOTE_ADMIN
PROJECT_ID: PROJECT-CLAB-001
CONTROL: NIGHTJET GLOBAL CONTROL
PRODUCTION: FORBIDDEN
PUBLIC_REPO: YES

## Goal
Prove that a ChatGPT account other than the current Global Control account can enter CLAB, assume REMOTE-ADMIN-01, create and coordinate a minimal local agent team, divide a bounded mission, collect evidence, use independent QA/Reviewer roles, and return a trustworthy result through GitHub without manual forwarding of long chat outputs.

## Remote Admin team target
Start with the minimum useful team:
- REMOTE-ADMIN-01
- REMOTE-EXECUTOR-01
- REMOTE-EXECUTOR-02
- REMOTE-QA-01
- REMOTE-REVIEWER-01

Maximum agents for this pilot: 6 including admin, unless GLOBAL CONTROL explicitly changes the limit.

## Work to divide
Create a public-safe `Multi-Account Project Bootstrap Pack` that another new project can reuse. The team must produce, through independent ownership:
1. a canonical project onboarding template;
2. a canonical agent registration/identity template;
3. a mission/assignment template with scope, pinned inputs, evidence, stop conditions and escalation;
4. a recovery/checkpoint template for context exhaustion/new chat continuation;
5. a public-safe Human Gate template;
6. a training/qualification template for missing capabilities;
7. QA evidence that the pack is internally consistent and contains no secret-request/storage instructions;
8. independent Reviewer PASS or REJECT with exact defects.

This work is deliberately adjacent to the private Control Plane mission but does not modify or depend on private WP01/WP02 implementation. Do not copy private code/evidence into CLAB.

## Required Remote Admin behavior
REMOTE-ADMIN-01 must:
- read `control/README.md` and `control/OPERATING-CONTRACT.md`;
- create `teams/TEAM-REMOTE-001/TEAM-STATE.md` and an agent roster only after the agents are actually instantiated/assigned;
- assign non-overlapping ownership;
- use the smallest useful team;
- target bounded meaningful work rather than micro-tasks;
- preserve AUTHOR != FINAL JUDGE;
- ensure QA does not repair executor work and Reviewer does not author the pack it judges;
- write public-safe evidence under `evidence/REMOTE-PILOT-001/`;
- update mission `STATE.md` after material transitions;
- stop at a genuine Human Gate rather than inventing access or evidence.

## Definition of Done
PASS requires all:
- actual remote admin bootstrap evidence;
- actual agent roster and assignments;
- all 6 bootstrap-pack deliverables present;
- QA report bound to exact paths/commits;
- independent Reviewer PASS on the exact QA-backed candidate;
- no unresolved P0 defect;
- no secret/private data in CLAB;
- recovery/read-back test showing a fresh chat can identify role, mission, current state and next step from repository files alone;
- GLOBAL CONTROL final read-back.

Executor self-report cannot satisfy PASS.

## Forbidden
- production deploy;
- credentials/secrets/tokens/cookies;
- private customer data;
- copying private repository contents into CLAB;
- claiming agents exist without factual creation/assignment evidence;
- self-review/self-PASS;
- expanding into unrelated product development.
