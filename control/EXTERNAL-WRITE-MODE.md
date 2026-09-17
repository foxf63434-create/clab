# CLAB EXTERNAL WRITE MODE

STATUS: ACTIVE
SCOPE: all external ChatGPT/GitHub accounts using CLAB

## Purpose
Public visibility guarantees read access, not repository file-write access. External ChatGPT GitHub integrations may be able to create Issues while repository Contents writes return 403.

This is a supported operating mode and must not block coordination.

## Mode A — ISSUE_WRITE
Use when the external account can read CLAB and create/comment on GitHub Issues but cannot write repository files.

The external role must:
- read canonical files from CLAB;
- receive its exact assignment from an Issue;
- publish factual status, candidate content, test output, blockers, task IDs and wake evidence in that Issue or a dedicated evidence Issue;
- never claim that a repository file exists when it only posted candidate text in an Issue.

GLOBAL CONTROL / an authorized canonical writer may later reconcile accepted public-safe evidence into repository files.

## Mode B — SCOPED_CONTENT_WRITE
Use only when the external account actually has repository Contents write permission.

The role may write only its explicitly assigned paths. It must not edit control policy, registries, other teams' state, QA/Reviewer evidence, or unrelated missions unless explicitly authorized.

## Canonical ownership
- `control/**`: GLOBAL CONTROL only unless explicitly delegated.
- `registry/**`: GLOBAL CONTROL reconciled registry; external teams propose changes via Issues unless explicitly delegated.
- mission deliverables: assigned executor or GLOBAL CONTROL reconciler according to the mission write mode.
- QA evidence: QA role only.
- Reviewer verdict: Reviewer role only.

## Evidence identity
Every material result must name:
- ROLE_ID
- MISSION_ID / PROJECT_ID
- assignment Issue
- candidate identity (file paths + commit/blob SHA when files exist; otherwise exact Issue/comment reference)
- status
- blocker/dependency
- next allowed transition

## Security
Never use a public Issue or file for secrets, credentials, cookies, tokens, private source code, customer data or confidential payloads.

## Completion rule
ISSUE_WRITE evidence can prove work and review decisions, but if a mission Definition of Done explicitly requires canonical repository files, GLOBAL CONTROL must reconcile the accepted evidence into those files before final completion.