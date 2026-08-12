# LLM kernel generation

**Definition.** LLM kernel generation is the use of a language model — usually inside an agentic search loop
— to author low-level accelerator kernels (Triton, CUDA, HIP, or a vendor DSL) from a higher-level
specification, where every candidate is judged by two mechanical signals: **differential correctness**
against a reference implementation, and **measured wall-clock time** on the target hardware. It is a special
case of [`evolutionary-algorithm-discovery`](evolutionary-algorithm-discovery.md)'s core bargain —
code-valued candidates graded by execution — applied to a domain where the evaluator is unusually cheap and
unusually trustworthy: `torch.allclose` plus a timer.

## Why this domain is a favorable one for agents

Three properties, none of which hold for research automation generally:

1. **The oracle is free.** A reference implementation already exists (the PyTorch eager or `torch.compile`
   version). Correctness is a numerical comparison, not a judgment call — no LLM-as-judge, no VLM reviewing
   plots, no human referee. Contrast [`agentic-tree-search`](agentic-tree-search.md), where AI Scientist-v2
   must trust an LLM+VLM verdict to decide whether a node is good.
2. **The objective is a scalar the hardware reports.** Speedup over the baseline. No proxy metric to game —
   the usual failure mode is instead *cheating on the constraint*: wrapping a vendor library, importing a
   pre-compiled routine, or falling back to a high-level PyTorch op that bypasses kernel-level work. Systems
   handle this with explicit anti-cheating rules ([KernelEvolve](../sources/kernelevolve.md)'s knowledge base
   has a whole `constraints/` subtree forbidding cross-platform abstractions, external library dependencies,
   and direct CUDA API usage).
3. **Failure is cheap and informative.** A bad kernel fails to compile or fails `allclose` in seconds, and
   the compiler/profiler emits structured diagnostics the next iteration can consume — instruction stalls,
   occupancy, memory throughput, register spills.

The counterweight: the search must run *long*. KernelEvolve reports 50-step searches for trivial ATen
operators and **300 steps** for a production conv1d, and names "absence of inference-time scaling" as one of
its six criticisms of prior systems (§1, p.7).

## Recurring design decisions

- **Target language.** Triton dominates because one source lowers through MLIR to NVIDIA (PTX/CUBIN), AMD
  (AMDGCN/HSACO), and MTIA (RISC-V) — cross-platform generation from a single spec is a *compiler* property
  the agent inherits, not something the agent solves. KernelEvolve's Figure 3 shows Triton passing CUDA as
  Meta's dominant kernel language (8,000+ kernels, ~60% growth) — the ecosystem reason as much as the
  technical one.
- **Artifact shape.** A standardized dual implementation — reference module + generated kernel + input
  generator — so validation and benchmarking are fully automatable and the same harness works for every
  candidate.
- **Who writes the evaluation harness.** [KernelEvolve](../sources/kernelevolve.md) makes this a
  **deterministic, non-LLM** code generator: the model writes only the kernel; the profiling harness is
  templated. This keeps measurements comparable across variants and moves compilation out of the inner loop
  (≥10 min → seconds).
- **Profiling as feedback, not just as a score.** The distinguishing move of the more mature systems is
  feeding *structured* profiler output (occupancy, stall reasons, memory throughput, per-PE utilization) back
  into the next prompt, rather than only the scalar time. KernelEvolve built **Triton MPP** partly because
  existing profilers "target human interpretation through textual reports and dashboards rather than
  structured data, forcing brittle text parsing unsuitable for automation."
- **Specialization vs. generality.** Search against a production shape distribution produces kernels that
  *lose* off-distribution (KernelEvolve reports 0.39–0.63× on out-of-distribution shapes). Every deployed
  instance therefore needs **shape-aware dispatch with fallback** to the vendor library. The search finds the
  win; a separate guard makes it safe to ship.

## Two distinct value propositions

Worth separating, because papers conflate them and they have different economics:

- **Optimization** — beat an existing, working kernel. Value scales with how much headroom the vendor library
  left, so it is *smallest* on mature stacks (KernelEvolve: 1.06–1.62× over tuned cuDNN paths on
  NVIDIA/AMD).
