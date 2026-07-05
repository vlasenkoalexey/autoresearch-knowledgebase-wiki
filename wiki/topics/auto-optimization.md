# Auto-optimization

This wiki's second core topic: automating the *tuning* of models, systems, and code — AutoML, hyperparameter
optimization, neural-architecture search (NAS), learned optimizers, and compiler / kernel / schedule
auto-tuning — as opposed to [Autoresearch](autoresearch.md), which automates the research process itself
(hypotheses, experiments, write-ups). The boundary is deliberately porous: an LLM agent that optimizes a GPU
kernel *is* both an auto-research coding agent and an auto-optimization method, and the systems below that sit
on that seam are cross-linked from both topic pages.

> This page is a stub seeded during the first papers pass. It currently holds only the auto-optimization
> facet of bridge systems; the dedicated learned-optimizer / NAS / kernel-autotuning literature will be
> filled in as those papers are ingested.

## LLM-driven auto-tuning / superoptimization

### AlphaEvolve as an auto-optimization / superoptimization system

[AlphaEvolve](../sources/alphaevolve.md) (Novikov et al., arXiv:2506.13131) is not only an autoresearch agent
(see [Autoresearch › Evolutionary and algorithm discovery](autoresearch.md)) — four of its case studies are
production **auto-optimization** results on Google's compute stack, making it this wiki's principal bridge
between the two topics. The paper frames the method as **code superoptimization** (iteratively improving a
program under execution feedback), with the twist that the search operator is an LLM proposing semantically
meaningful, context-informed code edits rather than the handwritten mutation operators of classical genetic
programming or the fixed sampling of hyperparameter-space AutoML/NAS. Concrete wins:

- **Data-center scheduling** — evolved a closed-form heuristic for Google's Borg cluster scheduler (framed as
  2D vector bin-packing); deployed fleet-wide, recovers ~0.7% of Google's fleet-wide compute that would
  otherwise be stranded. Chosen over deep RL for interpretability/debuggability.
- **Kernel auto-tuning** — evolved tiling heuristics for a Pallas TPU matmul kernel used to train Gemini; 23%
  average kernel speedup, 1% cut in Gemini's total training time, months of tuning compressed to days (a case
  of Gemini optimizing its own training).
- **Hardware/RTL** — simplified a verified Verilog TPU arithmetic circuit (Gemini's first direct contribution
  to TPU arithmetic circuits).
- **Compiler auto-optimization** — operated directly on XLA-generated IR for FlashAttention: 32% kernel
  speedup, 15% on pre/postprocessing, each numerically verified against the reference.

Its direct ancestor is **FunSearch** (Romera-Paredes et al., 2023): AlphaEvolve extends single-function Python
evolution to whole-codebase multi-language multi-objective evolution with frontier LLMs and rich NL context.
Relative to classical NAS / learned-optimizers / compiler auto-tuning, its differentiator is the
LLM-as-mutation-operator carrying world knowledge into the search. See
[`evolutionary-algorithm-discovery`](../concepts/evolutionary-algorithm-discovery.md).

### RD-Agent(Q)

[RD-Agent(Q)](../sources/rd-agent.md) (Microsoft, arXiv:2505.15155) is the auto-optimization-flavored half of
the [RD-Agent](../sources/rd-agent.md) project: it co-optimizes quant-finance trading factors and models with
a contextual-bandit scheduler deciding each round which axis to improve. See
[Autoresearch › Industrial R&D loop](autoresearch.md) and
[`closed-loop-experiment-design`](../concepts/closed-loop-experiment-design.md).
