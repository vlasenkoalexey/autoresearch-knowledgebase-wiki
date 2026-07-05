# Bilevel Autoresearch: Meta-Autoresearching Itself

**Source:** Qu and Lu, "Bilevel Autoresearch: Meta-Autoresearching Itself," arXiv:2603.23420v2 (originally
posted 2026-03-24, revised 2026-06-02).
[arxiv.org/abs/2603.23420](https://arxiv.org/abs/2603.23420), PDF
[arxiv.org/pdf/2603.23420](https://arxiv.org/pdf/2603.23420). Code:
[github.com/EdwardOptimization/Bilevel-Autoresearch](https://github.com/EdwardOptimization/Bilevel-Autoresearch)
(not ingested into this wiki as a code silo). Raw source:
[`../../raw/papers/bilevel-autoresearch.pdf`](../../raw/papers/bilevel-autoresearch.pdf).

## What this paper is

Bilevel Autoresearch takes literally the idea that "if autoresearch is itself a form of research, then
autoresearch can be applied to research itself" (p. 1, Abstract). It wraps an **outer autoresearch loop**
around an **inner autoresearch loop that is exactly this wiki's `autoresearch` benchmark** — Karpathy's
edit–train–keep/discard cycle on GPT pretraining `val_bpb`, cited directly as `[Karpathy, 2026]` (p. 2, 5).
The outer loop does not touch the inner loop's training code or its trained artifact; it reads the inner
loop's **runner code and execution trace**, diagnoses *why the search is stuck*, and **writes and injects new
Python search mechanisms at runtime** — drawn from combinatorial optimization, multi-armed bandits, and
design of experiments — that change how the inner loop proposes and accepts its next candidates (p. 1–2).
Both the inner and outer loop use the *same* LLM (DeepSeek `deepseek-chat`, p. 5, §3.1) — the paper's
central claim is that the gain comes from the **bilevel architecture**, not from a stronger meta-level model.

## The three levels

The paper structures this as three nested levels (Figure 2, p. 6; Algorithm 1, p. 8):

- **Level 1 — inner autoresearch loop** (§3.2, p. 5): the unmodified propose→train→evaluate→keep/discard
  cycle. An LLM sees the current `train.py` frozen at the best-accepted config plus any editable/frozen
  parameter list, proposes a parameter change with a one-sentence hypothesis, trains for a fixed 300-second
  budget, and keeps the change only if `val_bpb` improves. Budget: 30 iterations per run.
- **Level 1.5 — outer *search-strategy* loop** (§3.3, p. 5, 7): runs every 5 inner iterations. It reads the
  full proposal/outcome trace and emits a `SearchConfig` update: **freeze** parameters proposed ≥3 times with
  zero net improvement, **unfreeze** parameters untouched since the search moved to a new region, and
  **inject a guidance string** telling the inner loop to prioritize under-explored parameters. Critically,
  the paper is explicit that "Level 1.5 can redirect search diversity but cannot change the proposal
  generation logic, the acceptance criterion, or the loop structure" (p. 7) — it only re-weights *within* the
  existing, fixed mechanism.
- **Level 2 — mechanism research and code injection** (§3.4, p. 7): runs every 2 outer cycles, via a
  **4-round structured LLM dialogue**, each round one call: **Explore** (read `runner.py` + trace, survey
  mechanisms from adjacent fields), **Critique** (pick the most promising one against the observed failure
  mode, e.g. repetitive proposals or parameter fixation), **Specify** (write a class-level interface spec),
  **Generate** (write complete, runnable Python implementing it, plus any `runner.py` call-site edits). The
  generated module is **validated by dynamically importing it (`importlib`) before activation**; if the
  import fails, the pre-patch backup is restored and the old mechanism keeps running (p. 7–8).

Formally the paper borrows bilevel-optimization vocabulary (Colson et al. 2007, Sinha et al. 2018,
§2.2, p. 3): the outer level optimizes a search mechanism φ (the runner code) and the inner level optimizes
task performance θ (the training config), but it flags the key departure from classical bilevel
optimization up front — φ here is a **discrete, LLM-generated program**, not a differentiable real-valued
parameter, so what's implemented is "a finite-budget, non-differentiable analogue" (p. 3), not a solved
nested optimization problem.

## What Level 2 actually discovered

Across three repeats of the full system (Group C, below), Level 2 produced code from three distinct,
*active* mechanism domains (Table 3, p. 9; excerpt of one in Figure 5, p. 10): a **Tabu Search Manager**
(blocks reproposing recently-visited parameter regions), a **Multi-Scale Bandit Proposer** (treats parameter
choice as a multi-armed-bandit exploration/exploitation problem across scales), and **Systematic Orthogonal
Exploration** (forces proposals along under-explored parameter dimensions). A fourth attempt, a **GP
Regressor** (Bayesian optimization), was valid code but reverted automatically because `sklearn` wasn't
installed — the validate-and-revert gate catching an external-dependency failure exactly as designed (p. 9,
13). All code was accepted on the *first* generation attempt across all six sessions, zero retries (p. 9).

## The headline result: ~5x, and why parameter tuning alone didn't get it

Four ablation groups (Table 1, p. 8; results Table 2, p. 9), 3 repeats each, metric Δ = best − baseline
`val_bpb` (more negative = better):

| Group | Levels | Mean Δ |
|---|---|---|
| A | Level 1 only | −0.009 ± 0.002 |
| B | Level 1 + 1.5 | −0.006 ± 0.006 |
| C | Level 1 + 1.5 + 2 (full bilevel) | **−0.045 ± 0.030** |
| D | Level 1 + 2 (no strategy adjustment) | −0.034 ± 0.031 |

Group C's mean is the paper's headline **~5x over Group A** (and 7.5x over Group B) (p. 9, 12). Group B —
parameter-level redirection *without* new mechanisms — is not reliably better than plain Group A (H1, "not
supported," p. 12): Level 1.5 gets the LLM to explore more parameters, but within the *same* fixed
propose/accept structure that exploration doesn't translate into bigger wins, and B's worst repeat found
essentially zero improvement. Level 2 is the load-bearing ingredient (H2, "supported," p. 12).

Trace analysis (§4.3–4.4, p. 11–12) explains the mechanism: on the paper's RTX 5090 setup (running SDPA,
not Flash Attention 3), the decisive win in every high-performing repeat was discovering that
**`TOTAL_BATCH_SIZE` should be *reduced*** (2¹⁹→2¹⁷/2¹⁸), not increased — smaller batches buy more gradient
steps inside the fixed 300-second budget on this hardware. DeepSeek's default proposal prior tries a batch
*increase* first everywhere; Group A just discards and repeats that failed increase up to 22 times in a row;
Group B's Level 1.5 actually makes this *worse* in one respect — it freezes `TOTAL_BATCH_SIZE` after the
failed increase, which blocks the decrease direction entirely (p. 12). Only Level 2's injected mechanisms
(Tabu Search blocking the repeated failed increase, Orthogonal Exploration forcing a different dimension)
broke the LLM's deterministic prior and let the search find the *decrease* direction. Group D (Level 2
without Level 1.5) is messier evidence for the same story: two of its three repeats also found the
batch-size direction and scored comparably to Group C, but one repeat's Level 2 sessions generated code that
*failed* import validation, so it silently ran as bare Level 1 — the paper is careful to flag Group D as
"suggestive but inconclusive" (H4, p. 12) rather than a clean Level-2-without-1.5 result.

> [!inferred] Read structurally, the paper's own ablation shows Level 1.5 is not just "weaker than Level 2" —
> in the one concrete case traced in detail (`TOTAL_BATCH_SIZE`), the *parameter-freezing* mechanism that
> Level 1.5 hard-codes actively worked against the eventual winning direction, while Level 2's freedom to
> introduce a *different kind* of mechanism (Tabu Search, which blocks repetition without permanently
> freezing a whole parameter) let the search escape. That's a fairly direct empirical illustration of why the
> paper insists Level 1.5 and Level 2 are targeting *categorically different* objects (below), not points on
> one continuum of "more outer-loop intervention is better."

## Level 1.5 vs. Level 2: parameters vs. structure (the paper's own distinction)

The paper is explicit that this is not a matter of degree (§2.6, p. 5): **"Level 1.5 is closest to existing
outer loops (curriculum schedulers, adaptive configuration) in that it adjusts parameters of the existing
mechanism. Level 2 is categorically different: it generates code that modifies or replaces structural
components of the search mechanism."** Only Level 2 rewrites *what kind of search procedure runs at all* —
freeze/unfreeze is a knob on a fixed acceptance rule, whereas Tabu Search / bandit / orthogonal-exploration
injection replaces the proposal-generation logic itself.

## Mechanism-level self-improvement: the paper's broader claim

The paper deliberately generalizes beyond "Python code is special" (§5.3, p. 13; §2.5, p. 4). Its claim is
that the object worth modifying is the **mechanism** — the logic that generates, evaluates, selects, and
revises *future* candidates — and that Python is merely a convenient carrier for it in this implementation
because it's "explicit, executable, and easy to validate before activation" (p. 2). Skills, prompts,
workflows, evaluators, domain principles, world-model assumptions, and memory schemas are named as
alternative carriers of the same kind of object (p. 2, 4, 13–14), untested here (flagged explicitly as a
limitation, p. 13). This is the paper's way of drawing a line between two kinds of self-improving systems it
surveys in §2.5 (p. 4): **artifact-level** systems that optimize *an* artifact used in the current episode
(e.g., ADOPT optimizing prompts inside a fixed pipeline, or PiEvo doing Bayesian optimization over a
scientific-principle space) versus **mechanism-level** systems, where what's being optimized is the
generate/evaluate/select/revise logic that produces *future* artifacts. Bilevel Autoresearch places itself
in the second category and states it is "not aware of earlier autoresearch systems in which an autonomous
outer loop writes and injects code that modifies the structural logic of the inner autoresearch loop at
runtime, using the same model that runs the inner loop" (p. 5).

## How this differs from this wiki's other self-improvement papers

- **vs. `autoresearch`'s own ratchet** ([overview](../code/autoresearch/overview.md)): Karpathy's harness is
  exactly this paper's **unmodified Level 1** — a single-branch, human-designed keep/discard loop over
  `train.py`. Bilevel Autoresearch doesn't change what that loop is allowed to *edit* (still `train.py`,
  still `val_bpb`); it adds an outer loop that treats **the loop's own proposal/acceptance mechanism**
  (`runner.py`, not `train.py`) as a second, higher-level object to optimize. So where `autoresearch`
  optimizes the *task* (θ, the training config) under a fixed search procedure, Bilevel Autoresearch adds a
  level that optimizes the *search procedure* (φ) that generates θ-candidates — a genuinely different target
  than "self-modifying the training code," even though Level 1 of this paper *is* that training-code loop.
- **vs. Darwin Gödel Machine** ([source](darwin-godel-machine.md), concepts
  [`self-referential-code-rewriting`](../concepts/self-referential-code-rewriting.md),
  [`evolutionary-self-improvement`](../concepts/evolutionary-self-improvement.md)): DGM's self-modification
  target is the coding agent's **own tools, prompts, and orchestration** — the full scaffold that both
  produces edits *and* is itself edited, searched via a growing **archive** of every variant produced, with
  every archive member (even underperformers) retaining non-zero resampling probability as a potential
  stepping stone. Bilevel Autoresearch's Level 2 target is narrower: only the **search mechanism component**
  (the runner's propose/accept/explore logic), not the whole agent scaffold, and there is **no archive** —
  at any time there is one active mechanism φ, which is generated, import-validated, and either activated or
  reverted (closer to a single-branch ratchet *at the mechanism level* than to DGM's open-ended population
  search). DGM is also genuinely **self-referential** in Schmidhuber's sense — the thing being edited (the
  agent) is the same thing doing the editing, recursively, from the first iteration. Bilevel Autoresearch is
  explicitly *not* that (yet): Level 2 modifies Level 1, but Level 2's own logic — the 4-round dialogue
  structure, the K=5/M=2 cycle periods, Level 1.5's freeze/unfreeze rule — is fixed and human-authored in
  this paper. The paper names the missing piece directly: "if a discovered mechanism reliably improves
  Level 1, the same mechanism-discovery principle can in principle be applied to Level 2 itself" — but
  "recursive bootstrapping" of the *meta*-level loop "remains a future evaluation target," not something
  demonstrated here (p. 13–14, §5.4 "Recursive limitation"). So the paper's outer loop currently only closes
  the loop **one level deep** (outer improves inner); it does not (yet) improve *itself*.

> [!inferred] Put together, this wiki now has three distinct points on a "what gets self-modified" axis:
> `autoresearch` modifies the task artifact under a fixed mechanism; Bilevel Autoresearch modifies the
> mechanism under a fixed meta-mechanism; DGM modifies the mechanism *and* is itself the thing modifying it,
> with no fixed level above. Bilevel Autoresearch is a real step up from `autoresearch` (a second level
> exists at all) but a real step short of DGM (the second level is not itself open to revision, and there is
> no archive of surviving alternatives at either level).

## Limitations the paper is explicit about (§5.4, p. 13–14)

Small sample (n=3 repeats/group — Group C's own ±0.030 std is 67% of its mean); baseline `val_bpb` varies
1.094–1.114 run-to-run from training randomness; single benchmark (GPT pretraining, 50M params, RTX 5090,
300s budget) with unproven generalization; only Python code was tested as a mechanism carrier; a **dynamic
load fragility bug** (`sys.modules` registration) silently made an early preliminary run's mechanism
injections all fall back to the unmodified runner without erroring — fixed before the reported repeats, but
flagged as evidence that silent-fallback failure modes are a real risk for this style of runtime
self-modification; Level 2 has no import allowlist (the reverted GP-Regressor/`sklearn` case is the concrete
instance); and the Level 2 prompt names candidate domains (combinatorial optimization, RL, evolutionary
algorithms, Bayesian optimization) up front, which the authors flag as a double-edged constraint on what
mechanisms Level 2 can discover at all.

## Related work the paper positions against (§2, p. 2–5)

Karpathy's `autoresearch` [2026], AutoResearchClaw (multi-batch parallel search) and EvoScientist
(persistent cross-run memory) are all named as prior autoresearch variants whose search *procedures* were
still human-designed. §2.5 (p. 4) situates the paper relative to ADOPT (prompt optimization inside a fixed
pipeline) and PiEvo (Bayesian optimization over a scientific-principle space) as artifact-level comparators,
and lists a wave of concurrent/subsequent 2026 work explored through the same "carrier" lens — Meta-Harness,
Continual Harness, GEAR (population-based autoresearch with an evolvable controller), Discovering
Cooperative Pipelines, SkillEvolver, SkillOpt, and AEvo (a meta-agent editing the procedure/context that
controls future evolution, flagged as "especially close in spirit," p. 4).
