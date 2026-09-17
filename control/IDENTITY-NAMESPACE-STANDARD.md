# CLAB IDENTITY & NAMESPACE STANDARD

STATUS: ACTIVE
SCOPE: all CLAB-connected accounts, teams, agents and missions

## Purpose
Prevent role collisions when multiple ChatGPT accounts and teams work through the same CLAB repository.

## Mandatory identity tuple
Every active participant and assignment must be addressable by:
- NODE_ID — account/runtime node, e.g. `NODE-HQ-01`, `NODE-REMOTE-01`;
- TEAM_ID — team under that node, e.g. `TEAM-HQ-001`, `TEAM-REMOTE-001`;
- AGENT_ID — unique functional role within that team, e.g. `HQ-REGISTRAR-01`, `REMOTE-QA-01`;
- PROJECT_ID — target project;
- MISSION_ID — exact mission/work package.

No bare role names such as `Reviewer`, `Developer 01` or `Agent 02` are canonical identities.

## Namespace rules
1. HQ/local primary team uses prefix `HQ-`.
2. External account teams use prefix `REMOTE-` plus unique team number.
3. Agent IDs are unique inside CLAB, not only inside a chat/project.
4. Every GitHub assignment must name NODE_ID, TEAM_ID, AGENT_ID, PROJECT_ID and MISSION_ID.
5. Every wakeup prompt must include the same identity tuple and exact GitHub assignment issue.
6. Evidence without an attributable identity tuple is non-authoritative until reconciled.
7. Legacy chats keep historical names but receive no new assignments after migration unless explicitly reactivated.

## Team boundaries
A Remote Admin / HQ Registrar manages only its own TEAM_ID unless GLOBAL CONTROL explicitly grants cross-team authority.
Workers do not silently move between teams or accounts.
QA and Reviewer for an exact candidate must remain independently identifiable from its author.

## Scaling model
`GLOBAL CONTROL -> NODE_ID -> TEAM_ID -> AGENT_ID -> PROJECT_ID / MISSION_ID`

Example:
`GLOBAL CONTROL -> NODE-HQ-01 -> TEAM-HQ-001 -> HQ-REGISTRAR-01 -> PROJECT-CLAB-001 / HQ-BOOTSTRAP-001`

External example:
`GLOBAL CONTROL -> NODE-REMOTE-01 -> TEAM-REMOTE-001 -> REMOTE-ADMIN-01 -> PROJECT-CLAB-001 / REMOTE-PILOT-001`

## Online rule
An identity being registered does not mean it is ONLINE. ONLINE still requires factual task/automation existence, enabled state where applicable, exact assignment binding and successful read-back/evidence.