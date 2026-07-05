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
