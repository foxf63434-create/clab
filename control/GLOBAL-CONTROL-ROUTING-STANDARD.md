# GLOBAL CONTROL ROUTING STANDARD

STATUS: ACTIVE
SCOPE: all CLAB tasks, teams and future external accounts

## Goal
Prevent repeat bootstrap/routing mistakes and keep owner involvement to the minimum one-time action required to attach a new account.

## New external account rule
For every new external account, GLOBAL CONTROL must create exactly one canonical REMOTE-ADMIN bootstrap Issue before the owner starts the chat.

That bootstrap Issue MUST include, in this order:
1. exact REMOTE-ADMIN ID;
2. exact one-line owner bootstrap command;
3. WAKEUP-FIRST requirement: admin creates/enables its own recurring wakeup before worker creation;
4. exact recurring wake behavior: reread CLAB, detect new GLOBAL CONTROL tasks, continue dependency-safe work, write evidence after material changes;
5. permission/tool capability check using actual tools, not assumptions;
6. worker creation authority and maximum team size/bounds;
7. requirement that every worker gets an exact role, assignment Issue and recurring wakeup before ONLINE;
8. issue-write fallback when Contents write is unavailable;
9. evidence requirements for admin and worker ONLINE status;
10. Human Gate only after a factual failed attempt proves owner-only action is necessary;
11. public-safety/no-secrets rules;
12. recovery/read-back path.

## Task routing rule
When GLOBAL CONTROL receives a new task:
1. identify project and objective;
2. define Definition of Done and risk/authority boundary;
3. determine required capabilities;
4. inspect `registry/TEAMS.md` and `registry/CAPABILITIES.md`;
5. route to an existing qualified team with available capacity when possible;
6. if capability is missing, route training/qualification before production work;
7. if no team is suitable, bootstrap a new REMOTE-ADMIN using this standard;
8. create one canonical control/assignment Issue per independent workstream;
9. do not wake roles without executable work;
10. require QA/Reviewer independence where the mission requires it.

## Team sizing
REMOTE-ADMIN creates the minimum team needed for actual independent work. If a task says “create N agents”, it may create up to that authorized number, but must still give each role a real non-overlapping assignment and wakeup. No idle decorative agents.

## Wake semantics
Recurring wakeup means periodic polling, not continuous monitoring. Default cadence for this CLAB pilot is hourly because that is the maximum supported automation frequency in the current product context.

## Delivery proof
A GitHub Issue being created does NOT prove the remote account has seen it.
A task is considered operationally delivered only when the target admin's recurring wake has read the Issue and produced factual read-back evidence.

## ONLINE proof
ONLINE requires:
- actual automation/task created;
- enabled recurring schedule;
- exact role and Issue binding;
- successful GitHub read-back on at least one wake.

INTENDED != CREATED.
CREATED != ENABLED.
ENABLED != ONLINE.

## No owner relay
After one-time admin bootstrap and persistent wake proof, the owner must not be used as a routine message relay. GLOBAL CONTROL writes tasks to CLAB; Remote Admin discovers them on wake and routes them itself.

## Audit rule
Before creating a new bootstrap Issue, GLOBAL CONTROL must compare it against this standard. If any mandatory item is missing, the Issue is incomplete and must not be used to start the external account.