- **Enablement** — produce a kernel that does not exist. On MTIA v2i, operators like `sort.values_stable`,
  `_unique2`, and `unique_consecutive` have no native implementation, so PyTorch falls back to CPU with
  host-device synchronization; the generated kernel is the only on-device path. Value here is not a speedup
  ratio at all — it is whether the model can be deployed monolithically (see
  [`../topics/auto-optimization.md`](../topics/auto-optimization.md) on the 10–20 ms disaggregation tax).
  KernelEvolve's Batch Event Truncate case is the extreme point: a batched jagged-tensor kernel that "no
  batched variant existed" for, because the index arithmetic was too tedious to hand-write.

> [!inferred] The enablement framing is why an accelerator vendor deployed this first. If your hardware is
> proprietary and absent from every model's training corpus, LLM kernel generation is not a performance
> optimization — it is the cheapest available substitute for the years of library engineering that gave
> CUDA its moat. That predicts the technique diffuses fastest among ASIC and new-accelerator vendors, and
> slowest where cuBLAS/cuDNN already cover the operator set.

## Directed search vs. selection-driven search

The systems here split on a design axis that cuts across the "how long should the search run" question:
**does the next candidate come from a diagnosis, or from selection over sampled variants?**

| | Selection-driven ([KernelEvolve](../sources/kernelevolve.md), [AlphaEvolve](../sources/alphaevolve.md) / [openevolve](../code/openevolve/overview.md)) | Directed ([TPU autoresearch wiki, kernel lane](../sources/tpu-performance-autoresearch-wiki.md)) |
|---|---|---|
| What produces the next candidate | a search policy over scored variants — evolutionary population, MCTS/UCT, or greedy — with context retrieved into the prompt | a bound diagnosis (compute / bandwidth / dispatch floor read off the profile and lowered IR) plus the still-untried levers of the kernel's routed class page |
| Unit of iteration | a program in a population | one experiment = one **mechanism**; a different mechanism forces a new pre-registered page |
| Selection signal | fitness `F` (speedup, `0` on any correctness failure) | a verdict against a **pre-registered** falsification bar, calibrated to what the roofline says is reachable |
| Budget rule | steps / stall / threshold (KernelEvolve: 50 steps trivial, 300 for production conv1d) | the declared candidate plan, executed in full — *"not first-win, not a clock, not your judgment"* |
| Failures | low-fitness children don't propagate; no durable artifact | filed as pages; refuted patterns become a reusable prior layer |
| "No kernel can win here" | not expressible — the loop keeps sampling | a **first-class `refuted` verdict** backed by IR/roofline evidence |
| Scaling knob | inference-time compute (more steps, wider population) | knowledge (class-page levers, earned-rules briefs) |

Two consequences are worth carrying into any system in this family:

- **Coverage becomes checkable when levers are enumerated.** Because the TPU wiki maintains a
  `## Levers (verified)` list per kernel category, "have I covered the space?" is a **set-diff** — every
  lever is either tried with a resolving receipt, or ruled out with an argument against its *mechanism* at
  this operating point (a failed implementation route rules out the route, not the lever). A
  selection-driven loop has no equivalent notion of "covered," which is exactly why its stopping rule has
  to be a budget.
- **A negative result is evidence only if the instrument worked.** A candidate that fails the correctness
  gate refutes the *implementation*, not the operator's ceiling — so it can never license a "nothing more is
  available" conclusion. KernelEvolve encodes the same asymmetry in its fitness function (`F = 0` on any
  correctness failure, so a wrong kernel can never score), but only the directed loop has to state it
  explicitly, because only it draws conclusions from losing.

> [!inferred] These look complementary rather than competing, and the seam is visible inside both designs.
> AlphaEvolve's most production-relevant kernel win is *tuning* (tiling heuristics) inside a structure a
> human fixed; the TPU wiki's ordering discipline says the same thing from the other side — *structure
> before tiling before flags* — and it hands tile-size search to a constrained enumerative sweep once the
> algorithm and grid are settled. The division of labour that falls out: **direct the structural decision
> from a diagnosis; search the parameter interior.** No system here automates the handoff between the two.

## The proprietary-hardware problem

A base model cannot write kernels for hardware it has never seen. Two answers appear in the literature:

