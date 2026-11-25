# mini-harness S3 roadmap receipt
## Identity and pins
- Receipt contract: proposal-gate
- Original repository: dmoka/mini-harness
- Original HEAD: 4563935c87c4e22514a6ee3842fc51cf34ebe2fb
- Observed at: 2026-11-25
- Accepted Index assessment: https://github.com/opensiro/vsm-harness-index/blob/7abafd36dd9216d94e795dac9e6030bc0e8e56a6/assessments/dm/dmoka-mini-harness.md
- Accepted assessment blob SHA: 3513c706a289b150a9b0567b39771b8e4104ddb1
- Accepted review ref: 4563935c87c4e22514a6ee3842fc51cf34ebe2fb
- Accepted reviewed at: 2026-11-24
- Index corpus pin: 7abafd36dd9216d94e795dac9e6030bc0e8e56a6
- Profile version: 0.2.4
- Assessment procedure version: 0.3.8
- System in focus: local coding runtime and direct worktree children.
- Repository-wide source map: [Runtime](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51cf34ebe2fb/agent.py), [README](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51cf34ebe2fb/README.md), both backends, tests, requirements, license and full tracked tree inspected. No CI/contributor/Issue templates. Local parent Session and direct worktree children in act/chat; plan/consolidation reviewed. External model internals and maintainer governance excluded.
- Accepted VSM vector: S1=A · S2=A · S3=— · S3*=— · S4=— · S5=—
- S1 disposition: Model loop selects actions and completion; ALREADY_A.
- S2 disposition: Worktree isolation and join; ALREADY_A.
- S3 disposition: Fork/join starts eligible calls and joins reports; P0: allocate shared starts and slots.
- S3* disposition: Fresh context and generic Stop hooks; DEFER: independent audit/control path missing.
- S4 disposition: Local memory and compaction; NO_TARGET: local scope, intent unknown.
- S5 disposition: Task approval/configuration; NO_TARGET: no justified authority transfer.
- Priority rationale: S3 reuses actual isolated child units and narrow dispatch/result seam. S3* needs distinct audit/control recipient; S4/S5 widen the local teaching scope. A is not mandatory C work. Minimal teaching purpose documented, specific function intent and demand NOT_STATED.
- Target transition: S3=— -> S3=C
- P1 dependencies: Truthful exit/commit status, stable call IDs, session-wide ledger and gate for single/mixed calls, trusted opt-in, nested direct worktree launch denial in controlled mode.
- P2 optional: NONE
- Proposed C construction: Opt-in Session-level autonomous allocator of direct worktree commitments within operator-set slot and total-start limits, enforcing grants and reallocating after actual outcomes.
- C sufficiency falsifier: Equivalent first-party closure, actor-independent allocation, no outcome-sensitive effect or a direct worktree launch bypass.
- Scenario basis: HYPOTHETICAL
- Proposal-stage decision: GO
- Research disposition: NEEDS_EVIDENCE
- Proposed validation: Native fake model/temp Git, different legal choices, bounded actual starts, truthful results, negative grants and opt-out.
- Validation state: NOT_RUN
- Proposal falsifier: Equivalent first-party closure, actor-independent allocation, no outcome-sensitive effect or a direct worktree launch bypass.
## Rights and authority
MIT; no tracked CLA/DCO/AI policy found, not legal certification. Live original Issues/pulls state=all empty. Matching fork verified exact parent and main HEAD, push rights; Issues disabled. Bootstrap DORMANT/PAUSE outside #58 activation; no ongoing RESUME or public consent. Operator retains immutable caps and scope, no merge right.
## Existing work / overlap
SHIPPED: [dispatch](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51cf34ebe2fb/agent.py#L112-L122), [worktree](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51cf34ebe2fb/agent.py#L532-L545), isolation and report text. No competing issue/PR returned. Manual waves or fixed cap are alternatives, not adaptive allocation.
## Function ownership
HYPOTHETICAL: two pending direct children compete for one slot and two starts; A fails, actor chooses B or retry A. Operator fixes limits; actor decides; runtime enforces and returns actual outcome. Children retain task discretion.
## Capability priority
- P0: Opt-in Session-level autonomous allocator of direct worktree commitments within operator-set slot and total-start limits, enforcing grants and reallocating after actual outcomes.
- P1: Truthful exit/commit status, stable call IDs, session-wide ledger and gate for single/mixed calls, trusted opt-in, nested direct worktree launch denial in controlled mode.
- P2: NONE
- Proposed C-sufficiency verdict: PROPOSED_C_SUFFICIENT conditional on validation.
## Parallel contribution-on-top review
- Evaluation object: Current allocation of direct worktree commitments within one Session.
- Existing-work overlap: SHIPPED worktree isolation/fork-join; no dedicated allocator or structured outcome.
- Our on-top contribution: Optional actor, gated ledger and outcome feedback.
- Incremental benefit: HYPOTHETICAL delegation instead of manual prompt splitting.
- Decision scope: proposal only, not adoption or grade.
## Implementation options
Trusted Session factory; serialize grant decisions, gate all direct starts, return outcomes before reallocation. No shell containment, global token cap or preemption.
## Specification and domain alternatives
Optional original integration, MIT domain experiment, independent Profile/Skills feedback if actual ambiguity.
## Cost experiment
- Cost status: NOT_MEASURED
Matched manual waves vs actor, same tasks/limits; compare completion, intervention, engineering/review/test/maintenance.
## Delivery and publication
- Result: PLAN_ONLY
- External issue: DRAFT — NOT PUBLISHED
- Fork issue: NOT PUBLISHED, disabled.
- Case: .opensiro/issues/worktree-commitment-control-s3-20261125/; no product changes or contribution record; further effects require RESUME and exact consent.
