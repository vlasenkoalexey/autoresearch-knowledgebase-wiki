# Auto-optimization

This wiki's second core topic: automating the *tuning* of models, systems, and code — AutoML, hyperparameter
optimization, neural-architecture search (NAS), learned optimizers, and compiler / kernel / schedule
auto-tuning — as opposed to [Autoresearch](autoresearch.md), which automates the research process itself
(hypotheses, experiments, write-ups). The boundary is deliberately porous: an LLM agent that optimizes a GPU
kernel *is* both an auto-research coding agent and an auto-optimization method, and the systems below that sit
on that seam are cross-linked from both topic pages.

> Formerly a stub holding only the auto-optimization facet of bridge systems. [KernelEvolve](../sources/kernelevolve.md)
> (Meta, ISCA 2026) is the first ingested paper whose center of mass is *here* rather than on the autoresearch
> side, and it anchors the kernel-auto-tuning section below. The learned-optimizer / NAS / AutoML literature
> proper is still unfilled — those sections remain stubs, marked as such.

## LLM-driven kernel generation and auto-tuning

The most active area in this topic, and the one this wiki currently covers best. The shared shape:
**a candidate kernel is code, the objective is measured wall-clock time on real silicon, and correctness is
enforced by differential testing against a reference implementation** — so the harness, not the model's
self-report, decides what survives. See [`llm-kernel-generation`](../concepts/llm-kernel-generation.md) for
the concept page and how the systems differ.

### KernelEvolve (Meta) — the production deployment

[KernelEvolve](../sources/kernelevolve.md) ([arXiv:2512.23236](../../raw/papers/kernelevolve.pdf), ISCA 2026)
is an agentic framework generating and optimizing **Triton** kernels across NVIDIA GPUs, AMD GPUs, and Meta's
proprietary **MTIA** accelerators, running continuously in Meta's ads-ranking infrastructure. It is this
wiki's reference point for what auto-optimization looks like when it has to actually ship:

- **Kernel optimization formalized as graph search** `(F, π_sel, O, τ)` — fitness `F = t_pytorch/t_triton`
  with `F = 0` for any kernel failing `torch.allclose` or compilation; selection policy `π_sel` pluggable
  between greedy, MCTS/UCT, and evolutionary population search; a **single universal operator** `O`; a
  budget/stall/threshold termination rule `τ`.
- **The universal operator argument.** Prior frameworks bind specialized operators (`Draft`, `Debug`,
  `Improve`) to static prompt templates that cannot adapt to runtime context — a `Debug` prompt is
  error-focused whether the fault is algorithmic or a memory-access pattern. KernelEvolve replaces all of
  them with one operator whose behavior comes entirely from retrieval-augmented dynamic prompt synthesis.
  The cited premise (Toledo et al., 2025) is that **operator design, not the search algorithm, is the
  bottleneck** in LLM code generation. See
  [`retrieval-augmented-prompt-synthesis`](../concepts/retrieval-augmented-prompt-synthesis.md).
- **A hardware knowledge base as the retrieval target.** ≥100 hand-authored documents across
  `constraints/` (anti-cheating rules — no library wrappers, no direct CUDA API), `guidance/`, and
  `hardware/{nvidia,amd,mtia}/`, navigated via an `index.md`. This is what makes a *proprietary, undocumented*
  accelerator tractable: MTIA is absent from public training corpora, so the missing facts (SFU libdevice
  mappings, `cb_multiplier`/`use_dual_core` compile options, cross-PE `direction` broadcast/reduction,
  `tl.pe_runtime_barrier()`) are written down and retrieved in-context rather than fine-tuned in — "enabling
  immediate LLM-based kernel generation **without model retraining**" (§3.2.3).
- **Results.** 480/480 correct across 160 ATen operators × 3 platforms; 100% KernelBench pass rate (all 250
  problems, all three levels); **1.25–17×** over PyTorch baselines on production workloads; weeks → hours.
- **The honest parts.** Generated kernels are *specialized to production shape distributions* and lose on
  out-of-distribution inputs (0.39–0.63× on shapes outside the target), so deployment needs **shape-aware
  dispatch with fallback to vendor libraries**. And on trivial ATen primitives, only four of six tracked
  operators exceed 1.0× at all.

### The measurement gradient: where automated kernels win

KernelEvolve's cross-platform conv1d experiment (same spec, five platforms) is the cleanest datum in this
wiki on *where* automated kernel generation pays: vs. a tuned `conv2d` + `channels_last` + cuDNN baseline the
gains are **1.06× on AMD MI350, 1.25× on MI300, 1.35× on A100, 1.62× on H100 — and 4.71× on MTIA v3**. Gains
are smallest where vendor libraries are most mature and largest on the proprietary accelerator with the
thinnest ecosystem.

