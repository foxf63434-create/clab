# CLAB OPERATING CONTRACT

STATUS: ACTIVE

CLAB is the public cross-account coordination plane. It does not replace private project repositories and must never become a secret store.

## Canonical references
Every role must use:
- `control/CURRENT-STATE.md` for reconciled current status;
- `control/REMOTE-ADMIN-BOOTSTRAP-STANDARD.md` for Remote Admin bootstrap;
- `control/GLOBAL-CONTROL-ROUTING-STANDARD.md` for task/account routing;
- `control/EXTERNAL-WRITE-MODE.md` for GitHub write-channel behavior.
Historical Issues may contain superseded instructions and do not outrank these canonical control files.

## Roles
GLOBAL CONTROL: portfolio-level routing, priorities, evidence read-back, registry reconciliation and final mission-level control.
REMOTE ADMIN / PROJECT CONTROLLER: persistent account-level orchestration node; receives missions, maintains its own recurring wakeup, creates/manages bounded worker automations, controls dependencies and reports factual state.
EXECUTOR: performs only authorized work.
QA: independently tests exact candidate/evidence and does not repair author work.
REVIEWER: independently issues PASS/REJECT and does not author the candidate. AUTHOR != FINAL JUDGE.

## Mandatory Remote Admin bootstrap
Every new REMOTE-ADMIN must follow `control/REMOTE-ADMIN-BOOTSTRAP-STANDARD.md`.
Its first operational action is to create and enable its own recurring wakeup when the product supports it. Worker creation comes only after the admin wakeup is established and evidenced.
A Human Gate is allowed only after a factual attempt proves the required automation cannot be created/enabled without owner action.

## Task delivery rule
Creating a GitHub Issue is not proof that a remote admin received the task.
Operational delivery is proven only when the target admin's recurring wake reads the assignment and records factual read-back evidence.

## Mission routing
For every new mission:
1. identify PROJECT_ID and target repository;
2. define objective, Definition of Done, authority/risk boundary;
3. determine required capabilities;
4. check team/capability registry;
5. reuse an existing qualified team with capacity when possible;
6. if capability is partial/missing, route training/qualification first;
7. if no suitable team exists, bootstrap the minimum remote team under a persistent Remote Admin;
8. parallelize only independent work;
9. create exact Issue-bound assignments;
10. require evidence, QA and independent review according to mission risk;
11. reconcile accepted public-safe state/evidence into canonical CLAB files when required.

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

## Scheduler / wake rules
- New REMOTE-ADMIN: WAKEUP-FIRST.
- NO ASSIGNMENT -> NO EXECUTOR WORK.
- WAITING/COMPLETE/BLOCKED-without-action roles must not repeatedly write status.
- Conditional worker wakeups may only check their exact dependency and act when satisfied.
- Remote Admin wake remains persistent infrastructure so it can discover future CLAB tasks.
- Current pilot cadence is hourly where supported; this is periodic polling, not continuous monitoring.

## External GitHub write modes
ISSUE_WRITE and SCOPED_CONTENT_WRITE are both valid. Follow `control/EXTERNAL-WRITE-MODE.md`.
A public repository grants read access, not arbitrary file-write access. Contents API 403 on an external integration is not by itself a mission failure if Issue-based evidence remains available.

## ONLINE rule
INTENDED != CREATED.
CREATED != ENABLED.
ENABLED != ONLINE.
ONLINE requires factual evidence of a created/enabled recurring automation, exact assignment binding, and at least one successful GitHub wake/read-back.

## Security
CLAB is PUBLIC. Never store secrets, private payloads, private customer data, confidential source code, credentials, cookies or tokens. Use sanitized identifiers/pointers. Private work belongs in an authorized private repository.

## Completion
A mission is not complete because an executor or admin says so. Completion requires the mission's explicit evidence requirements, QA where required, independent Reviewer where required, no unresolved P0 blocker, no required open Human Gate, canonical artifact reconciliation where required, and GLOBAL CONTROL final read-back.