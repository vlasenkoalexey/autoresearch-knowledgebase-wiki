# Retrieval-augmented prompt synthesis

**Definition.** Retrieval-augmented prompt synthesis is the practice of **composing each iteration's prompt
at runtime** — from an analysis of what just happened plus targeted retrieval from a persistent knowledge
store — instead of filling a fixed template chosen from a small menu of operator types (`Draft`, `Debug`,
`Improve`). The prompt becomes a computed artifact, and the agent's behavior is determined by *what got
retrieved* rather than by *which operator was selected*.

Its strongest statement is [KernelEvolve](../sources/kernelevolve.md)'s **universal operator**: one
transformation function `O : S × C → S` whose entire behavioral variety comes from the context `C`.

## The argument against static operator templates

KernelEvolve's §3.1 (p.12–13), citing Toledo et al. (2025), makes a claim worth stating precisely because it
cuts against several other systems in this wiki:

> Performance bottlenecks in LLM-based code generation stem primarily from **operator design rather than
> search algorithms**.

The mechanism of the failure: a `Debug` operator carries a fixed error-focused prompt whether the fault is an
algorithmic error, a memory-access pattern, or a hardware-specific constraint; an `Improve` operator carries
a fixed performance-focused prompt whether the bottleneck is compute-bound, memory-bound, or synchronization
overhead. The paper's framing is that this "imposes cognitive constraints on the model's reasoning process,
potentially misleading the model by framing optimization problems through predefined lenses that may not
align with the actual runtime context," and that operator boundaries create "artificial boundaries in the
solution space" preventing one step from simultaneously fixing a numerical error *and* restructuring memory
access *and* exploiting a hardware feature.

## The mechanism (as KernelEvolve implements it)

A deliberately ordered two-stage pipeline (§3.2, p.13–16):

1. **Analyze first.** A *context memory sub-agent* reads the runtime artifacts of the current node — kernel
   source, execution log, correctness result, timings, and profiler metrics (instruction latency, memory
   throughput, occupancy, stalls) — and has an LLM produce a structured bottleneck diagnosis. Example from
   the paper: 30% occupancy on H100 with high shared-memory pressure → root-causes register spilling and
   bank conflicts → recommends value recomputation and warp-level access changes.
2. **Retrieve second, parameterized by the analysis.** A *deep search sub-agent* queries a hierarchical
   knowledge base — an `index.md` over `constraints/`, `guidance/`, `hardware/{nvidia,amd,mtia}/` — in two
   stages: identify relevant modules by platform / bottleneck type / optimization phase, then fetch those
   modules. A memory-bandwidth bottleneck on H100 returns
   `hardware/nvidia/optimization/{tma, shared_memory, on_device_tma}.md`.
3. **Compose.** The next prompt is assembled from four ingredients — current kernel + execution history, the
   analysis report, the retrieved documents, and hardware constraints — under a 64K–1M token budget, with
   secondary bottlenecks *deferred* to later iterations when several compete.

The ordering is the load-bearing design claim: **"effective knowledge retrieval requires runtime context to
determine retrieval targets."** Retrieval keyed on static heuristics returns generic guidance; retrieval
keyed on a fresh diagnosis returns documents about the bottleneck actually observed.

Two supporting properties:

- **Progressive specialization.** Content is organized so early iterations retrieve broad material (Triton
  basics, correctness requirements) and later ones navigate to expert content — a documented GEMM-on-H100
  trajectory walks `arch/tensor_cores.md` → `tlx/{warp_specialization, async_tensor_core_operations}.md` →
  `code_samples/hopper-gemm-ws.py`.
- **Negative memory.** The context memory keeps summaries of prior attempts, so a strategy that failed
  (increasing block size didn't help, or broke correctness) is not retried — "mirrors human debugging
  workflows where engineers track attempted fixes."

## Why it matters beyond kernels

Two consequences generalize past this domain:

**1. It is how you use a model on facts it was never trained on.** MTIA is proprietary and "largely absent
from public training corpora"; without retrieved documentation the model emits GPU-semantics Triton that
fails to compile or is silently wrong. Writing the facts down and retrieving them in-context substitutes for
fine-tuning, so a new accelerator is onboarded by authoring documentation rather than by retraining. See
[`llm-kernel-generation`](llm-kernel-generation.md).

**2. It is a context-management strategy, not just a knowledge strategy.** The paper explicitly frames
retrieval as the alternative to accumulating history in working memory, citing agentic coding systems that
"perform complex analysis over large datasets through targeted queries and incremental loading rather than
exhaustive context consumption." That is the same diagnosis and the same fix as this wiki's own
[context-pollution write-up](../sources/2026-06-05-making-karpathy-autoresearch-production-ready.md): loop
unreliability traced to context accumulating across iterations, fixed by re-deriving what each iteration
needs instead of carrying everything forward. KernelEvolve arrives at it from the opposite direction
(scaling a production search to hundreds of concurrent agents) and reaches the same architecture.

## How this compares across the wiki

The wiki's systems sit on a spectrum from *fixed template* to *fully synthesized prompt*:

- **[openevolve](../code/openevolve/overview.md)** — [`PromptSampler`](../code/openevolve/concepts/openevolve-prompt-sampler.md)
  is "the sole translation layer that re-derives evolutionary state into the natural-language prompt a
  stateless LLM needs on every call." Real synthesis, but the inputs are *evolutionary state* (parent
  program, scores, inspiration programs) drawn from
  [templates](../code/openevolve/concepts/openevolve-prompt-templates.md) — no external knowledge corpus and
  no diagnosis stage.
