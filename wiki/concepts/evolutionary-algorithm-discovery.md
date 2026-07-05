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

> [!inferred] Related but distinct: this concept is narrower than "AI-scientist / research agents" broadly
> (many of which reason in natural language and need no programmatic evaluator) and narrower than
> classical NAS/AutoML (which search configuration spaces with fixed operators). The distinguishing
> combination is: code-valued candidates + LLM-as-operator + execution-grounded evolutionary selection.

## In this wiki

- Papers: [AlphaEvolve](../sources/alphaevolve.md) (canonical). Referenced as an architectural family in
  the [AI-for-Auto-Research roadmap survey](../sources/ai-for-auto-research-roadmap.md).
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
<!-- connect:auto:end -->
