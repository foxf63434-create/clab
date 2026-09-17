# REMOTE ADMIN BOOTSTRAP STANDARD

STATUS: ACTIVE
SCOPE: all current and future CLAB remote administrator accounts

## Core invariant
A new REMOTE-ADMIN is not considered operational until its own recurring wakeup is created, enabled, and factually evidenced.

The administrator's FIRST operational action after reading CLAB is to establish its own recurring wakeup. Worker creation comes second.

## Mandatory bootstrap order
1. Read CLAB control contract and exact bootstrap issue.
2. Inspect actual available automation/scheduled-task tools.
3. Create and enable the REMOTE-ADMIN recurring wakeup immediately if the product supports it.
4. Record factual evidence in GitHub: admin role, automation/task ID if available, enabled state, cadence, first successful wake/read-back, and current mission state.
5. Only after the admin wakeup exists, create the minimum required worker agents/automations for the assigned mission.
6. Every worker gets its own recurring wakeup and exact GitHub assignment issue before being marked ONLINE.
7. On every admin wake, reread CLAB, determine the single real bottleneck, verify worker states/evidence, create/retire/reassign workers as needed, and continue dependency-safe work.
8. No manual forwarding of long task text between owner and workers; GitHub is the task bus.

## Wakeup prompt requirements
Every REMOTE-ADMIN wakeup must instruct itself to:
- open `foxf63434-create/clab`;
- read the current project/mission state and exact control issue(s);
- inspect new assignments, worker evidence, QA/Reviewer results, blockers and Human Gates;
- continue the highest-priority dependency-safe task;
- create additional workers only when real independent work exists;
- disable/retire workers with no executable assignment when possible;
- write GitHub state only when something materially changes;
- never invent agent status, evidence, PASS, tool access or completion;
- never write secrets/private data to CLAB.

## Human Gate rule
Do NOT open a Human Gate merely because no one manually created workers yet.
First attempt to create the admin wakeup and worker automations using actual available tools.
A Human Gate is allowed only after factual evidence proves the account cannot create/enable the required automation or requires owner-only permission/action.

## Persistence rule
The admin wakeup is persistent infrastructure for that account. Future GLOBAL CONTROL tasks are delivered through CLAB; the admin discovers them on its next wake and executes/routs them without the owner copying task text into chat.

## Evidence before ONLINE
INTENDED != CREATED.
CREATED != ENABLED.
ENABLED != SUCCESSFUL WAKE.
ONLINE requires factual evidence of enabled recurring automation plus at least one successful GitHub read-back/wake cycle.
