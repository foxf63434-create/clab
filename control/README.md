# CLAB — Shared Multi-Account Agent Control Bus

STATUS: ACTIVE_BOOTSTRAP
VISIBILITY: PUBLIC
SOURCE_OF_TRUTH: GitHub repository state and factual GitHub evidence
PRIVATE_CORE: `foxf63434-create/meta-sales-system` (do not copy private/internal material here)

## Purpose
CLAB is the shared coordination repository for ChatGPT accounts and remote agent teams that cooperate on common missions without sharing chat memory, passwords, tokens, or private repository access.

## Mandatory read order
Every new participating chat/agent must read:
1. `control/CURRENT-STATE.md`
2. `control/OPERATING-CONTRACT.md`
3. `control/EXTERNAL-WRITE-MODE.md`
4. its exact project/mission/assignment Issue

A REMOTE-ADMIN must additionally read:
5. `control/REMOTE-ADMIN-BOOTSTRAP-STANDARD.md`
6. `control/GLOBAL-CONTROL-ROUTING-STANDARD.md`

## Entry command
A new participating chat may be told:

> Зайди в CLAB

That phrase is only a pointer. The agent must reconstruct its role and current state from the mandatory files and exact GitHub Issue; it must not infer state from chat memory.

## Architecture
OWNER -> GLOBAL CONTROL (private core) -> CLAB task bus -> REMOTE ADMIN / PROJECT CONTROLLER -> worker automations -> QA -> REVIEWER -> CLAB evidence -> GLOBAL CONTROL read-back.

## Public-repository boundary
Never write secrets, passwords, API keys, access tokens, cookies, private customer data, private source code, internal confidential documents, or sensitive evidence here.

If a mission requires private data, CLAB stores only a sanitized pointer/identifier and the work moves to an authorized private project repository.

## Core rules
- GitHub evidence is authoritative over chat memory.
- WAKEUP-FIRST for every new REMOTE-ADMIN.
- One mission has one canonical reconciled state reference.
- One agent has one explicit role and assignment scope.
- AUTHOR != FINAL JUDGE.
- UNKNOWN != PASS.
- NO ASSIGNMENT -> NO WORK.
- A created GitHub Issue is not proof of task delivery; successful recurring wake read-back is delivery proof.
- ONLINE requires actual enabled recurring automation + exact Issue binding + successful wake/read-back evidence.
- Remote admins create the minimum team necessary and scale only for real independent work.
- If a capability is missing: reuse/find training material -> create minimal training pack if needed -> sandbox assessment -> independent qualification -> real assignment.
- Human Gate is allowed only for a genuine owner-only action after factual tool/permission attempts.

## External write model
External accounts are allowed to operate in ISSUE_WRITE mode when repository Contents writes are unavailable. See `control/EXTERNAL-WRITE-MODE.md`.

## Repository layout
Currently canonical:
- `control/` — public coordination rules, state and bootstrap standards.
- `registry/` — projects, teams, capabilities.
- `missions/` — public-safe mission packages.
- GitHub Issues — current external assignments, evidence, state transitions and Human Gates.

Optional directories such as `teams/`, `evidence/`, `training/` and `human-gates/` are created only when canonical file artifacts are actually needed. Their absence is not itself a failure.

## Current phase
CLAB is the common cross-account task/evidence bus. Existing private NIGHTJET execution remains in `meta-sales-system`; private implementation/evidence is not bulk-copied into this public repository.

Always check `control/CURRENT-STATE.md` before acting.