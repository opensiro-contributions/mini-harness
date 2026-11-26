# mini-harness — source-native S3 technical contract
Human [issue.md](issue.md); canonical [roadmap.md](roadmap.md). PLAN_ONLY. **DRAFT — NOT PUBLISHED**.

## 1. Function-specific construction boundary and methodology checks
**Source and mode boundary:** [Runtime](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py), [README](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/README.md), both backends, tests, requirements, license and full tracked tree inspected. No CI/contributor/Issue templates. Local parent Session and direct worktree children in act/chat; plan/consolidation reviewed. External model internals and maintainer governance excluded.

**Target transition:** S3=— -> S3=C

**Six-function dependencies (S1/S2/S3/S3*/S4/S5):** See roadmap.md; preserve S1 child discretion and S2 isolation; no S3*/S4/S5 grant.

**Function witness:** HYPOTHETICAL: two pending direct children compete for one slot and two starts; A fails, actor chooses B or retry A. Operator fixes limits; actor decides; runtime enforces and returns actual outcome.

**Counterfactual owner test:** Without actor, static order or no admission lacks adaptive allocation. Two valid actors can make different lawful choices.

**Possible methodological negative control:** Fixed executor cap alone is not discretionary current resource control.

**Contributor / maintainer priorities:** NOT_STATED; minimal teaching scope explicit.


## 2. Source-pinned baseline and parallel native Track A / on-top Track B
**Original native workflow:** [run_tool_calls](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L112-L122) uses ThreadPoolExecutor.map; [run_in_worktree](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L532-L545) runs child, attempts commit, returns branch/report. Single/mixed calls use call_tool.

**Closest existing solution:** Manual waves or static pool, no dedicated allocation feedback.

**Relevant original Issues/PRs:** Live state=all lists empty; no competing head or maintainer demand.



| Link | A | B | Falsifier |
| --- | --- | --- | --- |
| State | Calls/join | Session ledger | Equivalent path |
| Owner | Parent delegates | Autonomous scoped allocator | Hardcoded grants |
| Effect | Worktree process | Gate and feedback | Bypass/no return |

**On-top distinctness:** Finite starts and adaptive retry/defer distinguish S3 from fixed parallelism.

**Source ambiguity / rights blockers:** Demand and utility unknown; direct worktree scope only; fork Issues disabled; explicit owner RESUME recorded, ACTIVE/ALLOW.


## 3. Minimal complete S3 first-party C construction
**Required property:** Developer composes rightful autonomous resource/commitment owner with first-party effect and feedback.



| Port | Source | Edit | Owner and effect |
| --- | --- | --- | --- |
| Session | [Session](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L71-L83) | Optional trusted actor, immutable limits, ledger | Operator defines scope; actor sees snapshot |
| Dispatch | [call_tool](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L112-L148) | Gate all direct starts; as-completed callback | Actor chooses grant; runtime enforces |
| Outcome | [run_in_worktree](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/agent.py#L532-L545) | Actual exit/commit status, branch and original ID | Outcome returned before next choice |

**Architectural C-sufficiency argument:** Trusted Session factory composes autonomous actor (e.g. model-backed); actor reads pending/running/outcomes and remaining slots/credits, chooses start/defer/close or retry with new credit. Runtime serializes grants, rejects invalid/stale IDs, reserves slot and counts start at launch, releases slot on actual outcome and invokes actor again. No valid grant means defer with explicit original tool IDs. Gate single/mixed calls too; block nested worktree starts even after load_tools in controlled children. Arbitrary shell processes outside scope. Preserve plan/permissions and disabled baseline. No right to raise cap, change goal, merge or preempt. Static pool or generic hook lacks this complete loop.

**Explicit non-goals:** No global token cap, sandbox, arbitrary shell containment, daemon, merge, preemption or S4/S5.

**Implementation dependency graph:** Truthful outcomes/IDs → ledger and nested gate → actor and iterative dispatch → tests.


## 4. Priorities, optional alternative and stopping rules
**P0 and P1:** Canonical in roadmap.md; only scoped loop and dependencies.

**P2:** NONE.

**Alternative path:** Manual waves or fixed pool if fixed concurrency suffices.

**Stop:** Equivalent first-party closure, actor-independent allocation, no outcome-sensitive effect or a direct worktree launch bypass.


## 5. Future source-native acceptance — derive tests, do not copy a matrix
**Native test commands and entry points:** README pytest -q; [tests/test_agent.py](https://github.com/dmoka/mini-harness/blob/4563935c87c4e22514a6ee3842fc51fc34ebe2fb/tests/test_agent.py#L167-L205) covers subagents and worktrees. Extend fake model/temp Git. NOT_RUN.

**Positive functional closure:** A fails then B starts under one slot/two credits; actual launch and result IDs.

**Independent alternative (where applicable):** Retry A instead, B deferred, same inputs and caps.

**Negative authority and compatibility (where applicable):** Invalid/stale/missing grant, exhausted credits and nested launch denied; single/mixed path and opt-out baseline.

**Matched native alternative:** Manual waves with same task/caps; compare completion/interventions.


| Case | Setup | Expected | Falsifier |
| --- | --- | --- | --- |
| Feedback | Fake model/temp Git | A fails then B starts | Hidden failure |
| Alternative | Same input/retry actor | A retry, B deferred | Fixed order |
| Invalid | Mixed/single/nested | No ungranted starts | Bypass |
| Off | pytest -q | Baseline preserved | Regression |
## 6. Proposal verdict, falsification, evidence ownership and handoff
**Proposal-stage decision:** GO

**Research disposition:** NEEDS_EVIDENCE

**Primary falsifier:** Equivalent first-party closure, actor-independent allocation, no outcome-sensitive effect or a direct worktree launch bypass.

**Validation state:** NOT_RUN.

**Ownership of truth:** Profile semantics, Skills method, Index grades, original maintainers adoption, roadmap.md decision.

**Cost status:** NOT_MEASURED.

**Next permitted action:** Independent review; separate exact authorization for external effects.

**Human backlink:** [issue.md](issue.md).

**case receipt:** [roadmap.md](roadmap.md).

**AI disclosure:** AI-assisted; no implementation, test or independent review claimed.

