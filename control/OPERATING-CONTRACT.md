# CLAB OPERATING CONTRACT

STATUS: ACTIVE

CLAB is the public cross-account coordination plane. It does not replace private project repositories and must never become a secret store.

## Roles
GLOBAL CONTROL: portfolio-level routing, priorities, evidence read-back, final mission-level control.
REMOTE ADMIN / PROJECT CONTROLLER: receives a bounded mission, decides minimal team composition, creates assignments, controls dependencies and scheduler state.
EXECUTOR: performs only authorized work.
QA: independently tests exact candidate/evidence.
REVIEWER: independently issues PASS/REJECT. AUTHOR != FINAL JUDGE.

## Mission routing
For every new mission:
1. Identify PROJECT_ID and target repository.
2. Define objective and Definition of Done.
3. Determine required capabilities.
4. Check team/capability registry.
5. Reuse an existing qualified team when possible.
6. If capability is partial, create an upskilling package and qualification gate.
7. If no suitable team exists, instantiate the minimum remote team under a Remote Admin.
8. Parallelize only independent work.
9. Require evidence, QA and independent review according to risk.
10. Return sanitized state/evidence to CLAB.

## Task sizing
Prefer bounded 20–45 minute executor packages rather than micro-tasks. A package may contain 2–4 tightly related subtasks inside one ownership/work-package boundary. Do not cross QA, Reviewer, architecture, Human Gate, production/external-side-effect, or shared-writer boundaries without new authority.

## Blocker routing
Two materially different reasonable attempts without progress -> stop spinning and route:
- runtime/build/environment -> INCIDENT/DEBUG;
- implementation defect -> responsible developer;
- architecture conflict -> ARCHITECT;
- acceptance/evidence gap -> QA/REVIEWER;
- missing capability -> TRAINING/QUALIFICATION;
- owner-only access/decision -> HUMAN GATE.

## Scheduler
NO ASSIGNMENT -> NO WAKE.
WAITING/COMPLETE/BLOCKED-without-action/HUMAN_GATE roles must not consume recurring wakes. Conditional roles may wake only to check their exact deterministic dependency and must make no write if it is absent.

## Security
CLAB is public. Never store secrets or private payloads. Use sanitized identifiers/pointers. Private work belongs in an authorized private repository.

## Completion
A mission is not complete because an executor says so. Completion requires the mission's evidence requirements, QA where required, independent Reviewer where required, no unresolved P0 blockers, no required open Human Gate, and GLOBAL CONTROL read-back.
