# Meta-evolution — training the improver

**Meta-evolution** is a self-improvement design in which the outcomes of an evolutionary search are fed
back not only into the *search state* (which candidates survive, which parent is expanded next) but into
the **parameters of the model that proposes the variations**. The variation operator stops being a frozen
capability the harness merely orchestrates and becomes a **learned** one, trained on the very execution
evidence the harness generates.

The term and the ladder below come from [Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md)
(arXiv:2607.28568, Figure 2 right, p.4), which names its model for it — **M**eta-evolution **A**gent — and
credits the framing to Jiang et al. 2026's self-to-meta-evolution survey.

## The four-rung ladder

| Rung | What happens | Where the improvement is stored |
|---|---|---|
| **1. Evolution** | variation + selection over candidates | the population |
| **2. Self-evolution** | execution experience flows back and changes what the search explores next | the search state (archive, memory, tree) |
| **3. Meta-evolution** | that experience is reused to **train** the model that proposes future variations | the model weights |
| **4. Recursive self-improvement (RSI)** | each upgraded system further improves the process that produces its successors | everything, recursively |

Rungs 1–2 are where every other system in this wiki sits. Rung 3 is what Frontis-MA1 adds. Rung 4 is
explicitly *not* claimed — the paper calls OpenMLE "a concrete testbed for studying progress toward RSI …
rather than a claim that OpenMLE realizes general, autonomous recursive self-improvement" (§7, p.30). For
the theoretical ceiling rung 4 gestures toward — a formal proof of the recursive-self-improvement property
itself, at the cost of a fully axiomatized world — see [`../sources/goedel-machines.md`](../sources/goedel-machines.md).

## The load-bearing requirement: a shared operator interface

Meta-evolution is only tractable if training targets and inference actions are the *same* objects. Training
whole search trajectories gives sparse, controller-specific supervision that a different harness can't
reuse. OpenMLE's answer (§4.1) is a compact vocabulary of atomic program transformations —
**Draft / Improve / Debug / Crossover** — that serve simultaneously as SFT/RL targets and as the moves the
inference-time search composes. See [`program-evolution-operators`](program-evolution-operators.md).

The consequence is a clean split: **local skill lives in the weights, global composition lives in the
harness.** Verified evolutionary transitions supervise exactly the transformations search later invokes,
"making the trained model the variation engine of the evolutionary harness" (p.5).

## Why it is a different axis from the wiki's other self-improvement concepts

This wiki already tracks three targets of self-modification. All three modify **text**, proposed by a
**frozen** model. Meta-evolution modifies the model.

| Concept | What gets modified | Who proposes the change | Model weights |
|---|---|---|---|
| task-artifact ratchet ([`autoresearch`](../code/autoresearch/overview.md)) | a training config / `train.py` | frozen LLM | untouched |
| [`mechanism-level-self-improvement`](mechanism-level-self-improvement.md) (Bilevel Autoresearch) | the search-mechanism code | frozen LLM | untouched |
| [`self-referential-code-rewriting`](self-referential-code-rewriting.md) (DGM) | the agent's own tools/prompts/orchestration | the agent itself, frozen backbone | untouched |
| [`evolutionary-algorithm-discovery`](evolutionary-algorithm-discovery.md) (AlphaEvolve / openevolve) | a user-supplied target program | frozen LLM ensemble | untouched |
| **meta-evolution** (Frontis-MA1) | **the proposal policy itself** | SFT + RL on execution outcomes | **updated** |

> [!inferred] **DGM and Frontis-MA1 are orthogonal halves of the same ambition, and neither wiki page said
> so before this paper.** DGM rewrites the scaffold around a frozen model; Frontis-MA1 trains the model
> inside a fixed, human-authored scaffold. DGM's own limitation is that its archive/parent-selection loop
> stays human-owned; Frontis-MA1's limitation #4 is that "evolution operates primarily over candidate
> solutions, while the evolutionary system itself remains largely fixed." Each system's stated future work
> is roughly the other system's present. A rung-4 system would have to close both loops at once — train the
> proposer *and* let the trained proposer rewrite the harness that trains it — and no paper in this wiki
> does that yet.