- **[rd-agent](../code/rd-agent/overview.md)** — Co-STEER's
  [RAG memory](../code/rd-agent/concepts/rdagent-components-coder-CoSTEER-knowledge_management.md) retrieves
  over past (task, code, feedback) triples, i.e. **the system's own history**, and RD-Agent keeps an explicit
  Research/Development operator split — exactly the multi-operator architecture KernelEvolve argues against.
  See [`research-development-loop`](research-development-loop.md).
- **[pi-autoresearch-vkf](../code/pi-autoresearch-vkf/overview.md)** — retrieves **trust-gated VKF cards**
  (verified claims with a candidate → verified → contradicted lifecycle). Closest to KernelEvolve in spirit —
  a durable corpus consulted per iteration — but the corpus is *earned* by the agent's own experiments rather
  than authored by humans, and it carries a trust model KernelEvolve's knowledge base does not.
- **[Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md)** — synthesizes per-iteration context from the
  search's own state, but **keeps** the operator menu. Its `Improve` prompt is assembled from the parent's
  deterministic experience record + a vertical ancestor trace + a horizontal sibling set ranked by
  score/gain/novelty + a global experience board; `Crossover` gets both parents plus a method-family
  complementarity cue; `Debug` retrieves prior attempts with the **same error signature**. Natural-language
  memory is generated **lazily** — only after an operator has selected its nodes — explicitly because
  summarizing eagerly "produc[es] a summary before the decision context that should shape it is known."
  Retrieval keys off the operator *and* the runtime state, rather than off a diagnosis stage.
- **[KernelEvolve](../sources/kernelevolve.md)** — the only instance with **all three**: a
  human-authored external corpus (≥100 hardware documents), a diagnosis stage that decides what to retrieve,
  and a single operator with no template menu.

> [!note] **These two papers are the wiki's clearest live disagreement, and it is narrower than it looks.**
> KernelEvolve dissolves `Draft`/`Debug`/`Improve` into one universal operator; Frontis-MA1 keeps four and
> makes them post-training targets. But both cite the *same* premise (Toledo et al., 2025 — operator design,
> not search algorithm, is the bottleneck) and both concluded that the prompt must be **computed per
> iteration from live runtime state**. KernelEvolve's stated objection is to *static prompt templates*, and
> OpenMLE-Evo's operators are not static templates. What actually separates them is whether the move's name
> is a useful retrieval key — plus one consequence neither paper states: a universal operator has no
> per-operator training target, so it is a natural fit for wrapping a **frozen** model you don't own, and a
> poor fit for the meta-evolution loop Frontis-MA1 runs. See
> [`program-evolution-operators`](program-evolution-operators.md) for the full treatment and what evidence
> each side actually has.

> [!inferred] The distinction worth carrying: openevolve, rd-agent, and pi-autoresearch-vkf all retrieve
> **what the system has learned**; KernelEvolve additionally retrieves **what the system was told** — curated
> domain expertise the agent could never derive from its own trials, because no amount of trial-and-error
> tells you that `tl.extra.libdevice.gelu` maps to an SFU lookup table. Both kinds of memory are needed, and
> only one of them can be bootstrapped by the loop itself. That asymmetry is an argument for hand-authored
> knowledge bases surviving alongside self-accumulating ones, not being replaced by them — and it is the
> premise this whole wiki runs on.

## See also
- [`llm-kernel-generation`](llm-kernel-generation.md) — the domain where this was demonstrated.
- [`closed-loop-experiment-design`](closed-loop-experiment-design.md) — the feedback state each system
  retrieves from.
- [`../topics/wiki-driven-autoresearch-loop.md`](../topics/wiki-driven-autoresearch-loop.md) — context
  pollution and the re-injection fix, the same problem from the other direction.

<!-- connect:auto:begin -->
## In this wiki's repos
Grounded implementations of **retrieval-augmented-prompt-synthesis** across the ingested repos (generated by `wikify connect` — do not hand-edit inside this block):

- [openrsi](../code/openrsi/concepts/OpenMLE-ERL-RL-airaevo_experience.md) — airaevo_experience.py — the original-AIRA-Evo selection/memory adapter for RL rollouts
<!-- connect:auto:end -->