> [!inferred] Read together with the MTIA preprocessing case studies — where the generated kernel is not
> faster than the alternative but *is* the only on-device implementation, because the ATen operator does not
> exist on that hardware at all — the through-line is that **the value of automated kernel generation is
> inversely proportional to the maturity of the target's software ecosystem**. That reframes the economics:
> this is less "beat cuBLAS" than "make a new accelerator usable before its library ecosystem exists," which
> also explains why an ASIC vendor rather than a GPU vendor built and deployed it first.

### Kernel coverage as an architectural constraint, not a performance knob

The most transferable systems argument in [KernelEvolve](../sources/kernelevolve.md) has nothing to do with
LLMs. A *missing* preprocessing kernel is a **binary deployment constraint**: without a native accelerator
implementation the model must be split across a CPU preprocessing tier and an accelerator tier, and the
paper prices that tax on a real MTIA deployment at **P99 61 ms → 97 ms, of which 10–20 ms is pure network
overhead** buying nothing, against a sub-100 ms serving budget. Ads ranking runs 200+ preprocessing
operators with irregular access patterns and data-dependent control flow, so "generate a kernel that merely
*works*" carries more system value than "make an existing kernel faster." Any auto-optimization system
targeting new accelerators should be evaluated on coverage first and speedup second — which is exactly the
order KernelEvolve's own evaluation takes (§4 correctness, then §5 speedup).

### The TPU autoresearch wiki's kernel lane — the directed alternative