## Evidence that the rung is real

The claim "training the improver helps, on top of a better harness" needs the two gains separated, and
Frontis-MA1's controlled comparisons do that (§6.2, Table 1):

- **Fix the harness, swap the model.** Under identical OpenMLE-Evo: Qwen3.6-35B-A3B 39.39% → Frontis-MA1-35B
  **60.61%** Medal Average on MLE-Bench Lite (**+21.22 pp**), reproduced on a second backbone and scale
  (Qwen3-30B-A3B-Thinking 34.85% → Frontis-MA1-30B 53.03%, **+18.18 pp**).
- **Fix the model, swap the harness.** Frontis-MA1-35B under original AIRA-Evo 53.03% → under OpenMLE-Evo
  **60.61%** (**+7.58 pp**).
- **They compose**, reaching 71.21% with OpenMLE-Evo-Max — a 35B open model above GPT-5.5 + Codex (68.18%).
- **It transfers off-benchmark.** On the held-out 10-task NatureBench Lite, Match-SOTA rises 5/10 → 7/10
  when only the model is swapped and 2/10 → 5/10 when only the harness is swapped.

> [!inferred] The two-way ablation is what makes this more than a leaderboard entry: it is the only
> evidence in this wiki that *weight-level* and *harness-level* improvement are separable and additive
> rather than substitutes for one another. It also inverts the usual conclusion of the frozen-model
> systems: AlphaEvolve's thesis is that a good outer loop extracts more from a fixed model; Frontis-MA1's
> is that the same outer loop extracts *substantially* more from a model trained for that loop's specific
> moves. The margins are noisy (±7.73 pp over three epochs), so treat the ordering of the controlled
> comparisons as the finding, not the exact point values.

## What training on execution outcomes forces you to change

Meta-evolution's practical difficulty is that MLE execution feedback is nothing like short-horizon RLVR on
math or code: most programs never produce a usable reward, successes carry continuous scores on
incomparable metric scales, feedback arrives minutes-to-hours later, and every non-`Draft` action depends
on which parent was selected. OpenMLE-ERL's three answers (§4.3) are the concrete cost of climbing this
rung:

- **Adaptive reward bounds** derived from each task's on-policy score frontier rather than leaderboard
  extrema — otherwise meaningfully different programs collapse to near-identical rewards.
- **Entropic advantage** (an exponential tilt replacing GRPO's group normalization) so the *best* candidate
  in a rollout group dominates the update — because the objective is best-of-budget, not mean quality.
  Measured: best-candidate advantage 1.58 → 6.39.
- **Asynchronous rollouts**, because the dominant latency is sandbox execution, not token generation, and a
  synchronous batch idles on its slowest job.

Plus a fourth, easy to overlook: **which parent state to train each operator on.** Uniform sampling wastes
updates on exhausted regions, greedy sampling trains forever on the incumbent — so parents are drawn
proportional to reward + **child-reward variance** + a **visit-cooling** term (Eq. 3).

## See also
- [`program-evolution-operators`](program-evolution-operators.md) — the shared interface that makes rung 3 possible
- [`self-referential-code-rewriting`](self-referential-code-rewriting.md) — the orthogonal half (scaffold, not weights)
- [`mechanism-level-self-improvement`](mechanism-level-self-improvement.md) — the rung below, in text rather than weights
- [`evolutionary-self-improvement`](evolutionary-self-improvement.md) — the population shapes rung 1–2 systems use
- [`../sources/frontis-ma1.md`](../sources/frontis-ma1.md)
- [`../topics/mle-agents-and-benchmarks.md`](../topics/mle-agents-and-benchmarks.md)
