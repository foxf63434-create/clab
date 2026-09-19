# CLAB CURRENT STATE

STATUS: HQ_WP04_R05_QA_RESUMING_WITH_DSA_RUNTIME_BLOCKED
LAST_CONTROL_AUDIT: 2026-09-19
SOURCE_OF_TRUTH: GitHub state + actual scheduler observations + exact execution evidence
CURRENT_AUTHORITIES: `HQ-CONTROL-DELIVERY-RESUMPTION-20260919-01`; `HQ-CONTROL-PARALLEL-LANES-20260919-01`; `HQ-CONTROL-PREFLIGHT-PREVENTION-20260919-01`; scoped `HQ-CONTROL-ROUTING-CORRECTION-20260919-01`; `HQ-CONTROL-LONG-PACKETS-20260919-01`; historical R04 recovery authority remains history only.
PUBLIC_WORK_ISSUES: #18 / `BUILD-WP04`; #24 / `WP09-01 DSA qualification`.

## Global control
CONTROL: NIGHTJET GLOBAL CONTROL
PRIVATE_CORE: `foxf63434-create/meta-sales-system`
PUBLIC_BUS: `foxf63434-create/clab`
CONTROL_AGENT: `NODE-HQ-01 / TEAM-HQ-001 / HQ-CONTROL-01`
ADMIN_AGENT_ID: `HQ-REGISTRAR-01`

## Preserved accepted history
WP01: Reviewer PASS on `14872635c8c857ed33384975cd20f18cf7a8f5d9`.
WP02: Reviewer PASS on `b2f18f96a91fb44a60f303303bbd0139e3b6d425`.
WP03: frozen `CONTROL_ACCEPTED / WP03_R02_BOUNDED_PASS` on `b7445b57ae6db866cf4d75dc88e0626d4ff6c3e9`, tree `c033cb98b07afd0691a1e9984f2b2ddcc1876bf1`.
Product network-backed `GitHubApiSource` remains `NOT_TESTED`; connector reads are not product integration proof.

## BUILD-WP04
R01-R04 remain immutable independent QA REJECT history. Delivery authority permits only R05-R07, total maximum candidate rounds 7, with no R08/reset/renamed retry. Rejected-round accounting remains `4` until another actual independent REJECT.

CURRENT_PHASE: `QA`.
CURRENT_ROUND: `R05`.
TASK_ID: `HQ-QA-WP04-API-R05`.
ACTIVE_OWNER: `HQ-QA-01`.
RUN_STATUS: `QA_ROUTING_PENDING_ENABLE_AFTER_EXACT_BYTE_MATERIALIZATION_REMEDY`.
BUILD_BRANCH: `build/wp04-status-evidence-api-001`.
R04_INPUT: `5d92dd1455a1090546a6295adf394f96b0fb2881` / tree `397b6b920e915c7d1cff82d73996a3de51f359d4`.
PINNED_R05_CANDIDATE: `2a1b39fef0778e786bac79b1cd51c54118269783` / tree `a73d7cecc935f1f49af145aa1f8ba5f22832c880`.
PINNED_BLOBS: `status_api.py=d0d122e9eb4502f92439ff7dc973465d3328f13b`; `tests/test_status_api.py=49cd93c82fc6e7eff541dc29709a615993351335`.
DEVELOPER_RESULT: `READY_FOR_QA`; reported `102/102` author/regression tests plus compile. This remains author evidence only and the author stays frozen.
PRIOR_QA_RESULT: `BLOCKED / REQUIRED_EXACT_BYTE_EXECUTION_ENVIRONMENT_UNAVAILABLE`, independent product tests executed = `0`; prior evidence blob `838d1648ac909d9f06d3636de1c5dc2e4ec7b913` remains immutable history.
MATERIALIZATION_REMEDY: Control proved an already-available authenticated connector -> isolated runtime exact-byte bridge with local per-file Git-blob verification. Private evidence `meta-orchestrator/missions/digital-organization-infrastructure-v1/BUILD-ITERATION-1/EVIDENCE/CONTROL-WP04-R05-EXACT-BYTE-MATERIALIZATION-DIAGNOSIS-20260919-01.md` @ `c759e29ae5c55926104de729e463721ce9438b4c`, blob `348e1fb2ef29755fa442f4cbc84cd451967861fd`; public #18 comment `5740705583`.
QA_SCHEDULER: existing QA worker is being rebound to the SAME R05 task; `ROUTING_PENDING_ENABLE`. This is not execution or PASS.
REVIEWER: `DEPENDENCY_GATED / NOT_ROUTED`.
CONTROL_ACCEPTANCE: `NOT_REACHED`.

