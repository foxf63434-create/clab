# CLAB — Shared Multi-Account Agent Control Bus

STATUS: ACTIVE_BOOTSTRAP
VISIBILITY: PUBLIC
SOURCE_OF_TRUTH: this repository for cross-account coordination only
PRIVATE_CORE: foxf63434-create/meta-sales-system (do not copy private/internal material here)

## Purpose
CLAB is the shared coordination repository for ChatGPT accounts and remote agent teams that must cooperate on common missions without sharing chat memory, passwords, tokens, or private repository access.

## Entry command
A new participating chat may be told:

> Зайди в CLAB

It must open `foxf63434-create/clab`, read this file, then read `control/OPERATING-CONTRACT.md`, `registry/PROJECTS.md`, `registry/TEAMS.md`, and its exact assignment under `missions/` or `teams/` before acting.

## Architecture
OWNER -> GLOBAL CONTROL (private core) -> CLAB mission package -> REMOTE ADMIN / PROJECT CONTROLLER -> EXECUTORS -> QA -> REVIEWER -> CLAB evidence -> GLOBAL CONTROL read-back.

## Public-repository boundary
Never write secrets, passwords, API keys, access tokens, cookies, private customer data, private source code, internal confidential documents, or sensitive evidence here.

If a mission requires private data, CLAB stores only a sanitized pointer/identifier and the work moves to an authorized private project repository.

## Core rules
- GitHub evidence is authoritative over chat memory.
- One mission has one canonical state path.
- One agent has one explicit role and write scope.
- AUTHOR != FINAL JUDGE.
- UNKNOWN != PASS.
- NO ASSIGNMENT -> NO WAKE.
- No production/external irreversible action without explicit authority/Human Gate.
- Remote admins create the minimum team necessary and scale only for real independent parallel work.
- If a capability is missing: find/reuse training material -> create minimal training pack if needed -> sandbox assessment -> independent qualification -> real assignment.

## Repository layout
- `control/` — public coordination rules and bootstrap.
- `registry/` — projects, teams, capabilities.
- `missions/` — sanitized mission packages and states.
- `teams/` — remote-team state/assignments.
- `evidence/` — public-safe evidence only.
- `training/` — public-safe training packs and qualification evidence.
- `human-gates/` — sanitized owner-only requests; never secrets.

## Current phase
CLAB is being bootstrapped as the common cross-account bus. Existing private NIGHTJET execution remains in `meta-sales-system` until a migration is explicitly validated. We are not bulk-copying the private repository into this public repository.