The [TPU performance autoresearch wiki](../sources/tpu-performance-autoresearch-wiki.md) added a **kernel
lane** in July 2026, applying its model-lane autoresearch loop to hand-written **Pallas/Mosaic** kernels on
TPU. It is this wiki's only kernel system whose next candidate comes from a **diagnosis** rather than from
selection over sampled variants — the full contrast is in
[`llm-kernel-generation`](../concepts/llm-kernel-generation.md#directed-search-vs-selection-driven-search).
What is distinctive as *auto-optimization* method:

- **A cost-ordered ladder of intervention classes** — `refute → flag → xla-rewrite → kernel-authored` —
  where authoring a kernel is the *last*, most expensive option and each cheaper class must be ruled out
  first. The stated discriminating skill is "not forcing a kernel where a flag, a rewrite, or a refute is
  correct."
- **`refuted` as a first-class verdict.** If the compiler is already fusion-complete and near roofline, "no
  kernel can win here" is the correct outcome, filed with the bound and the blocker. Sharpened by a rule
  worth generalizing: a `refuted` verdict confirms a *bound* **only from a candidate that passes the
  correctness gate** — a wrong kernel's timing says nothing about the operator's ceiling.
- **Enumerated levers make coverage a set-diff.** Each of seven kernel categories has a class page whose
  `## Levers (verified)` list is the checklist a family must exhaust (tried-with-receipt, or ruled out
  against the lever's *mechanism*) before it may claim to be at ceiling — with a consecutive-lever limit and
  bounded deferral enforced at hypothesis-*selection* time, not just at close time.
- **Provenance decides what a result may claim.** Operating points must come from real model-lane profiles
  (`activity: optimization`); benchmark-suite op-points are `capability-eval` and are structurally barred
  from updating any model frontier. And a kernel win never flips the model frontier by itself — it spawns a
  model-lane experiment that must validate end-to-end first, because kernel-level wins are refuted by
  dispatch overhead and op-point mismatch often enough that skipping the step is a known failure mode.
- **The measurement is an artifact, not an assertion** — a self-hashed receipt from a single measurement
  tool, produced by a verifier process that is not the author. See
  [`verification-independence`](../concepts/verification-independence.md).

Reported result, as published in the project's own README and interactive kernel explorer: GQA attention on
one v6e chip against a hand-tuned reference's published 2.48× — Claude Opus 5 **6.77×** over 22 experiments,
Codex GPT-5.6 3.73× over 9, Gemini Flash 3.6 3.51× over 12. Treat the per-arm figures as a **snapshot of one
kernel family**, not a settled benchmark: they are single-arm runs on a live campaign, the explorer is
regenerated as branches land, and the project reports numbers per family rather than as an aggregate score.
The robust part of the result is the ordering (all three arms above the reference) and the *shape*: as with
[KernelEvolve](../sources/kernelevolve.md)'s 50–300-step searches, depth matters — most experiments do not
move the frontier, which advances in a staircase of rare structural changes separated by long flat runs of
refuted hypotheses.

### The classical lineage this builds on

KernelEvolve's related work (§7) situates LLM kernel agents against decades of auto-tuning: **Halide**
(Ragan-Kelley et al., 2013) decoupling algorithm from schedule; **TVM** (Chen et al., 2018) adding learned
cost models for automated schedule search; **Triton** (Tillet et al., 2019) as a block-level
Python-embedded DSL; and the newer abstraction layers — NVIDIA's **CuTe** DSL (CUTLASS v4), Meta's **TLX**
(warp-aware intrinsics, explicit pipeline control for Hopper/Blackwell), OpenAI's **Gluon** dialect,
**TileLang**, and **Helion** (PyTorch-like syntax compiled to autotuned Triton). The paper's position: these
reduce effort but "still require substantial domain expertise for novel kernel transformations and struggle
to generalize across heterogeneous hardware without manual adaptation." Also relevant and pre-LLM:
**GEVO/GEVO-ML** (Liou, Forrest, Wu et al., 2019–2022) applied evolutionary computation to GPU code at the
LLVM/MLIR level with *handwritten* transformation operators — the direct ancestor of
[`evolutionary-algorithm-discovery`](../concepts/evolutionary-algorithm-discovery.md) with the LLM swapped in
for the mutation operator.

### The rest of the field (not yet ingested)

KernelEvolve's §1 and §7 inventory the LLM-kernel landscape; none of these are in this wiki as papers yet,
listed here as a reading queue: **KernelBench** (Ouyang et al., 2025 — the standard benchmark, three
difficulty tiers), **AutoTriton** (Tsinghua, RL post-training for Triton), **KernelLLM** and **CWM**
(Meta — supervised Triton generation; open-weights code world model), **TritonRL** (Amazon, execution-guided
rewards), **GEAK** (AMD, agentic Triton for MI300X/MI250), **Kevin** (Cognition, multi-turn RL for CUDA),
**KernelAgent** (PyTorch, multi-agent verified Triton), and **TritorX** (Hammond et al., 2025,
[arXiv:2512.10977](https://arxiv.org/abs/2512.10977) — agentic operator generation for ML ASICs, the direct
MTIA-facing predecessor).

## LLM-driven superoptimization / algorithm discovery

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

### AlphaEvolve vs. KernelEvolve on the same task

Both attack kernel auto-tuning with LLM-driven search graded by measured execution, and both shipped. The
axis that separates them is **generality vs. heterogeneity**. AlphaEvolve is one mechanism (evolutionary
population search over code) applied to everything from open mathematics to TPU circuits, all inside
Google's stack. KernelEvolve is one task (kernel synthesis) with a pluggable search policy — evolution is
merely one setting of `π_sel` next to greedy and MCTS — applied across three vendors, including an
accelerator no pretrained model has ever seen. Consequently their distinctive machinery differs: AlphaEvolve
invests in the **population database** (MAP-elites × islands) governing which candidates seed the next
generation; KernelEvolve invests in the **knowledge base and dynamic prompt synthesis** governing what the
model knows when it writes each candidate. KernelEvolve's own related-work characterization of AlphaEvolve as
"synthetic workloads / single hardware platform" is contested on
[`sources/kernelevolve.md`](../sources/kernelevolve.md).

### Recursive — SOL-ExecBench, a different metric shape

[Recursive's report](../sources/recursive-automated-ai-research.md) (blog, 2026-06) improves NVIDIA's
SOL-ExecBench mean score 0.699→0.754 across 235 kernels (an 18% reduction in the remaining gap to the 1.0
speed-of-light ceiling) via bit-packed MoE routing, native-PTX FP4 packing, and fused-reduction GQA decode
kernels. The SOL metric is a fraction-of-theoretical-ceiling score, not KernelEvolve's `t_pytorch/t_triton`
ratio, so the two results are not directly comparable in magnitude — see
[`sources/recursive-automated-ai-research.md`](../sources/recursive-automated-ai-research.md) for the caveat.
Like the same report's `autoresearch` benchmark result (see [Autoresearch › Self-improving research
loops](autoresearch.md)), the article names no search/ratchet mechanism, so read the number as reported
rather than as a grounded method comparison.

### Frontis-MA1 / OpenMLE — AutoML's target, reached by trained code evolution

[Frontis-MA1](../sources/frontis-ma1.md) (arXiv:2607.28568) optimizes precisely what classical AutoML
optimizes — feature engineering, model selection, hyperparameters, validation strategy, ensembling — but
through open-ended program evolution rather than a search over a predefined pipeline space. The paper draws
that contrast itself (§7, p.29): "Classical AutoML optimizes over predefined model and pipeline spaces
[AutoGluon, auto-sklearn, TPOT, Auto-WEKA], whereas LLM-based MLE agents operate through open-ended,
code-mediated experimentation." Its own Figure 2 places AutoML, NAS, and RLAIF/self-play as sibling rungs
of one AI4AI ladder, with MLE as the executable testbed for all of them.

What makes it belong on *this* page rather than only on [Autoresearch](autoresearch.md) is where the
optimization pressure now lives. AlphaEvolve's thesis is that a good outer loop extracts more from a fixed
model. Frontis-MA1's is that the same outer loop extracts substantially more from a model **trained for
that loop's specific moves** — `Draft`/`Improve`/`Debug`/`Crossover` become SFT and RL targets, not prompt
roles. The evidence separates the two contributions cleanly: **+21.22 pp** Medal Average on MLE-Bench Lite
from post-training at fixed harness, **+7.58 pp** from the harness at fixed model, composing to 71.21% from
a 35B open model on a single 12 GB RTX 4090. See [`meta-evolution`](../concepts/meta-evolution.md).

The efficiency result is the other reason it sits here: against the same checkpoint under original AIRA-Evo
over 66 matched task–runs, operator-conditioned bounded context cuts total model tokens **41.7%** while
evaluated nodes fall only 12.4%, raising new-best validation updates per million tokens **1.77 → 3.27**.
That is an auto-tuning result about the *search harness itself* — cost per useful discovery, not just final
score. Its benchmark context is on
[MLE agents and their benchmarks](mle-agents-and-benchmarks.md).

### RD-Agent(Q)

[RD-Agent(Q)](../sources/rd-agent.md) (Microsoft, arXiv:2505.15155) is the auto-optimization-flavored half of
the [RD-Agent](../sources/rd-agent.md) project: it co-optimizes quant-finance trading factors and models with
a contextual-bandit scheduler deciding each round which axis to improve. See
[Autoresearch › Industrial R&D loop](autoresearch.md) and
[`closed-loop-experiment-design`](../concepts/closed-loop-experiment-design.md).

### Bilevel Autoresearch — optimizing the optimizer

[Bilevel Autoresearch](../sources/bilevel-autoresearch.md) belongs here too, one level up: rather than tuning
an artifact, its outer loop writes and injects new *search mechanisms* (Tabu search, bandits, orthogonal
design-of-experiments) into a running inner optimization loop. Its finding — parameter-level tuning of the
inner loop gave no reliable gain while mechanism-level rewriting gave ~5× — is the sharpest evidence in this
wiki that in LLM-driven optimization the **search mechanism matters more than its hyperparameters**, which
rhymes with KernelEvolve's operator-not-algorithm premise. See
[`mechanism-level-self-improvement`](../concepts/mechanism-level-self-improvement.md).

## Model- and systems-level performance optimization

The [TPU model performance work](../sources/2026-05-01-tpu-model-performance-auto-optimization.md) that
motivated this wiki has a **model lane** at a coarser granularity than kernels: an agent optimizing a whole
training harness's MFU (sharding, remat, batch/sequence layout, compiler flags) rather than a single
operator. The [methodology page](../sources/tpu-performance-autoresearch-wiki.md) documents its
phase-ordering discipline, HLO/AOT pre-filters, and falsifiability requirements.

> [!warning] Superseded by the 2026-08-06 re-ingest of [`tpu-performance-autoresearch-wiki`](../sources/tpu-performance-autoresearch-wiki.md)
> This section previously described that project as operating *only* at model granularity, with
> KernelEvolve as "the industrial-scale point of comparison one level down." It now runs **both**
> granularities: the kernel lane added in July 2026 optimizes individual Pallas kernels, and the two lanes
> are explicitly coupled (a slow op found in a model profile spawns a kernel family at that exact operating
> point; a kernel win merges only after it re-validates end-to-end in the model lane). See
> [the kernel-lane section above](#the-tpu-autoresearch-wikis-kernel-lane--the-directed-alternative) and the
> relation section in [`sources/kernelevolve.md`](../sources/kernelevolve.md).

## Still stubs

- **AutoML / hyperparameter optimization** — nothing ingested yet.
- **Neural architecture search (NAS)** — nothing ingested yet. KernelEvolve gestures at the intersection in
  §6, proposing co-optimization of model structure (quantization, sparsity, architecture search) *with*
  kernel implementation.
- **Learned optimizers** — nothing ingested yet.
- **Compiler / schedule auto-tuning proper** (Halide/TVM/Ansor lineage) — referenced above through
  KernelEvolve's related work, but no primary source ingested.