- **Knowledge injection (retrieval).** Write the missing architecture documentation, language extensions, and
  code samples into a knowledge base and retrieve them into context at generation time. KernelEvolve's
  `hardware/mtia/` subtree documents SFU libdevice mappings, `cb_multiplier`/`use_dual_core` compile options,
  cross-PE `direction` broadcast/reduction, `tl.pe_runtime_barrier()`, and MTIA's custom type system.
  Claimed advantage: new hardware is onboarded by writing docs, **without model retraining**. See
  [`retrieval-augmented-prompt-synthesis`](retrieval-augmented-prompt-synthesis.md).
- **RL from execution feedback.** Fine-tune on compilation success / correctness / latency rewards.
  KernelEvolve lists this as *future* work (§6) and notes its appeal for proprietary hardware: the reward is
  computed inside the vendor's walls, so the model adapts without the architecture details leaving.
  [KernelBlaster](../sources/kernelblaster.md) is a caution against reading "RL" here as necessarily
  weight-updating: its MAIC-RL never touches model weights — it borrows REINFORCE's vocabulary to describe
  rewriting a natural-language knowledge base, which mechanistically belongs under the knowledge-injection
  bullet above, not this one. A genuine weight-updating instance would be what KernelBlaster itself cites as
  "Training-Based Solutions" — Kevin-32B and CUDA-L1 — neither yet ingested here.

## In this wiki

- **Papers:** [KernelEvolve](../sources/kernelevolve.md) is the canonical instance — production-deployed,
  three vendors, 480/480 operator-platform correctness, 1.25–17× on production workloads.
  [AlphaEvolve](../sources/alphaevolve.md) does kernel auto-tuning as one of several case studies (Pallas TPU
  matmul tiling heuristics: 23% kernel speedup, 1% of Gemini's total training time; XLA IR for
  FlashAttention: 32%). [KernelBlaster](../sources/kernelblaster.md) (NVIDIA, arXiv:2602.14293) is the
  third — raw CUDA rather than Triton or Pallas, on standard NVIDIA GPUs (A6000/A100/H100/L40S), reaching
  1.43×/2.50×/1.50× geomean on KernelBench L1/L2/L3 via a Persistent CUDA Knowledge Base updated by an
  in-context (not weight-space) "RL" loop; an ablation shows removing that memory costs 1.67× slowdown. The
  [TPU autoresearch wiki](../sources/tpu-performance-autoresearch-wiki.md)'s
  **kernel lane** is the directed counterpart above — Pallas/Mosaic on TPU, one experiment per mechanism,
  pre-registered bars, an independent verifier, and `refuted` as a first-class outcome. Its published
  head-to-head is GQA attention against a hand-tuned reference's 2.48×, with three agents at 6.77× / 3.73× /
  3.51× — a single-family snapshot from a live campaign rather than a settled benchmark (see the caveat in
  [`auto-optimization`](../topics/auto-optimization.md#the-tpu-autoresearch-wikis-kernel-lane--the-directed-alternative)).
- **Topics:** [`auto-optimization`](../topics/auto-optimization.md) — the section this concept anchors.
- **Verification:** [`verification-independence`](verification-independence.md) — this domain's "free
  oracle" is what makes independence cheap here and expensive everywhere else in autoresearch.
- **Not yet ingested** (from KernelEvolve's related work): KernelBench, AutoTriton, KernelLLM, CWM, TritonRL,
  GEAK, Kevin, KernelAgent, TritorX. From KernelBlaster's related work: **Kevin-32B** and **CUDA-L1**
  (Li et al., arXiv:2507.14111) — the genuine weight-updating RL counterparts to MAIC-RL's in-context
  version; CUDA-L1 additionally pairs weight updates with its own retrieval archive, the natural next paper
  to sharpen the in-context-vs-weight-space comparison.

## See also
- [`evolutionary-algorithm-discovery`](evolutionary-algorithm-discovery.md) — the broader family: code
  candidates, LLM operator, execution-grounded selection.
- [`agentic-tree-search`](agentic-tree-search.md) — the search structure both KernelEvolve and the
  AI-Scientist lineage use, and the judge-vs-oracle difference between them.
- [`retrieval-augmented-prompt-synthesis`](retrieval-augmented-prompt-synthesis.md) — how KernelEvolve gets
  hardware facts into a model that lacks them.
