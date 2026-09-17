# CLAB CONTROL PREFLIGHT CHECKLIST

STATUS: ACTIVE
USE: GLOBAL CONTROL must run this checklist before bootstrapping a new external account, routing a new mission, or declaring a team/mission operational.

## A. Repository/state integrity
- [ ] `README.md` points to current canonical control files.
- [ ] `control/CURRENT-STATE.md` reflects factual GitHub evidence, not chat claims.
- [ ] no active instruction contradicts `control/OPERATING-CONTRACT.md`.
- [ ] superseded Issues are closed or clearly marked superseded.
- [ ] public/private boundary is explicit.

## B. New Remote Admin bootstrap
- [ ] bootstrap Issue exists before owner starts the chat.
- [ ] exact REMOTE-ADMIN ID is assigned.
- [ ] one-line owner command is included.
- [ ] WAKEUP-FIRST is the first operational action.
- [ ] actual tool capability must be checked; no assumed automation support.
- [ ] admin recurring wake behavior is fully specified.
- [ ] external ISSUE_WRITE fallback is specified.
- [ ] Human Gate requires factual proof of owner-only necessity.
- [ ] recovery/read-back path is specified.

## C. Worker creation
- [ ] workers are created only for real independent work.
- [ ] each worker has exact ROLE_ID and Issue assignment.
- [ ] each worker has recurring wakeup when supported.
- [ ] each worker has scope, authority, stop/dependency rules.
- [ ] QA does not repair author work.
- [ ] Reviewer does not author candidate work.
- [ ] no worker is marked ONLINE before first successful wake/read-back evidence.

## D. Task delivery
- [ ] GitHub Issue created.
- [ ] target persistent admin is already ONLINE, or this is the bootstrap Issue itself.
- [ ] successful recurring wake read-back proves operational delivery.
- [ ] no owner message relay is required after bootstrap.

## E. Registry/capability consistency
- [ ] `registry/TEAMS.md` matches actual evidence/status.
- [ ] `registry/PROJECTS.md` points to current mission/controller.
- [ ] `registry/CAPABILITIES.md` does not label unproven capability QUALIFIED.
- [ ] missing capability routes to training/assessment before real work.

## F. Completion/read-back
- [ ] exact candidate/evidence identity exists.
- [ ] required QA evidence exists.
- [ ] required independent Reviewer verdict exists.
- [ ] no unresolved P0 blocker.
- [ ] no required Human Gate remains open.
- [ ] canonical files are reconciled if Definition of Done requires them.
- [ ] GLOBAL CONTROL rereads GitHub after final transition.

## Fail rule
Any unchecked mandatory item blocks the corresponding bootstrap/routing/PASS transition. Fix the state first; do not rely on owner/chat memory to compensate.