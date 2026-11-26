# Proposal: outcome-aware worktree resource allocation for mini-harness — Opensiro VSM architecture review

## Proposal in the project's own terms

We propose an optional allocation policy for direct worktree subagents, keeping the existing fork-join behavior as the default.

**What exists today:** [Parallel dispatch](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L112-L148) and [worktree execution](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L532-L545) support isolated coding children and branch reports.

**What may be missing:** A developer-composable allocator that chooses which pending child to start, defer or retry under operator-set concurrent-slot and total-start limits, then reallocates based on actual subprocess and Git commit outcomes.

**Closest existing project-native solution:** Manual task batching or prompt splitting; fixed concurrency limits are another simpler design alternative.

**Existing discussion:** No original Issues or PRs returned by the bounded original-repository search and publication-history review on 2026-11-26. This is not a global novelty claim.

## How we reached this proposal — Opensiro VSM assessment

We use the Viable System Model (VSM) to examine organizational functions and decision ownership, not product quality, safety or maturity.

**Historical assessment:** [Accepted Index assessment](https://github.com/opensiro/vsm-harness-index/blob/7abafd36dd9216d94e795dac9e6030bc0e8e56a6/assessments/dm/dmoka-mini-harness.md); Index commit 7abafd36dd9216d94e795dac9e6030bc0e8e56a6; assessment blob 3513c706a289b150a9b0567b39771b8e4104ddb1; reviewed 2026-11-24; review_ref 4563935c87c4e22514a6ee3842fc51fc34ebe2fb; Profile 0.2.4; Skills Methodology 0.3.8.

**Boundary:** Local Python coding-agent runtime, SDK and Claude CLI backends, act/chat/plan modes and direct operational children; external model internals and maintainer governance excluded.

**Current original HEAD:** [4563935c87c4e22514a6ee3842fc51fc34ebe2fb](https://github.com/dmoka/mini-harness/commit/4563935c87c4e22514a6ee3842fc51fc34ebe2fb), observed 2026-11-26.

| Key | Organizational function | Historical state | Evidence or limitation |
| --- | --- | --- | --- |
| **S1 · Operations** | Doing the actual work | A | [Model loop](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L85-L148) selects actions and completion. |
| **S2 · Coordination** | Reducing interference between operations | A | [Child execution](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L510-L545) enables model-selected isolated worktrees. |
| **S3 · Current management** | Allocating current resources and commitments | — | Parallel dispatch and join do not evidence a dedicated autonomous allocation loop. |
| **S3* · Independent audit** | Independently checking operations and returning corrective feedback | — | [Hooks](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L566-L609) and fresh contexts do not establish an independent audit loop. |
| **S4 · Future adaptation** | Exploring future change and returning adaptation options | — | [Local memory](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L297-L429) is not evidence of strategic adaptation. |
| **S5 · Identity and policy** | Resolving ultimate policy and authority | — | [Plan approval](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L491-L503) is not evidence of autonomous system-level policy ownership. |

- `A`: autonomous decision and feedback closure in a supported first-party mode.
- `C`: first-party construction path requiring developer composition of the autonomous actor, authority or closure.
- `P`: supported parent-governed S3, S4 or S5 without established A/C autonomy.
- `A(P)` / `C(P)`: independently evidenced parent-governed mode alongside A or C for S3/S4/S5.
- `—`: no material first-party function path evidenced after bounded absence review.
- `?`: insufficient evidence for a positive path or bounded absence.

These are ownership and constructibility states, not quality ranks. Missing functions need not be defects.

## Why this particular construction?

**Whole-repository prioritization:** S1/S2 already have autonomous paths. S3 can reuse actual child units and the dispatch/result seam. S3* needs a distinct audit/control recipient; S4/S5 would widen the teaching scope. Specific maintainer intent and demand are not established.

**Construction hypothesis:** S3=— → S3=C. This is a proposed future construction, not a reassessment or shipped feature.

**Native building blocks:** Session, parallel dispatch, isolated child worktrees and branch reports.

**Minimal proposed addition:** A trusted opt-in Session-level allocator interface, shared ledger and structured outcome feedback, with enforced grants for all direct worktree launches.

**Scope exclusions:** Arbitrary shell containment, global token budgets, preemption, autonomous merge authority and the other VSM functions. The operator sets immutable limits; children retain task discretion.

## Proposed approach and validation

1. Track pending tasks, active worktrees, stable call IDs and remaining launch capacity.
2. Allow the allocator to choose start, defer, retry or close; enforce grants across single and mixed direct worktree calls and deny nested controlled worktree launches.
3. Return actual subprocess and Git commit outcomes before reallocation. Preserve existing behavior when disabled.
4. Test two pending tasks competing for one slot and two starts: after A fails, one allocator chooses B and another retries A. Check actual starts, truthful results, rejection of invalid/exhausted grants and compatibility.

**Hypothesized benefit:** Less manual intervention when allocating limited capacity across direct coding children. This scenario is hypothetical; demand and utility have not been demonstrated.

**How to falsify:** An equivalent first-party path already exists, allocation decisions do not affect actual starts, outcome feedback is insufficient, or controlled launches bypass grants.

**Cost status:** NOT_MEASURED. No implementation or tests have been performed for this proposal.

## Feedback requested

Would this optional mechanism fit mini-harness's educational and architectural goals? Would manual batching or fixed limits be preferable? Is our VSM interpretation inaccurate or intentionally outside scope? The maintainers alone decide whether to adopt, simplify or decline the proposal.

## Three independent ways to participate

- Improve mini-harness through a focused native implementation if the maintainers want it.
- Challenge or improve the open VSM assessment methodology.
- Explore the mechanism in a legally permitted independent experimental fork without changing mini-harness.

## Research attribution and AI disclosure

[OpenSiro Upstream](https://github.com/opensiro/upstream) · [VSM Profile](https://github.com/opensiro/vsm-harness-profile/blob/main/PROFILE.md) · [VSM Skills](https://github.com/opensiro/vsm-harness-skills/blob/main/skills/assess-vsm-harness/references/autonomy-states.md) · [VSM Index](https://github.com/opensiro/vsm-harness-index)

[Original architecture proposal and technical contract](https://github.com/opensiro-contributions/mini-harness/tree/0e90bb34f5c9adaff49ed5e5855ed69a9e1387d9/.opensiro/issues/worktree-commitment-control-s3-20261125)

**AI involvement:** Prepared with AI assistance. No independent human technical validation, maintainer endorsement, implemented constructor, new Index grade or measured savings is implied.