Before any import/test, QA must materialize every required candidate/module/dependency/test file from authenticated GitHub at exact immutable refs into an isolated runtime and verify each complete file against its expected Git blob. Any mismatch, incomplete response or unverified required file is a hard BLOCKED stop. After successful materialization, the full mandatory C01-C12+canonical identity/association coverage, unchanged R01-R04 suites, candidate tests, affected accepted upstream regressions, positive controls and full imported local pipeline remain required. Control's materialization pilot is not product QA.

NEXT_WP04_TRANSITION: Registrar completes prompt read-back and enables existing HQ-QA-01 on the same immutable R05 task. Same-candidate `READY_FOR_REVIEW` routes existing Reviewer; an actual REJECT follows finite delivery stop/repair rules; truthful BLOCKED preserves R05. No R06, author restart, Reviewer routing or candidate mutation from the prior blocked artifact alone.

## Separate WP09-01 DSA lane
PUBLIC_LANE_ISSUE: #24.
TASK_ID: `HQ-DEV-WP09-01-QUAL-Q01`.
PHASE: `BLOCKED_RUNTIME`.
ACTIVE_OWNER: `NONE`.
CAPABILITY: `UNVERIFIED`.
BRANCH: `build/wp09-01-dsa-foundation-001`.
SAVED_PROBE: `aad029d0f4c2e3c0bc1e73f8b8bccbc79a0a63e3` / tree `8611573a1059a2b20cd5bb3f5e600fbbbc0eb25b`.
BLOCKER: `POSTGRESQL_ISOLATED_RUNTIME_UNAVAILABLE_IN_CURRENT_EXECUTION_ENVIRONMENT`.
Q1 remains partial/blocked; Q2-Q6 not executed; Q7 partial probe only. A later Control-owned isolated remedy attempt failed before PostgreSQL test steps. No runtime recovery or qualification is proven. This blocker is not a V0 dependency.
NEXT_DSA_TRANSITION: Control identifies a safe already-authorized isolated PostgreSQL runtime plus client/driver and independent verifier path, then Registrar performs an explicit Q01 recheck. Independent QUALIFIED is required before DSA implementation.

## Problem cycle
Private native `[NIGHTJET-PROBLEM]` Issues in `foxf63434-create/meta-sales-system` are the sole problem register and are not task authority. Current canonical cards: #44 PostgreSQL runtime / WAITING; #45 existing WP04 identity defect / VERIFYING_PENDING_RESUMED_QA; #46 reporting rollout / IN_PROGRESS; #47 WP04 QA exact-byte execution runtime / VERIFYING_MATERIALIZATION_REMEDY. QA reaches a legitimate safe boundary on this same-task recovery, so its current prompt must receive the reporting addendum before activation. Other stopped/blocked workers are not awakened solely for policy distribution.

## Downstream gates
Post-WP04 #21/#22/#23 and later V0 work remain gated behind exact WP04 independent QA + Reviewer PASS + final Control acceptance. Freeze state remains owned only by canonical Freeze Control. WP09-02 waits accepted WP09-01; later DSA DAG dependencies remain unchanged.

No production/deploy, product-main merge, force-push, live DSA/scheduler cutover, secrets/permissions/workflows, paid infrastructure, consequential customer action, false PASS or self-acceptance is authorized.

PUBLISHED != ACKNOWLEDGED. ENABLED != EXECUTED. EXECUTED != QUALIFIED. QUALIFIED != ACCEPTED.