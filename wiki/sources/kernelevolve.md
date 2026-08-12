# KernelEvolve: Scaling Agentic Kernel Coding for Heterogeneous AI Accelerators at Meta

**Source:** KernelEvolve Team, Meta Platforms (project leads Gang Liao, Gaoxiang Liu; correspondence also
Carole-Jean Wu), "KernelEvolve: Scaling Agentic Kernel Coding for Heterogeneous AI Accelerators at Meta,"
arXiv:2512.23236 — this wiki ingested **v4, dated 6 Jul 2026** (technical-report date on p.1: July 8, 2026).
Appears at **ISCA 2026** (53rd International Symposium on Computer Architecture). Companion engineering-blog
post: [engineering.fb.com, 2026-04-02](https://engineering.fb.com/2026/04/02/developer-tools/kernelevolve-how-metas-ranking-engineer-agent-optimizes-ai-infrastructure/).
Raw source: [`../../raw/papers/kernelevolve.pdf`](../../raw/papers/kernelevolve.pdf).

> [!note] **This is the first paper in this wiki whose center of mass is [auto-optimization](../topics/auto-optimization.md)
> rather than [autoresearch](../topics/autoresearch.md).** [AlphaEvolve](alphaevolve.md) straddles the two
> (open math problems *and* Google's compute stack); KernelEvolve does only the optimization half — it never
> generates a scientific hypothesis, writes a paper, or evaluates novelty. What it contributes to the
> autoresearch side of this wiki is the *harness*: an agentic tree search whose fitness function is measured
> wall-clock speedup on real silicon, run continuously in production. It de-stubs
> [`topics/auto-optimization.md`](../topics/auto-optimization.md).

## What this paper is

A **deployment experience report**, not a benchmark paper. KernelEvolve is an agentic framework that takes a
kernel specification and autonomously generates, compiles, validates, profiles, and optimizes **Triton**
kernels across NVIDIA GPUs, AMD GPUs, and Meta's proprietary **MTIA** accelerators. The authors claim it is
"the first LLM-based kernel coding system deployed at-scale for business-critical recommendation model
inference" (§7, p.40), operating continuously in Meta's production infrastructure for hundreds of models
(§1 contributions, p.8).

The paper's own three-axis contribution claim (§7, p.40): **heterogeneous hardware at scale** (one system
targeting three vendors including a proprietary ASIC), **production operator diversity** (200+ ads
preprocessing operators, not canonical GEMM benchmarks), and **deployment-integrated optimization**
(continuous validation, multi-level profiling, serving-infrastructure compatibility).

## The problem: a "curse of dimensionality" that is really a deployment blocker

§1.1 (p.3–7) frames kernel work at Meta as a combinatorial explosion across three axes:

1. **Hardware heterogeneity** — NVIDIA (multi-MB L2), AMD (Infinity Cache), MTIA (custom on-chip SRAM), each
   with incompatible programming models (CUDA thread-blocks, Triton tiles, ROCm/HIP, CuTe layout algebra,
   MTIA's C++ DSL, TileLang/TLX/Gluon), plus *within-vendor* generational discontinuities (Ampere→Hopper
   introduced TMA, 128-thread warp-groups/WGMMA, mbarrier producer–consumer pipelines). Each
   platform-specific implementation is quoted at **2–8 weeks of expert effort**, against **12–18-month**
   hardware refresh cycles that invalidate prior tuning (p.4).
2. **Model diversity** — a multi-stage ads funnel (≥500 early-stage models at 0.01–0.1 GFLOPS/request; ≥1000
   late-stage at 0.2–2 GFLOPS/request; Transformer-based sequence models at ~80 GFLOPS/request, a 10–100×
   jump) — Table 1, p.5.
3. **Kernel diversity beyond GEMM** — ads ranking runs **200+ data-preprocessing operators** (bucketization,
   n-gram hashing, top-k truncation, cryptographic hashing with modulo reduction, jagged-tensor ops) with
   low arithmetic intensity, irregular access, and data-dependent control flow (p.5).

The load-bearing argument — and the reason this is a systems paper rather than a performance paper — is that
**missing preprocessing kernels are a binary deployment constraint, not an incremental performance loss**
(p.6). Without a native accelerator implementation, the model cannot be deployed monolithically; it must be
split across a CPU preprocessing tier and an accelerator tier. Table 2 (p.5) prices that tax on a real MTIA
deployment: monolithic serving hits **P99 = 61 ms**; disaggregated serving hits **P99 = 97 ms**, of which
**10–20 ms is pure network overhead** (δ = α − β − γ) buying nothing — a 25% degradation against a sub-100 ms
budget. So "generate a kernel that merely *works*" has larger system value than "make an existing kernel
faster."

A second motivating datum: Figure 3 (p.7) shows **Triton has overtaken CUDA as the dominant kernel language
at Meta** — over 8,000 Triton kernels growing at ~60%, against a stagnant legacy CUDA codebase, with CuTe,
TLX, and Helion each under 600. This is why KernelEvolve targets Triton (plus Triton-TLX): one source
language, three backends via MLIR lowering to PTX/CUBIN, AMDGCN/HSACO, and RISC-V (Figure 2, p.6).

## The system

### Kernel optimization as graph-based search (§3.1, p.12)

KernelEvolve maintains a search graph `G_t = (V_t, E_t)`; nodes are kernel artifacts, edges are
transformations, the root is the baseline/spec. Each iteration **selects** nodes, **applies** a
transformation, and **scores** the result. The whole system is specified as a four-tuple `(F, π_sel, O, τ)`:

- **Fitness `F`** = `t_pytorch / t_triton` — measured speedup over the `torch.compile`d PyTorch reference.
  Kernels failing numerical validation or hitting compilation/runtime errors get **`F(v) = 0`**. Correctness
  is a hard constraint folded into the objective, not a separate gate.
- **Selection policy `π_sel`** — pluggable: **greedy** (single best node), **MCTS** with UCT, or
  **evolutionary algorithms** maintaining a diverse population for crossover/mutation.
- **Universal operator `O : S × C → S`** — see below.
- **Termination `τ`** — wall-clock/artifact budget exhausted, progress stalled, or a fitness threshold met.

The synthesized prompt goes to either **external** LLM backends (**Claude 4.5, GPT-5**) or **internal** ones
(Meta's **CWM** and **Llama**, served on Twine) — the architecture is deliberately backend-agnostic, and the
paper attributes no result to a specific model (§3, p.11; Figure 5, p.10).

### The universal operator — the paper's sharpest design claim (§3.1, p.12–13)

Citing Toledo et al. (2025b), the paper asserts that **the bottleneck in LLM-based code generation is
operator design, not the search algorithm**, and draws the consequence: conventional frameworks with
multiple specialized operators (`Draft`, `Debug`, `Improve`) bind each to a *static prompt template* that
cannot adapt to runtime context. A `Debug` operator uses the same error-focused prompt whether the fault is
algorithmic, a memory-access pattern, or a hardware constraint; an `Improve` operator uses a
performance-focused prompt regardless of whether the bottleneck is compute-bound, memory-bound, or
synchronization. The paper's claim is that this "imposes cognitive constraints on the model's reasoning
process… framing optimization problems through predefined lenses that may not align with the actual runtime
context," creating "artificial boundaries in the solution space."

KernelEvolve therefore uses **exactly one operator** whose behavior is determined entirely by
retrieval-augmented dynamic prompt synthesis, letting a single generation step simultaneously fix numerical
errors, restructure memory access, and exploit hardware features. Figure 6 (p.13) traces one such
invocation: an agent iteratively calling `read_file` / `write_to_file` / `replace_in_file` / `lint` over 20
steps to produce a lint-free autotuned Swish kernel.

### Two sub-agents and a persistent knowledge base (§3.2, p.13–18)

The prompt is assembled by a two-stage pipeline, explicitly modeled on retrieval-style agentic coding
(the paper cites Anthropic's Claude Code and its context-engineering post, p.13):

- **Context memory sub-agent** — analyzes the *runtime* artifacts of a node (kernel source, execution logs,
  correctness results, timings, occupancy/throughput/stall metrics), invokes an LLM to produce a structured
  bottleneck diagnosis, and composes the next prompt from four ingredients: current kernel + execution
  history, the analysis report, retrieved knowledge-base content, and hardware constraints — within a
  **64K–1M token budget** depending on backend (p.15). It also maintains summaries of what has already been
  tried so failed strategies aren't re-attempted.
- **Deep search sub-agent** — performs *targeted* retrieval from a persistent knowledge base laid out as a
  **hierarchical file system** with an `index.md` at the root, partitioned into `constraints/` (anti-cheating
  rules: no cross-platform abstractions, no external library wrappers, no direct CUDA API calls — so the
  agent cannot "win" by calling cuBLAS), `guidance/` (platform-agnostic debugging, autotuning, fusion, Triton
  idioms), and `hardware/{nvidia,amd,mtia}/` (**15–40 documents per platform, ≥100 total**). Retrieval is
  two-stage: query the index for relevant modules by platform/bottleneck/phase, then fetch the modules
  (p.14).

The ordering is the point: **the context memory sub-agent runs first and parameterizes the deep search
sub-agent**, because "effective knowledge retrieval requires runtime context to determine retrieval targets"
(p.14). A 30%-occupancy H100 profile with shared-memory pressure produces a diagnosis (register spilling,
bank conflicts) that in turn selects which documents to load — rather than loading generic guidance up front.

**Progressive specialization** (p.14–15): a GEMM-on-H100 trajectory walks
`hardware/nvidia/arch/tensor_cores.md` → `hardware/nvidia/tlx/{overview, warp_specialization,
async_tensor_core_operations}.md` → `code_samples/{hopper-gemm-pipelined, hopper-gemm-ws}.py`, i.e. from
novice to expert-level content as the search deepens.

### MTIA knowledge injection — the paper's most transferable finding (§3.2.3, p.16–18)

MTIA is "absent from public training corpora," so a pretrained LLM asked for an MTIA kernel emits standard
GPU-semantics Triton that fails to compile or is functionally wrong. KernelEvolve's answer is to write the
missing documentation into the knowledge base and let retrieval teach the model in-context. The documented
extension surface is concrete: libdevice APIs mapping `tl.extra.libdevice.gelu(x)` to a Specialized Function
Unit lookup-table query (faster, potentially less accurate) rather than a math approximation; compile-time
options `cb_multiplier` (circular-buffer allocation) and `use_dual_core` (DMAs on core A while core B runs
vector instructions), both explorable via `@triton.autotune`; compute helpers
(`unary_elemwise_compute` with 30+ ops, `binary_elemwise_compute`, `binary_elemwise_const_compute`); custom
types (`TensorView`, `CoreID`, `ExecutionGrid`); and multi-PE primitives absent from standard Triton —
cross-PE broadcast/reduction via a `direction` attribute ("down"/"right") on `tl.load`/`tl.store` with a
complementary `tl.consume()`, `tl.pe_runtime_barrier()`, and `tl.copy()`. Figure 7 (p.17) shows the target:
an 8×8 PE array, each PE with dual RISC-V cores plus MLU/DPE/RE/SE/CP fixed-function units.

The generalization the authors draw (p.18): "as new hardware platforms enter production, corresponding
documentation injected into the knowledge base enables immediate LLM-based kernel generation **without model
retraining**."

### Persistence: the search graph lives in a database (§3.2.2, p.15)

Nodes persist to a **relational metadata store** (`id`, `pid`, `score`, `is_buggy`, `path_ref`) pointing at
an **object store** holding `kernel_n.py`, profiling results, and an LLM-written `overview.md` per node. Four
capabilities follow, and they are the operationally interesting part of the paper:

1. **Distributed concurrent exploration** — dozens-to-hundreds of agents expand different nodes
   simultaneously under database transaction isolation; an in-memory graph would not survive the scale.
2. **Complex contextual queries** — SQL (recursive CTEs) reconstructs graph views without materializing the
   tree: sibling outcomes, strategies from high-performing ancestors, global best.
3. **Cross-session knowledge reuse** — a new kernel request is matched against history by operator type,
   input shapes, and platform, and search is *initialized from the best prior implementation* rather than
   from scratch. The worked example (p.15): a new GEMM variant for attention on AMD MI350 matches 15
   historical GEMM kernels, three above 1.5× via TLX warp specialization; the best is retrieved with its
   optimization report and search starts from there.
4. **Fault tolerance / checkpointing** — each node insertion *is* a checkpoint; a crashed multi-hour campaign
   resumes from the last iteration. The paper lists "no checkpointing support" as one of six named
   deficiencies in prior systems (p.7).

### Evaluation infrastructure (§3.4, p.18–23)

- **Standardized dual-implementation artifact** — every generated file contains a `PytorchModel` (correctness
  ground truth), a `@triton.jit` kernel plus wrapper plus `TritonModel`, and `get_inputs()` producing test
  cases across scales. Training operators must also supply matching `backward()` methods (footnote, p.19).
  `nn.Module` shape is deliberate: it composes with `torch.compile`.
- **Non-LLM evaluation code generation** — a *deterministic* generator turns each artifact into
  tool-specific harnesses (TritonBench, Torch Profiler, NCU, Proton). The separation buys three things
  (p.21): compilation happens once at interpreter deploy time rather than per evaluation (**≥10 minutes → seconds**),
  evaluation code is identical across variants so profiling is comparable, and profiler APIs can change
  without touching generation prompts.
- **AI hardware interpreters** — three Bento (Jupyter) environments bundling per-platform toolchains and
  runtimes, rebuilt and redeployed daily by Meta's **Conveyor** CD system so the agent always targets current
  dependencies (Figure 8, p.20).
- **Triton MPP (Multi-Pass Profiler)** — Meta's federated profiling framework, composing MLIR-level
  instrumentation, profiling passes, and trace synthesis as job-graph tasks. The motivating problem is that
  profilers "target human interpretation through textual reports and dashboards rather than structured data,
  forcing brittle text parsing unsuitable for automation" (p.21). MPP also does *minimally invasive*
  probing — isolating single instructions in specific iterations rather than inserting waits that perturb
  the async overlap being measured.
- **Agentic debugging via JIT introspection** (§3.4.5, p.22) — MTIA-Triton can emit the C++ IR before RISC-V
  codegen (`emit_cxx=True`, then `compiled_kernel.asm["cpp"]`); the agent edits that C++ and re-launches it
  through `replay_cpp(...)`, skipping full recompilation. Hypothesis validation drops "from minutes to
  seconds."
- **FaaS-based evaluation** (§3.4.6, p.22–23) — generation is CPU-bound, evaluation needs accelerators, so
  evaluation is dispatched to Meta's FaaS platform (Tasklet resource model extended from CPU/RAM to GPU).
  Without this, agents serialize through the 8 GPUs / 24 MTIA devices on a host, **each occupying a device
  for 8–12 minutes that is mostly idle generation time**.

## Results

### Correctness first (§4, p.23)

- **480/480 operator-platform configurations correct** — 160 curated ATen operators (elementwise,
  transcendental, reductions, activations) × {NVIDIA H100, AMD MI350, MTIA v3}, validated with
  `torch.allclose` in TritonBench against `torch.compile`d references.
- **KernelBench: 100% pass rate across all three levels** (single operators / fused patterns / full model
  blocks) — the abstract puts this at **all 250 problems**. Note this is a *correctness* pass rate; the paper
  does not report KernelBench speedup statistics.

Figure 10 (p.24) shows 50-step trajectories for six ATen ops, split into a **draft phase (steps 0–10:
independent sampling, no feedback)** and a **tree-expansion phase (steps 10–50: each node inherits ancestor
profiling/compile/correctness feedback)**. The honest reporting here is worth noting: `torch.cos` improves
2.8→3.05×, `aten.add.Tensor` improves 0.64→0.70× (**still below 1× — the generated kernel loses to the
baseline**), and `torch.amax`/`torch.div` sit flat at ~1.0×. Only **four of six** exceed 1.0×. The authors
say plainly that these primitives exist to validate correctness, not to demonstrate headroom.

### Production case studies (§5, p.24–38)

Headline: **1.25–17× over PyTorch baselines** (Figure 4, p.8), across Llama-3.1-8B attention (4.6×) and
SDPA+MLP (3.3×), convolutional transformers, data preprocessing (MapId 4.1×, MBDT 9.25×, Batch Event
Truncate 9.8×), ranking fusion kernels (WuKong Optimized FM 4.0×, InterFormer PFFN 2.5×), MTIA training
(RMSNorm 2D backward **17×** — the top-line number), and retrieval (Sparse Inverted Index 1.25×).

**conv1d in the Convolutional Transformer (§5.1, p.24–26).** On the production shape
(B×C_in×C_out×L = 2048×96×96×200) in FP16: **2.30× over `torch.conv1d`, 1.62× over the strong `conv2d` +
`channels_last` + cuDNN workaround**. The mechanism is legible from the trace (Table 4, p.26): PyTorch conv1d
launches five kernels (two NCHW↔NHWC layout conversions, cuDNN implicit GEMM, output conversion, bias
fusion); the conv2d workaround launches four; **KernelEvolve launches two** — a weight-packing kernel and a
fused GEMM-style convolution operating directly on the native 1D layout. cuDNN still wins on the convolution
proper; KernelEvolve wins end-to-end by deleting the layout traffic. Complementary discovered optimizations:
>20 autotune configs, a 3D grid parallelizing grouped-convolution channels, double buffering, and
differentiated cache modifiers (`.ca` for streaming activations, `.cg` for reused weights). Figure 12 (p.27)
visualizes the **300-step** search: draft-phase fitness ~2000 climbing through 4000, 5000, converging at
6889.

**Specialization is explicit and admitted.** Table 3 (p.25) reports out-of-distribution shapes where the
same kernel **loses** — 0.63× vs conv1d and 0.49× vs conv2d at 64×768×768×1024 (FP16), 0.48×/0.39× in FP32.
The system's answer is **shape-aware dispatch with fallback to vendor libraries** when a generated kernel
underperforms (§5.2, p.28) — the same pattern recurs for Optimized FM (fall back to unfused PyTorch when
N > 64) and MapId (runtime dispatch on input dimensions). *Deploying the search's output safely requires a
guard the search itself doesn't provide.*

**Cross-platform (§5.2, Figure 13, p.28).** The same conv1d spec, five platforms, production shape, FP16 —
vs. the conv1d baseline: 1.75× (MI300), 1.77× (A100), 2.30× (H100), ~2.6× (MI350), **6.54× (MTIA v3)**; vs.
the tuned conv2d baseline: 1.25× (MI300), 1.06× (MI350), 1.35× (A100), 1.62× (H100), 4.71× (MTIA v3). The
gradient is the finding: gains are smallest where vendor libraries are most mature (cuDNN on NVIDIA) and
largest on the proprietary accelerator with the thinnest library ecosystem.

**Fusion in ranking models (§5.3, p.29–31).** WuKong's Optimized FM computes `X·(XᵀY)` (the low-rank
reassociation that drops O(N²D) to O(NKD)); `torch.compile` emits two `extern_kernels.bmm` calls with an HBM
round-trip between them, while KernelEvolve fuses both matmuls into one kernel keeping `XᵀY` in SRAM —
~2× less memory traffic, **3.6–3.9× speedup at N=24**, degrading toward 1× as N grows past 64 and tile
management overhead swamps the on-chip win. InterFormer's PFFN (bmm → GELU → RMSNorm → bmm → RMSNorm)
collapses PyTorch's three memory passes into one single-pass kernel: **2.0–2.6× at small batch**, settling
to 1.2–1.4× at large batch as launch-overhead amortization erodes the fusion advantage, with a documented
non-monotonic dip at D≈200 where tiles brush SRAM capacity and partially spill.

**MTIA preprocessing — enablement, not just speed (§5.4, p.31–36).** Table 5 (p.32) lists ATen operators
*missing* on MTIA: on v2i, MapId needs `clamp.out`, `gather.out`, `sort.values_stable`, `all.all_out`,
`_unique2`; MBDT needs `all.all_out`, `unique_consecutive` (v3 needs strictly fewer). Without generated
kernels PyTorch falls back to CPU with host-device synchronization. MapId fuses bucketize+clamp+gather+where
into one launch (4× less global memory traffic) with a fixed 20-iteration binary search — a `tl.constexpr`
bound supporting 2²⁰-entry tables that the compiler unrolls into branchless predicated code. Results:
**up to 4.07× on MTIA v2i, 1.05–1.36× on v3**; MBDT hits **2.94–9.25× on v2i, 2.31–3.09× on v3**. MBDT's
generated kernel notably replaces binary search with **SIMD vectorized counting** — O(n) beats O(log n) for
3–10 element border arrays because it is branch-free — and avoids `tl.where` inside loops, a construct that
fails MTIA compilation.

**Batch Event Truncate (§5.5, p.37–38).** Truncating nested jagged event sequences across features required
"coordinated index arithmetic across three nested levels" that nobody had batched by hand — *"no batched
variant existed due to the complexity."* KernelEvolve produced one: **9.8× at 9 features and 14.5× at 32
features** when no truncation is needed (vectorized comparison vs. PyTorch's per-element loop), 1.4–2.0× when
truncation happens, **2× end-to-end in production**. This is the paper's strongest qualitative claim — not a
faster version of an existing kernel, but a kernel that did not exist.

## Where this differs from prior LLM-kernel work (§1, p.6–7; §7, p.39–40)

The paper's six-point indictment of prior systems (KernelBench, AutoTriton, KernelLLM, CWM, TritonRL, GEAK,
Kevin, KernelAgent, TritorX) is a useful checklist for reading any kernel-agent paper: (1) narrow
optimization scope, no end-to-end lifecycle; (2) synthetic evaluation on canonical operators with static
shapes, not production workloads with dynamic batching and jagged tensors; (3) single-platform (NVIDIA)
focus; (4) limited agent capability — no multi-level correctness verification, hierarchical profiling
feedback, or persistent knowledge base; (5) **no inference-time scaling** (no search running hundreds-to-
thousands of steps per kernel); (6) **no checkpointing** — restart from scratch on failure.

> [!inferred] Points 5 and 6 are the ones this wiki should carry forward. They are not about kernels at all;
> they are the same two properties that separate the harnesses in
> [`topics/wiki-driven-autoresearch-loop.md`](../topics/wiki-driven-autoresearch-loop.md) from one-shot agent
> demos — sustained search under a budget, and durable state that survives the process. KernelEvolve's
> version of "durable state" (a SQL-queryable search graph reused *across sessions and operators*) is more
> aggressive than anything else currently in this wiki: [openevolve](../code/openevolve/overview.md)'s
> program database and [ai-scientist-v2](../code/ai-scientist-v2/overview.md)'s Journal are both scoped to a
> single run.

## Future directions the authors name (§6, p.38–39)

Model-level rather than operator-level optimization (cross-layer fusion, global allocation, co-optimizing
model structure with kernel implementation); **deeper codegen** below Triton (MLIR dialects, PTX/SASS —
"positioning LLM agents as general-purpose compilers rather than domain-specific tools"); **massively
parallel search** ("infinite-width," relaxing consistency to evaluate thousands of candidates at once, with
inference-time scaling laws implying kernel quality improves predictably with compute); **RL from execution
feedback** to adapt generic models to proprietary hardware without exposing its details; end-to-end
integration with AOT Inductor and CI; and **sustainability accounting** — token consumption per kernel,
prompt cost, carbon footprint across the search.

## Reading cautions — internal inconsistencies in v4

Grounding discipline for anyone citing numbers from this preprint. These are small but real, and a reader
who quotes the wrong one will be wrong:

- **The headline range is stated four different ways**: "up to 17 times" (abstract, p.1), "1.2 to 17 times"
  (contributions, p.8 and §5, p.24), "1.25-17×" (Figure 4 caption, p.8, and conclusion, p.40). This wiki uses
  **1.25–17×**.
- **conv1d on AMD MI350**: §5.2 body text says 2.54×, the Figure 13 data label says 2.64×. The same figure's
  caption says "up to 6.22× speedup" while both the body text and the plotted value say **6.54×** for MTIA v3.
- **MTIA generation labels are transposed in §5.4**: the MapId analysis compares v3 against "v1" (p.33) when
  Table 7 has no v1, and then attributes v3's smaller gains to "stronger PyTorch baselines **on v2i** due to
  improved native operator coverage" — but Table 5 (p.32) shows *v3* has the better coverage. §5.4.2 repeats
  the same swap ("v2i has higher native operator coverage"). The intended claim in both places is clearly
  that **v3's better native coverage yields a stronger baseline and therefore smaller speedups**.
- **Table 8 (p.38), row 1**: PyTorch 0.148 ms vs. Triton 0.313 ms is reported as "1.0×"; the arithmetic gives
  **0.47×** — a regression, and the paper's own text mentions no single-feature regression.
- **Two different fitness definitions**: §3.1 (p.12) defines `F = t_pytorch/t_triton` (speedup), but Figure 12
  (p.27) says "the fitness score equals 1/latency" and plots values in the thousands. Both are
  monotone-in-latency, so the search is unaffected — but they are not the same quantity, and the ~6889
  convergence figure is not a speedup.
- **Figure 4's "Conv1d 6.54× / Conv2d 4.71×" bars are not two kernels.** Both values reappear in Figure 13
  (p.28) as the *same generated conv1d kernel* on MTIA v3, measured against the two different PyTorch
  baselines (`conv1d` and the `conv2d` + `channels_last` + cuDNN workaround). Read as two separate operators
  — as secondary coverage of this paper has done — they overstate the breadth of the result.
- **Naming residue**: several artifacts still carry the system's internal name **AlphaKernel** — the workspace
  path in Figure 6 (`/tmp/alpha_kernel_workspace_…`), the interpreter names in Figure 8/9
  (`alpha_kernel_*_interpreter`), and a stale duplicated §3.4.2 block on p.21 that reads "AlphaKernel
  establishes dedicated interpreter environments." The body text uses `meta_kernel_*_interpreter`. Same
  system; useful to know when searching.

## Relation to this wiki's other systems

**vs. [AlphaEvolve](alphaevolve.md).** Both are LLM-driven search over code graded by real execution, and
both landed production infrastructure wins. Three real differences. (a) **What varies across candidates**:
AlphaEvolve evolves a *population* through an explicit MAP-elites/island database and treats evolution as
*the* architecture; KernelEvolve treats the evolutionary algorithm as **one interchangeable setting of
`π_sel`** alongside greedy and MCTS, and never reports which policy produced which result. (b) **Where the
knowledge comes from**: AlphaEvolve's prompt carries prior programs, scores, and problem context;
KernelEvolve adds a curated, hand-authored **hardware knowledge base** whose entire purpose is to supply
facts the base model cannot have — this is what makes a proprietary, undocumented accelerator tractable, and
it has no AlphaEvolve analogue. (c) **Breadth vs. depth**: AlphaEvolve spans open mathematics through TPU
circuits; KernelEvolve does one task on three vendors, continuously, in production.

> [!warning] **A claim about AlphaEvolve worth flagging.** KernelEvolve's related work (§7, p.39) places
> AlphaEvolve among systems that "target single hardware platforms with synthetic workloads, lacking
> heterogeneous hardware support, production operator coverage, and deployment infrastructure integration,"
> describing it as optimizing "select stages of TPU/GPU kernels." That characterization is only partly fair
> on this wiki's own reading of [`sources/alphaevolve.md`](alphaevolve.md): AlphaEvolve's Pallas kernel and
> XLA-IR results were measured on real TPUs against production Gemini training (23% kernel speedup, 1% of
> total training time) and its Borg scheduling heuristic was deployed fleet-wide — that is production
> deployment, not synthetic benchmarking. The defensible narrower claim is the one about **heterogeneity**:
> AlphaEvolve's compute-stack case studies are all Google-internal and TPU/XLA-centric, whereas KernelEvolve
> generates from one spec across three vendors including an ASIC absent from any training corpus.

**vs. [The AI Scientist-v2](ai-scientist-v2.md).** Both run agentic tree search over generated code with
buggy/non-buggy node status — KernelEvolve cites AIDE (Jiang et al. 2025), the same lineage. The decisive
difference is **who judges**. AI Scientist-v2 marks a node buggy on an *LLM* verdict over the run plus a
*VLM* verdict over the plots; KernelEvolve marks a node buggy on `torch.allclose` against a PyTorch
reference and scores it by measured wall-clock time. There is no judge to fool, which is exactly why it can
run 300 steps in production and be trusted to ship the winner. See
[`concepts/agentic-tree-search.md`](../concepts/agentic-tree-search.md).

**vs. [RD-Agent](rd-agent.md).** RD-Agent's explicit Research→Development split has no counterpart here —
that is the whole content of the universal-operator argument, which says merging the phases into one
context-adaptive operator is *better*, not merely simpler. See
[`concepts/research-development-loop.md`](../concepts/research-development-loop.md).

**vs. the TPU-performance sibling wiki.** [`sources/tpu-performance-autoresearch-wiki.md`](tpu-performance-autoresearch-wiki.md)
and the [blog series](2026-06-26-making-tpu-auto-optimization-work-with-other-agents.md) attack the adjacent
problem (model-level TPU performance, agent-driven, wiki-grounded). KernelEvolve is the industrial-scale
version of the same bet — with two mechanisms that wiki lacks: a **curated hardware knowledge base as the
retrieval target** and **cross-session reuse of prior optimization campaigns**. Its context-memory sub-agent
is also a direct answer to the context-pollution diagnosis in
[`sources/2026-06-05-making-karpathy-autoresearch-production-ready.md`](2026-06-05-making-karpathy-autoresearch-production-ready.md):
load per-iteration context by retrieval rather than accumulating it.

## Open thread

The paper's cross-session reuse cites a companion the wiki does not yet have —
**"Experience Graphs: The Data Foundation for Self-Improving Agents"** (Liao et al., 2026,
[arXiv:2606.29823](https://arxiv.org/abs/2606.29823)) — as the basis for initializing search from historical
solutions. If durable cross-run agent memory is the thread being pulled (see
[`concepts/closed-loop-experiment-design.md`](../concepts/closed-loop-experiment-design.md), where
`pi-autoresearch-vkf`'s VKF card store is currently the wiki's only persistent-memory instance), that is the
next paper to ingest.
