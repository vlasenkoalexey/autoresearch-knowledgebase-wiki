# AlphaEvolve: A Coding Agent for Scientific and Algorithmic Discovery

**Source:** A. Novikov, N. Vũ, M. Eisenberger, E. Dupont, P.-S. Huang, A. Z. Wagner, S. Shirobokov,
B. Kozlovskii, F. J. R. Ruiz, A. Mehrabian, M. P. Kumar, A. See, S. Chaudhuri, G. Holland, A. Davies,
S. Nowozin, P. Kohli, M. Balog (Google DeepMind), "AlphaEvolve: A coding agent for scientific and
algorithmic discovery," arXiv:2506.13131 (16 Jun 2025). Accompanying results repo:
[google-deepmind/alphaevolve_results](https://github.com/google-deepmind/alphaevolve_results). An
independent open-source reimplementation exists — [codelion/openevolve](https://github.com/codelion/openevolve)
— but it is **not** the object of this summary; this page is about the DeepMind white paper only.
Raw source: [`../../raw/papers/alphaevolve.pdf`](../../raw/papers/alphaevolve.pdf).

> [!note] **This paper is a deliberate bridge in this wiki.** It is simultaneously an **autoresearch**
> system (an autonomous agent that runs its own discovery loop over open scientific/mathematical
> problems, with essentially no human in the loop once the task is specified) and an
> **auto-optimization** system (four of its case studies are, concretely, kernel/compiler/scheduling
> auto-tuning against a real production compute stack). It should be linked from both topic pages.

## What this paper is

A white paper (not a peer-reviewed conference submission) presenting **AlphaEvolve**, an evolutionary
coding agent built on top of Gemini that "substantially enhances capabilities of state-of-the-art LLMs
on highly challenging tasks such as tackling open scientific problems or optimizing critical pieces of
computational infrastructure" (p.1). It is explicitly framed as a major extension of DeepMind's earlier
**FunSearch** system (Romera-Paredes et al., 2023) — same family of LLM-guided evolutionary code search,
but scaled up to evolve entire codebases with frontier LLMs rather than a single short function with a
small code-only model.

## The evolutionary loop over code

At its core, AlphaEvolve is an evolutionary algorithm whose mutation operator is an LLM. The loop
(Figures 1–2, p.3–4):

1. **Task specification.** The human supplies (a) an *initial program*, with the parts open to change
   wrapped in `# EVOLVE-BLOCK-START` / `# EVOLVE-BLOCK-END` markers — the rest of the file is a fixed
   skeleton that invokes the evolved pieces — and (b) an `evaluate` function `h` that maps a candidate
   program to a dictionary of scalar metrics to be maximized (§2.1, p.3–4). This is the load-bearing
   design choice: the human defines *what* "better" means and provides a starting point; AlphaEvolve
   figures out *how* to get there (Figure 1).
2. **Sample and prompt.** The controller samples a parent program plus "inspiration" programs from the
   **program database** and the **prompt sampler** assembles a rich prompt: prior solutions and their
   scores, explicit problem context (equations, code snippets, even PDFs of relevant literature),
   stochastic template variation, and — optionally — a *meta-prompt* that the LLM itself evolves in a
   parallel database (§2.2, p.5).
3. **Propose.** An **ensemble of LLMs** — Gemini 2.0 Flash (cheap/fast, for volume) and Gemini 2.0 Pro
   (expensive/capable, for occasional breakthroughs) — generates a code modification, formatted as
   `SEARCH/REPLACE` diff blocks (or a full rewrite for short programs) (§2.3, p.5–7, Figure 3).
4. **Evaluate.** The diff is applied and the resulting child program is scored by the `evaluate`
   function. AlphaEvolve supports an **evaluation cascade** (cheap/small tests first, to kill broken
   programs fast, before expensive full-scale tests), **LLM-generated feedback** for qualities hard to
   score programmatically (e.g. "simplicity"), and **parallelized, hours-long evaluation** on
   accelerators for evaluations too expensive to run serially (§2.4, p.7–8).
5. **Register and repeat.** Surviving programs go back into the **program database**, whose selection
   algorithm is "inspired by a combination of the MAP-elites algorithm and island-based population
   models" (§2.5, p.8) — it balances exploiting the best-known programs against keeping enough
   diversity to escape local optima. The whole thing runs as an asynchronous (`asyncio`) distributed
   pipeline of a controller, LLM samplers, and evaluator nodes, optimized for **throughput** — maximizing
   the number of ideas proposed-and-scored per unit of compute, not the latency of any one evaluation
   (§2.6, p.8).

Because every proposal is graded by real code execution rather than accepted on the LLM's say-so,
"this evaluation mechanism allows AlphaEvolve to avoid any incorrect suggestions from the base LLM"
(p.2) — correctness is enforced by the harness, not by trusting the model.

## How it differs from FunSearch and single-shot agents

Table 1 (p.3) is the paper's own side-by-side against its direct predecessor, FunSearch:

| | FunSearch | AlphaEvolve |
|---|---|---|
| scope | evolves a single function | evolves an entire code file |
| size | ≤10–20 lines | up to hundreds of lines |
| language | Python only | any language |
| evaluation | must finish in ≤20 min on 1 CPU | can run for hours, in parallel, on accelerators |
| samples | millions of LLM samples | thousands suffice |
| LLM size | small, code-only; no benefit from scale | benefits from SOTA/frontier LLMs |
| prompt context | minimal (prior solutions only) | rich natural-language context and feedback |
| objective | single metric | simultaneous multi-objective |

The paper also explicitly contrasts AlphaEvolve with **AI Co-Scientist** (Anand et al.), which
represents hypotheses and evaluation criteria in *natural language* across specialized agents. By
representing candidates as *code* graded by *programmatic* evaluators, AlphaEvolve "substantially
sidestep[s] LLM hallucinations," letting evolution run for far more steps without an LLM judge's
unreliability compounding (§5, p.19) — at the cost of only being applicable where an automated
evaluator can be written at all (see Limitations, below). This is the paper's core differentiator from
single-shot or sequential-pipeline research agents: rather than one LLM call (or one linear
plan→execute→report pipeline) producing a final answer, a *population* of candidate solutions is
continuously proposed, graded, and recombined, so that partial improvements compound across many
generations instead of being thrown away after one attempt.

## Concrete discoveries

### Faster matrix multiplication and a Strassen-beating result

Framed as low-rank tensor decomposition (the rank of the decomposition of the ⟨m,n,p⟩ matrix-product
tensor equals the number of scalar multiplications required), AlphaEvolve was given a simple
gradient-based decomposition algorithm as its initial program and asked to evolve it (§3.1, p.9–11).
Result: it **improved the best known rank for 14 different matrix-multiplication targets** (Table 2,
p.9). The headline result: multiplying two 4×4 complex-valued matrices using **48 scalar
multiplications**, beating the rank-49 bound obtainable by recursively applying Strassen's 1969
algorithm — "for 56 years, designing an algorithm with rank less than 49 over any field with
characteristic 0 was an open problem" (p.10). Figure 4 (p.11) shows the actual diff AlphaEvolve
produced — 15 mutations deep, rewriting the optimizer (Adam→AdamW), the initializer, the loss function
(adding discretization, hallucination, and gradient-noise terms), and the hyperparameter sweep — i.e.
qualitatively different code from the seed, not a local tweak.

### Open mathematical problems

Applied to a curated set of **over 50 open problems** spanning analysis, combinatorics, number theory,
and geometry, AlphaEvolve **matched the best known construction ~75% of the time** and **found a new,
better construction (surpassing SOTA) ~20% of the time**, always starting from a simple or random
construction (§3.2, p.10–13). Named results include an improved upper bound on **Erdős's minimum
overlap problem**, an improved lower bound on the **kissing number in 11 dimensions** (593 non-overlapping
unit spheres touching a central sphere, vs. the previous record of 592), and improvements to
autocorrelation inequalities and an uncertainty-principle construction. Methodologically, the paper
notes AlphaEvolve often does better by **evolving a heuristic search algorithm** (given a fixed compute
budget, e.g. 1000 seconds) rather than evolving the final construction directly — later generations
discover multi-stage strategies (crude-but-effective early heuristics, followed by fine-tuning
heuristics) that would be hard to hand-design (p.12). Several problems were suggested by, and
formulated in collaboration with, external mathematicians Terence Tao and Javier Gomez Serrano —
explicitly framed as human–AI collaboration rather than full autonomy (p.13, p.21).

### Google's compute stack (the auto-optimization case studies)

Four separate deployments, each a genuine production auto-tuning result (§3.3, p.13–17):

- **Data center scheduling.** Reframed as 2D vector bin-packing, AlphaEvolve evolved a heuristic
  scoring function (shown in closed form, Figure 6, p.14) for Google's Borg cluster scheduler. Deployed
  fleet-wide, it **recovers on average 0.7% of Google's fleet-wide compute resources** that would
  otherwise be stranded. The paper states it was preferred over a deep-RL approach specifically for
  interpretability, debuggability, and predictability, not just performance (p.14).
- **Gemini kernel engineering.** AlphaEvolve evolved tiling heuristics for a Pallas matrix-multiplication
  kernel used to train Gemini itself, optimizing directly against measured runtime on real TPUs. Result:
  an **average 23% kernel speedup** over the prior expert-designed heuristic and a **1% reduction in
  Gemini's overall training time** — compressing "several months of dedicated engineering effort" into
  "just days of automated experimentation" (p.15–16). The paper calls out that this is **Gemini
  optimizing its own training process** via AlphaEvolve — a small, concrete instance of the
  self-improving-loop idea, though the authors are careful to note current feedback loops for improving
  the *next* AlphaEvolve are still "on the order of months," not a runaway recursive loop (§6, p.21).
- **TPU arithmetic circuit design.** AlphaEvolve rewrote a Verilog RTL implementation of a TPU
  matrix-multiplication-unit arithmetic circuit, removing unnecessary bits while preserving verified
  functional correctness — validated by TPU designers and integrated into an upcoming TPU. The paper
  calls this "Gemini's first direct contribution to TPU arithmetic circuits" (p.16).
- **Compiler-generated code (XLA IR for FlashAttention).** Operating directly on XLA-generated
  intermediate representations (not source code — IR "designed for debugging purposes rather than
  direct editing"), AlphaEvolve sped up a FlashAttention kernel configuration by **32%** and its
  pre/postprocessing by **15%**, each change checked for numerical correctness against the reference
  implementation on randomized inputs and finally confirmed correct by human experts (§3.3.4, p.17).

## Ablations

Controlled comparisons on the matrix-decomposition and kissing-number tasks (§4, Figure 8, p.17–18)
remove one mechanism at a time — no evolution (repeatedly re-prompting from the same initial program),
no prompt context, no meta-prompt evolution, no full-file evolution (evolving only the loss function),
and a small-base-LLM-only ensemble — and find **every one of these components contributes a significant
share of the final performance**; none is redundant.

## Limitations (the authors' own, §6, p.21)

The central limitation is architectural, not incidental: AlphaEvolve **only works on problems for which
an automated evaluator can be written**. This covers much of mathematics and computer science but
excludes domains — natural sciences prominently among them — "where only some experiments can be
simulated or automated." The paper notes AlphaEvolve does support LLM-provided evaluation of ideas as a
fallback but "this is not a setting we have optimized for," and floats combining AlphaEvolve's
programmatic-evaluation regime with AI Co-Scientist-style natural-language hypothesis evaluation as
future work — LLM judgment for high-level ideas, then AlphaEvolve-style machine feedback once an idea is
reduced to code (p.21).

> [!inferred] The paper's own framing (§6) of AlphaEvolve as "a test-time compute agent that ...
> significantly enhances the capability of the base LLM" reads as a general recipe applicable beyond
> this paper's specific case studies: wherever a problem can be reduced to (a) a code representation of
> a candidate solution and (b) a programmatic scorer, an LLM-driven evolutionary outer loop appears to
> reliably extract more capability from a fixed base model than repeated independent sampling does. That
> generality — not any single discovery — is likely why this paper is being cited as a template by
> later systems (e.g. the open [openevolve](https://github.com/codelion/openevolve) reimplementation)
> that generalize the harness beyond DeepMind's internal infrastructure.

## Relation to this wiki's other systems

> [!inferred] Two topic-page connections worth drawing once those pages exist:
> - **vs. sequential/single-shot autoresearch pipelines** (The AI Scientist, Agent Laboratory-style
>   systems, or Karpathy's `autoresearch` harness already in this wiki's `code/autoresearch/overview.md`):
>   those systems run one attempt (or a short fixed sequence of attempts) per idea and keep/discard
>   against a single held-out metric; AlphaEvolve instead maintains a whole **population** of candidates
>   evaluated on possibly *multiple* metrics simultaneously, with an explicit exploration/exploitation
>   database (MAP-elites/island model) governing which candidates get to seed the next generation. This
>   is a materially different point in the design space, not just "more compute."
> - **vs. classical auto-tuning/NAS/AutoML**: the data-center-scheduling, kernel-tiling, and
>   circuit-design case studies are auto-tuning problems in the classical sense (a search over a space of
>   heuristics/configurations against a measured objective), but the search operator is an LLM proposing
>   semantically meaningful code edits (informed by natural-language context) rather than a
>   hyperparameter-space sampler or a fixed grammar of mutations — this is the paper's own contrast with
>   "handwritten evolution operators" in classical genetic programming (§5, p.18–19).
