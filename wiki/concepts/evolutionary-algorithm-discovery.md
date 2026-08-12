# Evolutionary algorithm discovery (LLM-guided)

**LLM-guided evolutionary algorithm discovery** is a search paradigm in which candidate solutions are
represented as *code* (or as code that *constructs* a solution), an **LLM acts as the mutation/crossover
operator** — proposing edits to existing programs — and an **automated evaluator scores each candidate**,
with a population database selecting which survivors seed the next generation. It sits between classical
evolutionary/genetic programming (which uses handwritten mutation operators) and single-shot LLM code
generation (one pass, no population, no execution-grounded selection). The defining property is that
**correctness and quality are enforced by executing a programmatic evaluator**, so many generations can
run without an LLM judge's errors compounding — at the cost of only applying to problems for which such an
evaluator can be written.

## Core mechanism

1. **Candidate = code.** A solution is a program (evolving the final artifact directly, evolving a
   constructor function, or evolving a bespoke search algorithm that finds the artifact within a compute
   budget — the last often works best for asymmetric problems).
2. **Mutation = LLM diff.** Rather than a fixed grammar of edits, a frontier LLM proposes changes
   (typically as SEARCH/REPLACE diff blocks), informed by prior high-scoring programs, their scores, and
   natural-language problem context. This lets the operator carry world knowledge into the search.
3. **Selection = programmatic evaluation + population database.** An `evaluate` function returns scalar
   metric(s); a database balancing exploration vs. exploitation (e.g. MAP-elites + island models) decides
   which programs are resurfaced as parents/inspirations. Multi-objective scoring is common and often
   improves even a single target metric by diversifying the population.

## Lineage

- **FunSearch** (Romera-Paredes et al., 2023) — the progenitor: LLM-guided evolution of a *single* short
  Python function against a *single* objective, using a small code-only model and millions of samples.
  Discovered new mathematical constructions and online-algorithm heuristics.
- **AlphaEvolve** (Novikov et al., 2025) — see [`../sources/alphaevolve.md`](../sources/alphaevolve.md).
  Scales the paradigm to whole codebases in any language, multi-objective scoring, frontier-LLM ensembles
  (Gemini Flash+Pro), rich NL context, and hours-long parallel accelerator evaluation. Reached a rank-48
  4×4 complex matrix-multiply (first improvement over recursive Strassen in 56 years), improved ~50 open
  math problems, and delivered production compute-stack optimizations (Borg scheduling, Gemini kernels,
  TPU circuits, XLA IR). This is the wiki's canonical exemplar of the concept.
