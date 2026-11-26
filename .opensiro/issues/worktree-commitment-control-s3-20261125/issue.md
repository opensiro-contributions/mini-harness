# mini-harness — S3 worktree commitment control (Opensiro roadmap)

**PLAN_ONLY · GO · NEEDS_EVIDENCE · DRAFT — NOT PUBLISHED**

**One-sentence proposal:** Opt-in Session-level autonomous allocator of direct worktree commitments within operator-set slot and total-start limits, enforcing grants and reallocating after actual outcomes.

**Canonical decision receipt:** [roadmap.md](roadmap.md).

**Technical companion:** [constructor-sufficiency.md](constructor-sufficiency.md).

**Working fork:** opensiro-contributions/mini-harness.

**Case:** .opensiro/issues/worktree-commitment-control-s3-20261125/ on opensiro/meta.


## 1. Why Opensiro and central accepted VSM assessment

Research reusable VSM constructs, not proven cost reduction or mandatory architecture.

> ACCEPTED HISTORICAL INDEX — not current-HEAD grades
> S1=A · S2=A · S3=— · S3*=— · S4=— · S5=—
> [Accepted assessment](https://github.com/opensiro/vsm-harness-index/blob/7abafd36dd9216d94e795dac9e6030bc0e8e56a6/assessments/dm/dmoka-mini-harness.md); 2026-11-24; review_ref 4563935c87c4e22514a6ee3842fc51fc34ebe2fb; blob 3513c706a289b150a9b0567b39771b8e4104ddb1; Profile 0.2.4 / Methodology 0.3.8.

**Repository-wide audit:** [Runtime](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py), [README](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/README.md), both backends, tests, requirements, license and full tracked tree inspected. No CI/contributor/Issue templates. Local parent Session and direct worktree children in act/chat; plan/consolidation reviewed. External model internals and maintainer governance excluded.


| Function | Historical | Current owner/closure | Priority |
| --- | --- | --- | --- |
| **S1 · Operations** | A | Model loop selects actions and completion | ALREADY_A |
| **S2 · Coordination** | A | Worktree isolation and join | ALREADY_A |
| **S3 · Current management** | — | Fork/join starts eligible calls and joins reports | P0: allocate shared starts and slots |
| **S3* · Complementary audit** | — | Fresh context and generic Stop hooks | DEFER: independent audit/control path missing |
| **S4 · Future adaptation** | — | Local memory and compaction | NO_TARGET: local scope, intent unknown |
| **S5 · Ultimate policy** | — | Task approval/configuration | NO_TARGET: no justified authority transfer |

A autonomous; C first-party developer-composable autonomous owner; P parent-governed S3/S4/S5; A(P)/C(P) separately evidenced parent mode; — bounded absence; ? unresolved. Ownership categories, not quality ranks.

**Priority rationale:** S3 reuses actual isolated child units and narrow dispatch/result seam. S3* needs distinct audit/control recipient; S4/S5 widen the local teaching scope. A is not mandatory C work. Minimal teaching purpose documented, specific function intent and demand NOT_STATED.

**Deliberate exclusions / methodology challenge:** Minimal teaching purpose explicit; specific omission unknown. Larger deployment could challenge boundary.

**Contributor / maintainer interests (OPTIONAL):** NOT_STATED.


## 2. Selected construction hypothesis and operator outcome
**Target transition:** S3=— -> S3=C

**Function-specific disturbance:** HYPOTHETICAL: two pending direct children compete for one slot and two starts; A fails, actor chooses B or retry A. Operator fixes limits; actor decides; runtime enforces and returns actual outcome.

**Proposed C capability (P0):** Opt-in Session-level autonomous allocator of direct worktree commitments within operator-set slot and total-start limits, enforcing grants and reallocating after actual outcomes.

**Best native operator alternative:** Manual waves or prompt splitting; [dispatch](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L112-L122).

**Expected user benefit:** HYPOTHETICAL: delegate allocation without editing dispatch or manual prompt splitting.

**Architectural sufficiency argument:** Actor sees current commitments and actual results, chooses scoped grants; runtime enforces and returns results before next allocation.


## 3. Existing native work versus missing construction
**Track A — native coverage:** SHIPPED isolation/fork-join, report text, permissions; no original issue/PR returned.

**Track B — independent on-top C construction:** Session controller, validated ledger and structured results.


| Link | Existing | Missing |
| --- | --- | --- |
| State | Calls/join | Pending/running/outcomes and grants |
| Owner | Parent proposes tasks | Composed allocator |
| Effect | [Worktree](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L532-L545) | Gate and actual outcome return |
**Distinctness and falsifier:** Equivalent first-party closure, actor-independent allocation, no outcome-sensitive effect or a direct worktree launch bypass.


## 4. Priorities and minimum sufficient result
- **P0:** Opt-in Session-level autonomous allocator of direct worktree commitments within operator-set slot and total-start limits, enforcing grants and reallocating after actual outcomes.
- **P1:** Truthful exit/commit status, stable call IDs, session-wide ledger and gate for single/mixed calls, trusted opt-in, nested direct worktree launch denial in controlled mode.
- **P2:** NONE.

**Proposed C-sufficiency verdict:** PROPOSED_C_SUFFICIENT conditional; not shipped C.


## 5. Proposed acceptance and stop gates
**Future positive test:** One slot, two credits: A fails; actor chooses B; alternative actor retries A. Actual launches and IDs reflect decision.

**Future negative test:** Invalid/exhausted grant and nested controlled launch denied; baseline unchanged.

**Proposed falsifier:** Equivalent first-party closure, actor-independent allocation, no outcome-sensitive effect or a direct worktree launch bypass.

**Validation state:** NOT_RUN.


## 6. Independent paths
**Original-native contribution:** Optional narrow constructor; maintainers decide.

**Profile / Skills:** Separate feedback only if independent review finds fixed-limit versus S3 ambiguity.

**Domain fork:** MIT permits bounded parallel coding experiment.


## 7. Cost hypothesis
Matched manual waves vs actor, same caps/tasks; completion, interventions, engineering and maintenance. NOT_MEASURED.
## 8. Decision / handoff
**Proposal-stage decision:** GO

**Research disposition:** NEEDS_EVIDENCE

**Decision reason / next permitted step:** Complete proposed loop; demand and tests unverified. Independent review and separate implementation authorization.

**Agent/developer handoff:** [constructor-sufficiency.md](constructor-sufficiency.md) and [roadmap.md](roadmap.md).

**Rights and publication:** MIT; no tracked CLA/DCO/AI policy found, not legal certification. Live original Issues/pulls state=all empty. Matching fork verified exact parent and main HEAD, push rights; Issues disabled. Initially DORMANT/PAUSE; explicit owner RESUME 2026-11-26, ACTIVE/ALLOW. Separate exact publication consent remains.

**AI disclosure:** AI-assisted; no native tests or independent human review presumed.

