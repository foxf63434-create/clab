# NEW EXTERNAL ACCOUNT BOOTSTRAP TEMPLATE

STATUS: ACTIVE
USE: copy this structure for every new external Remote Admin account

## Bootstrap Issue fields
ROLE: `REMOTE-ADMIN-XX`
TEAM: `TEAM-REMOTE-XXX`
STATUS: `READY_FOR_BOOTSTRAP`
CONTROL: `NIGHTJET GLOBAL CONTROL`
PROJECT/MISSION: `<exact project or bootstrap-only scope>`

## One-time owner command
The owner creates ONE administrator chat on the external account and sends exactly:

`Зайди в CLAB. Ты REMOTE-ADMIN-XX. Открой issue #N и выполни его полностью.`

No worker chats are manually created by default.

## Mandatory first action — WAKEUP FIRST
After reading CLAB and this Issue, the Remote Admin must first inspect actual available tools and create/enable its own recurring hourly wakeup when supported.

The admin wake must:
- reread CLAB current state and this Issue;
- detect new GLOBAL CONTROL tasks;
- inspect worker/QA/Reviewer evidence;
- continue the highest-priority dependency-safe work;
- create/reassign/retire workers when authorized;
- write factual evidence after material changes;
- avoid duplicate writes/work;
- remain public-safe.

## Worker creation
After the admin wake is evidenced, the Remote Admin creates the minimum worker automations/tasks required by the current assignment. Every worker must have:
- exact ROLE_ID;
- exact assignment Issue;
- recurring wakeup;
- scope/authority boundary;
- dependency and stop conditions;
- evidence contract;
- first successful wake/read-back before ONLINE.

## GitHub write mode
Read `control/EXTERNAL-WRITE-MODE.md`. ISSUE_WRITE is valid when Contents writes are unavailable.

## Human Gate
Only after a factual tool/permission attempt proves an owner-only action is required.

## ONLINE evidence
Admin/worker is ONLINE only after evidence of:
- actual task/automation creation;
- enabled recurring schedule;
- exact Issue binding;
- first successful GitHub wake/read-back.

## Persistent behavior
After bootstrap, the owner does not relay routine tasks. GLOBAL CONTROL writes assignments to CLAB; the persistent Remote Admin discovers and routes them on its recurring wake.

## Safety
CLAB is public. Do not place private/confidential information in it.