- **openevolve** ([codelion/openevolve](https://github.com/codelion/openevolve)) — an independent
  open-source reimplementation of the AlphaEvolve recipe.
- **GEVO / GEVO-ML** (Liou, Forrest, Wu et al., 2019–2022) — the pre-LLM branch, cited by
  [KernelEvolve](../sources/kernelevolve.md) §7: evolutionary computation applied to GPU code at the
  LLVM/MLIR level with *handwritten* transformation operators. The same skeleton with the LLM swapped in for
  the mutation operator — useful for isolating what the LLM actually contributes.

## A partial instance: evolution as one setting, not the architecture

[KernelEvolve](../sources/kernelevolve.md) is worth recording here as a boundary case. It satisfies the
defining property — code-valued candidates, LLM-authored edits, execution-grounded selection with a hard
correctness constraint (`F = 0` on any `allclose` or compilation failure) — but it does **not** commit to
evolution as its architecture. Its selection policy `π_sel` is explicitly pluggable between greedy search,
MCTS with UCT, and "evolutionary algorithms maintaining populations of diverse candidates for crossover and
mutation" (source §3.1, p.12). Evolution is one configuration among three, and the paper never reports which
policy produced which of its production results.

The contrast with AlphaEvolve is sharp and worth holding: AlphaEvolve's distinctive machinery is the
**population database** (MAP-elites × islands) deciding which candidates seed the next generation, and its
ablations show every component of that machinery contributes. KernelEvolve's distinctive machinery is
instead the **prompt** — a diagnosis stage plus retrieval from a hand-authored hardware knowledge base
determining what the model *knows* when it writes each candidate (see
[`retrieval-augmented-prompt-synthesis`](retrieval-augmented-prompt-synthesis.md)). Same bargain, opposite
investment: one system spends its complexity budget on *which parent to mutate*, the other on *what the
mutation operator has read*.

> [!inferred] These are not competing answers to one question — they are answers to different questions, and
> which one dominates likely depends on whether the base model already knows the domain. AlphaEvolve's
> targets (matrix decomposition, bin-packing heuristics, open math) are all well within a frontier model's
> pretraining, so the binding constraint is search: how to escape local optima across generations. MTIA
> kernels are outside *any* model's pretraining, so the binding constraint is knowledge: no selection policy
> recovers a fact the model has never seen. Neither paper tests the other's regime, which makes this a clean
> open question rather than a resolved trade-off.

> [!inferred] Related but distinct: this concept is narrower than "AI-scientist / research agents" broadly
> (many of which reason in natural language and need no programmatic evaluator) and narrower than
> classical NAS/AutoML (which search configuration spaces with fixed operators). The distinguishing
> combination is: code-valued candidates + LLM-as-operator + execution-grounded evolutionary selection.

## When the mutation operator is trained rather than prompted

Every instance above uses a **frozen** LLM as the mutation operator — the whole paradigm's premise is that a
good outer loop extracts more capability from a fixed model. [Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md)
(arXiv:2607.28568) breaks that premise: it **post-trains the mutation operator on the outcomes the
evolutionary loop itself produces**, with SFT and RL targeting the same `Draft`/`Improve`/`Debug`/`Crossover`
transformations the search later composes ([`program-evolution-operators`](program-evolution-operators.md)).

All three pillars of the Core Mechanism survive intact — code-valued candidates, LLM-authored edits,
execution-grounded selection with a hard validity gate — so this is an instance of the concept, not a
departure from it. What changes is where the improvement accumulates. The two-way ablation separates them
on MLE-Bench Lite: holding the harness fixed and swapping in the trained model is worth **+21.22 pp** Medal
Average; holding the model fixed and swapping in the better harness is worth **+7.58 pp**; they compose. So
the harness-extracts-more-from-a-fixed-model thesis is not wrong — it is the *smaller* of the two effects
here. See [`meta-evolution`](meta-evolution.md).

Two design consequences the frozen-model instances never face, both from §4.3:

- **Reward scales must be re-derived on-policy.** AlphaEvolve's `evaluate` returns whatever the problem's
  natural metric is and the database ranks on it. To *train* on those scores across heterogeneous tasks you
  need them comparable, and fixed leaderboard or theoretical bounds are far wider than the region a policy
  actually occupies — "meaningfully different programs collapse to nearly identical rewards." OpenMLE
  derives bounds from each task's historical **on-policy score frontier**, moving with the policy.
- **Best-of-budget must be written into the loss.** Evolutionary search is judged on the single best
  program found, so uniformly reinforcing every non-failing candidate is the wrong update. An **entropic
  advantage** (an exponential tilt replacing GRPO's group normalization) concentrates the signal on a
  group's top candidates — measured best-candidate advantage 1.58 → 6.39.

> [!inferred] Selection pressure is the one thing every system on this page already had; what
> Frontis-MA1 shows is that the *same* selection signal can be spent twice — once to choose which child
> survives this generation, and again as a training weight that makes the next generation's proposals
> better a priori. openevolve's cascade evaluator computes exactly the scalar this would need. Nothing in
> the architecture of AlphaEvolve or openevolve forbids it; they simply don't own the model.

## In this wiki

- Papers: [AlphaEvolve](../sources/alphaevolve.md) (canonical);
  [Frontis-MA1](../sources/frontis-ma1.md) (the trained-operator variant);
  [KernelEvolve](../sources/kernelevolve.md) (the boundary case above). Referenced as an architectural
  family in the [AI-for-Auto-Research roadmap survey](../sources/ai-for-auto-research-roadmap.md).
- Topics: appears in both [autoresearch](../topics/autoresearch.md) (as a search-based/self-improving
  system) and [auto-optimization](../topics/auto-optimization.md) (as LLM-driven superoptimization) — this
  concept is the mechanism those two entries share.

## Grounded in code

[`openevolve`](../code/openevolve/overview.md) is this concept's first grounded implementation in the
wiki (previously paper-only, cited only through AlphaEvolve's white paper) — an independent open-source
reimplementation of the AlphaEvolve recipe, not DeepMind's own code. Reading the source confirms all
three pillars of the Core Mechanism above are real, load-bearing subsystems, not a paraphrase of the
paper:

- **Selection = population database.** [`ProgramDatabase`](../code/openevolve/concepts/openevolve-database.md)
  implements MAP-elites **per island**: several independent sub-populations each run their own
  feature-grid elitism, so five islands can hold five different solutions in the same behavioral cell
  instead of one global grid collapsing them — the concrete mechanism behind "balancing exploration vs.
  exploitation." A hard-learned migration ratchet (a documented production incident let one program spawn
  183 descendant copies via unrestricted re-migration) shows this database is a maintained system, not a
  textbook data structure.
- **Mutation = LLM diff.** [`LLMEnsemble`](../code/openevolve/concepts/openevolve-llm-ensemble.md) reduces
  AlphaEvolve's cheap/fast + expensive/capable model mixing to a weighted random draw per call (the
  shipped default: 80% `gemini-2.0-flash-lite`, 20% `gemini-2.0-flash`) — reproducing the paper's Flash+Pro
  ensemble idea as a two-line config, not a bespoke dispatcher. The diff itself is applied by
  [SEARCH/REPLACE splicing](../code/openevolve/concepts/openevolve-utils-code_utils.md): an exact,
  sequential, whitespace-sensitive line-match with no AST and no fuzzy matching — simple by design, at
  the cost of pushing exact reproduction onto the LLM's output.
- **Selection pressure = the cascade evaluator.** [`Evaluator`](../code/openevolve/concepts/openevolve-evaluator.md)
  spends compute progressively (cheap stage 1 first, pricier stages only if a candidate clears a
  threshold) and folds an optional LLM-judged qualitative pass back into the *same* scalar
  `combined_score` the database selects on — never a separate qualitative channel.
- **Orchestration.** [`OpenEvolve.run`](../code/openevolve/concepts/openevolve-controller.md) ties the
  three together inside a [process pool](../code/openevolve/concepts/openevolve-process_parallel.md) with
  a strict single-writer design (only the main process ever mutates the database), and
  [`PromptSampler`](../code/openevolve/concepts/openevolve-prompt-sampler.md) is the sole translation
  layer that re-derives evolutionary state into the natural-language prompt a stateless LLM needs on
  every call.

**Where this sits among the wiki's other self-improvement mechanisms:** openevolve evolves an arbitrary
*user-supplied target program*, not the agent's own source — unlike
[self-referential-code-rewriting](self-referential-code-rewriting.md) (DGM rewrites the coding agent
itself) and [mechanism-level-self-improvement](mechanism-level-self-improvement.md) (Bilevel Autoresearch
rewrites the search mechanism, keeping exactly one active variant). Its population database is closer in
spirit to DGM's growing archive — both keep a diverse set of historical variants rather than a single
hill-climbing lineage (see [evolutionary-self-improvement](evolutionary-self-improvement.md)) — but
openevolve's archive is a MAP-elites feature grid over an externally-scored artifact, while DGM's archive
is scored by the agent's own benchmark performance after each self-edit. The shared thread across all
three is *keeping more than one candidate alive at once so search doesn't collapse to a single lineage* —
they differ in **what** gets evolved (target artifact vs. agent vs. mechanism) and **how much** of the
population survives between rounds.

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **evolutionary-algorithm-discovery** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [openevolve](../code/openevolve/concepts/openevolve-controller.md) — OpenEvolve's main evolution loop — orchestrating LLM mutation, cascade evaluation, and MAP-Elites/island selection
- [openevolve](../code/openevolve/concepts/openevolve-database.md) — The program database — MAP-Elites × island model for evolutionary code search
- [openevolve](../code/openevolve/concepts/openevolve-evaluator.md) — Evaluator — cascade evaluation with folded-in LLM judgment
- [openevolve](../code/openevolve/concepts/openevolve-llm-ensemble.md) — LLM Ensemble — weighted model sampling as the mutation operator
- [openevolve](../code/openevolve/concepts/openevolve-process_parallel.md) — Process-based parallel evolution (ProcessParallelController)
- [openevolve](../code/openevolve/concepts/openevolve-prompt-sampler.md) — Prompt sampler — assembling what the LLM mutation operator sees
- [openevolve](../code/openevolve/concepts/openevolve-utils-code_utils.md) — SEARCH/REPLACE diffs — turning an LLM's text output into a child program
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-RL-airaevo_experience.md) — airaevo_experience.py — the original-AIRA-Evo selection/memory adapter for RL rollouts
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-RL-generate_mle.md) — The RL rollout — operator-conditioned generation and reward computation
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-RL-program_database.md) — Program database — three-term fitness and operator-conditioned parent sampling
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-program_database.md) — Program database — reward-as-fitness store behind SFT's greedy draft/improve search
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md) — GeneratorService — the operator-agnostic LLM caller behind tts_search's SFT trajectory collection
- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md) — Scheduler — the tts_search orchestrator behind the SFT evolutionary path
- [openrsi](../code/openrsi/concepts/OpenMLE-Evo-tts_search-program_database.md) — Program database — the storage substrate, not the selection policy
<!-- connect:auto:end -->
