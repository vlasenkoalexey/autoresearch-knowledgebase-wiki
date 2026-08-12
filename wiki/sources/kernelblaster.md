---
title: "KernelBlaster: Continual Cross-Task CUDA Optimization via Memory-Augmented In-Context Reinforcement Learning"
type: source
authors: Kris Shengjun Dong (NVIDIA / UC Berkeley), Sahil Modi, Dima Nikiforov, Sana Damani, Edward Lin, Siva Kumar Sastry Hari, Christos Kozyrakis (NVIDIA)
arxiv: 2602.14293
venue: "arXiv preprint, 2026-02"
source: ../../raw/papers/kernelblaster.pdf
updated: 2026-08-06
---
# KernelBlaster — summary

## What it is

KernelBlaster is an NVIDIA agentic system (most of the work done by Kris Shengjun Dong during a 2025 summer
internship) that optimizes **CUDA** kernels — not Triton — across mainstream, well-documented NVIDIA GPU
generations (A6000, A100, H100, L40S), starting from an already-functional CUDA implementation and
iteratively rewriting it under NCU-profiling feedback (p.1, Table 2 p.9). Its headline claim is a
**Memory-Augmented In-context Reinforcement Learning (MAIC-RL)** framework built around a **Persistent CUDA
Knowledge Base**, motivated by the observation that prior agentic CUDA systems "have limited ability to
aggregate knowledge from prior exploration" and re-derive the same strategies from scratch on every new
kernel (p.1, §2 p.3–4). Reported results: geometric-mean speedups over the PyTorch baseline (best of Eager
and `torch.compile`) of **1.43× (Level 1), 2.50× (Level 2), 1.50× (Level 3)** on KernelBench (p.1 abstract).
The paper is explicitly framed against two adjacent families this wiki already covers — training-based RL
(Kevin-32B, CUDA-L1), and memory-augmented retrieval (AI CUDA Engineer, and **KernelEvolve**, cited directly,
p.4) — and against evolutionary program-database methods (**AlphaEvolve**, OpenEvolve, CodeEvolve, cited
directly, p.4).

## The mechanism: what the Knowledge Base stores, and what "RL" means here

**Storage.** The Persistent CUDA Knowledge Base holds entries of the form `⟨state, ⟨optimization, score⟩⟩`
(p.5). A **state** is a performance *signature* — a bottleneck classification such as
`memory_bandwidth_saturated`, `compute_throughput_saturated`, or a hybrid — not a kernel identity or an
operator type. Figure 4 (p.5) shows the taxonomy is hierarchical: `Memory Limited States` (latency-bound,
bandwidth-bound, bank-conflict), `Compute Bound States` (throughput-saturated), and `Hybrid States`
(compute/memory-imbalanced); each leaf state carries a table of optimization techniques with observed
multipliers (`Opt 1: 1.2x`, `Opt 2: 0.6x`, …) plus a `?x` slot for untried candidates. Figure 5 (p.6) shows
one entry's actual JSON shape: a `technique` string, a `primary_bottleneck`, and `secondary_characteristics`
strings (e.g. "Memory throughput >80%, Bandwidth utilization high"). The whole database is reported at
**~50 KB** after training across KernelBench Levels 1–2 on an A6000 (§5, p.11) — several orders of magnitude
smaller than a program archive that stores full kernel source per candidate.

**Retrieval and use.** A pipeline of five roles (p.5–6): an LLM-powered **State Extractor** derives the
signature from the NCU report's "Details" section for the current kernel; a **State Matcher** compares it
against documented bottlenecks to decide known-vs-discovered state; if known, an **Optimization Selector**
retrieves the state's candidate `⟨optimization, score⟩` pairs and performs a **weighted random search**
over predicted gain to pick the top-*k* — explicitly *not* greedy, "to ensure that the agent does not always
select the best past performer and explores new optimizations" (p.6); a **Lowering Agent** implements and
validates the choice; a **Policy Evaluation** module scores the result and feeds the update below.

**Is MAIC-RL weight-updating RL?** No — and the paper is unusually explicit about this, so this wiki can
state it with high confidence. Table 1 (p.8) gives the mapping directly: the RL formalism's
**parameters `θ`** are defined as "the natural language context (the Knowledge Base) that guides the LLM,"
and the **gradient update** is "an LLM rewrite[ing] the context document (θ) based on the summary to favor
better strategies." The base LLM (GPT-4.1 / GPT-5.0, Table 2) is never fine-tuned; "all adaptation happens in
the forward pass by reasoning over the provided history" (p.4). Mechanically, three LLM-agent roles
approximate one REINFORCE-style policy-gradient step (Algorithm 2 vs. the literal REINFORCE, Algorithm 1,
p.7): `PolicyEvaluation` compares achieved vs. expected performance across a replay buffer and computes a
discrepancy `g_k`; `PerfGapAnalysis` reasons in natural language about *why* the prediction was wrong;
`ParameterUpdate` rewrites the Knowledge Base entries (`θ_k → θ_{k+1}`) to reflect the correction. The
reward `r_t` is "a function of the discrepancy between predicted performance and actual performance… measured
from running the final generated code on the GPU" (Table 1, p.8) plus low-level NCU breakdowns. So MAIC-RL
borrows RL's *vocabulary* (state/action/reward/policy, an explicit REINFORCE analogy) and TextGrad's textual
gradient framing (Yao et al. 2024, cited p.4) to describe an update rule, but the artifact being mutated is a
natural-language memory document, not a weight tensor — mechanistically this is **retrieval-augmented
generation over a self-written, self-correcting knowledge base**, not gradient-based RL.

## Results

**KernelBench, geometric-mean speedup vs. PyTorch (best of Eager/`torch.compile`)** — headline: **1.43× L1,
2.50× L2, 1.50× L3** (abstract, p.1). Table 3 (p.9) breaks this out per GPU: on L40S, GeoMean is 1.080 (L1),
2.214 (L2), 1.502 (L3, matching the abstract's L3 figure); on H100, 1.497 (L1), 2.592 (L2), 1.110 (L3).
**ValidRate** (passes both functional correctness and an LLM-based soft-verification pass, §4.2 p.7) is
93%/95%/67% on L40S and 86%/81%/67% on H100 for L1/L2/L3 respectively (Table 3). Against **naive CUDA**
(the agent's own unoptimized starting point, not PyTorch) speedups reach up to **100×**, attributed mostly to
the naive baseline lacking basic tiling/vectorization (§4.6, p.9). Against the **IREE** compiler baseline,
KernelBlaster's PyTorch-relative gains are far larger — IREE itself only reaches 27–28% of PyTorch Eager's
speed on L1/L2 (§4.8, p.10; Table 3 GeoMeans 0.268/0.279 on L40S corroborate this). Against **AI CUDA
Engineer** (Sakana), the primary agentic comparison, on H100 (Fig. 11, p.11): AI CUDA Engineer 1.03× (L1) /
1.21× (L2); KernelBlaster without cuDNN 0.68× (L1) / 1.89× (L2); KernelBlaster with cuDNN enabled 1.43× (L1)
/ 2.50× (L2). On L3, using KernelBench full-model problems: LeNet5 achieves **2.68×**, and SqueezeNetFireModule
is reported at **1.95×** in the main text (§4.9, p.11) but **1.2×** in the appendix worked example (§8.3,
p.25) — see Reading cautions below.

**Ablations isolating the Knowledge Base's contribution (§6.1, p.14).** The key result: a `no_mem_agent`
variant that has *full* NCU profiling access but an *empty* Knowledge Base and no state-conditioned reuse
underperforms the full system, running **1.67× slower**. The paper's own conclusion: "profiling feedback
alone is necessary but not sufficient: the strongest gains arise from the interaction between structured
profiling signals and a persistent, state-aware knowledge base." A related but distinct ablation on
*profiling fidelity* (not memory) shows a cycle-only-feedback agent reaches 1.22× on Level 2 vs. 1.57× with
full NCU data (§6.3, p.15) — profiling detail matters independently of whether it is remembered.
**Cross-hardware and cross-level transfer**: a Knowledge Base trained on an A6000 is reused directly for
optimization runs on H100 and L40S (Fig. 16, p.14); techniques discovered on Levels 1–2 (cross-layer fusion,
algebraic simplification, memory-locality reuse) transfer to Level 3 full-model problems (§4.9, p.11).
**Cost**: a "minimal agent" baseline (CUDA + NCU data in, optimized code out, no Knowledge Base) needs
**2.4× more tokens** for the same 10×10 trajectory budget, achieves only **0.379×** KernelBlaster's
performance-per-token, and loses to KernelBlaster in **71%** of matched cases (§6.4, p.15).

## Comparison to KernelEvolve and AlphaEvolve

KernelBlaster never runs a head-to-head benchmark against either system — the empirical comparisons in §4
are exclusively against AI CUDA Engineer, "Kernelsseum" (a zero-shot prompting baseline, Ouyang et al.
2025a), and the IREE compiler. Both KernelEvolve and AlphaEvolve appear only in related work (p.4), so the
comparison below is this wiki's own reading of mechanism, not a result either paper reports.

| Axis | AlphaEvolve | KernelEvolve | KernelBlaster |
|---|---|---|---|
| What accumulates | a **population of complete candidate programs** + scores in a MAP-elites/island database | (a) **static, hand-authored** hardware docs (b) a **SQL search-graph** of past campaign nodes | compact **`⟨state, ⟨optimization, score⟩⟩`** entries (~50 KB after L1–2) |
| Retrieval key | parent + "inspiration" sampling from the program DB, balancing fitness and diversity | (a) runtime-diagnosed bottleneck → doc retrieval (b) operator-type / input-shape / platform match | an LLM-derived, profiling-based **bottleneck signature**, abstracted away from kernel/operator identity |
| How new knowledge enters | child programs are evaluated and, if they survive selection, added back to the DB | (a) humans write the docs (b) new nodes are appended to the graph | an LLM-driven **rewrite** of existing entries (`PolicyEvaluation`→`PerfGapAnalysis`→`ParameterUpdate`), not just append |
| Exploration mechanism | MAP-elites / island model | `π_sel` pluggable: greedy, MCTS/UCT, or evolutionary population | weighted random search over predicted score (never pure top-1) |
| Touches model weights? | no — Gemini frozen | no — external/internal LLMs frozen | no — GPT-4.1/GPT-5.0 frozen; only the KB text is "updated" |
| Target hardware | Google's internal TPU/XLA stack | NVIDIA, AMD, **and MTIA** (undocumented ASIC) | mainstream NVIDIA GPUs only (A6000/A100/H100/L40S) |

> [!inferred] On the wiki's own "where does the knowledge come from" axis, KernelBlaster sits structurally
> closer to KernelEvolve's search-graph reuse (b) than to AlphaEvolve's program population: both KernelEvolve's
> graph and KernelBlaster's Knowledge Base are *self-generated from the agent's own attempts*, not hand-authored
> domain facts, and both explicitly warm-start new work from prior experience rather than resampling from
> scratch. Three differences are real, though. First, the **retrieval key**: KernelEvolve matches by operator
> type / input shape / platform (kernel *identity*), while KernelBlaster matches by an abstracted profiling
> *bottleneck signature* — its own stated bet is that this transfers "bottleneck-level knowledge... across
> kernels whose surface structure differs" (p.4), which KernelEvolve's identity-based matching cannot do by
> construction. Second, **what is stored**: KernelEvolve's graph nodes are full kernel artifacts with an
> LLM-written `overview.md` each; KernelBlaster stores technique-level distillations, which is why its store
> stays at ~50 KB rather than growing with every kernel variant — the same tradeoff the paper explicitly
> raises against AlphaEvolve-style program archives (p.4: "storing full code artifacts… can incur nontrivial
> storage overhead and inflate the amount of context needed"). Third, **the update rule**: KernelEvolve's
> reuse is retrieve-and-warm-start (no correction of past entries); KernelBlaster's `ParameterUpdate` step
> *rewrites* existing entries when the KB's predicted score for a technique turns out wrong — a genuinely
> different operation, closer to a self-correcting cache than a growing archive.

> [!inferred] This also refines a bullet on [`llm-kernel-generation.md`](../concepts/llm-kernel-generation.md)'s
> "proprietary-hardware problem" section, which currently frames "RL from execution feedback" as KernelEvolve's
> *future-work* item and implicitly assumes it means weight-space fine-tuning (the appeal being that "the
> reward is computed inside the vendor's walls" without exposing architecture details to an external trainer).
> KernelBlaster is evidence that "RL" in this space can mean something that never leaves the *retrieval*
> family at all — it is not a third mechanism sitting between knowledge-injection and weight-space RL, it is
> knowledge-injection wearing RL's vocabulary. A reader who wants an actual weight-updating instance for that
> bullet should look to what KernelBlaster itself cites as "Training-Based Solutions" (§2, p.2): Kevin-32B
> (Baronio et al., multi-turn RL fine-tuning) and CUDA-L1 (Li et al., contrastive RL, *also* pairing weight
> updates with a stored-solution retrieval archive) — neither yet ingested into this wiki.

> [!inferred] AlphaEvolve's most relevant contrast is architectural rather than domain-specific: KernelBlaster's
> §2 related-work critique of evolutionary program databases (p.4) — that they under-represent negative
> outcomes because elite-sampling selection discards low scorers, and that full-program storage is costly —
> is a direct, if implicit, critique of AlphaEvolve's MAP-elites/island design. KernelBlaster's counter-evidence
> is Figure 14 (p.13), which stacks *every* attempt by technique, success and failure alike, and its
> `PerfGapAnalysis` step, which reasons explicitly about *why* an attempt underperformed rather than simply
> letting it lose the selection step. Whether this generalizes better than population-based selection is untested
> here — KernelBlaster reports no ablation removing its own failure-logging or gap-analysis step in isolation.

## Reading cautions

Grounding discipline for anyone citing this preprint's numbers, following this wiki's practice on
[`kernelevolve.md`](kernelevolve.md):

- **The KernelBench Level 3 headline is stated three different ways.** The abstract gives **1.50×** (p.1,
  matching Table 3's L40S Level-3 GeoMean of 1.502). The end of §1 instead states "**2.50×** when
  accelerating entire models in KernelBench Level 3" (p.2–3) — identical to the Level-2 figure quoted one
  sentence earlier, almost certainly a copy-paste duplication rather than a distinct measurement. The
  Conclusion (§7, p.15) gives yet a third figure, "**1.32×** on Kernelbench Level 1 and 2 problems," which
  combines L1+L2 and omits L3 entirely. This wiki uses the abstract's per-level figures (1.43× / 2.50× /
  1.50×), corroborated by Table 3.
- **SqueezeNetFireModule's Level-3 speedup is given as both 1.95× and 1.2×** for what reads as the same
  worked example — §4.9 body text (p.11) says "1.95× improvement over PyTorch"; the Appendix §8.3 worked
  example (p.25), covering the same model, says "achieving a speedup of 1.2× over the PyTorch baseline."
- **Table 3's "Ours" GeoMean on H100 doesn't match either bar in Figure 11.** Table 3 (p.9) reports H100
  GeoMean 1.497 (L1) / 2.592 (L2) under a plain "Ours" row with no cuDNN annotation; Figure 11 (p.11) reports
  two distinct H100 values, "Ours" (no cuDNN) at 0.68×/1.89× and "Ours (w/ cuDNN)" at 1.43×/2.50×. Table 3's
  numbers land in between and match neither exactly, and it is not stated whether the Table 3 row includes
  the cuDNN augmentation.

## Where this fits in the wiki

Registered as the wiki's **third** concrete instance of
[`llm-kernel-generation`](../concepts/llm-kernel-generation.md), alongside [KernelEvolve](kernelevolve.md)
(Triton, NVIDIA/AMD/MTIA, production-deployed) and [AlphaEvolve](alphaevolve.md) (Pallas/XLA on TPU, one
case study among many). It is the wiki's first paper targeting raw **CUDA** rather than Triton or Pallas, and
its Persistent CUDA Knowledge Base is a second, more automated data point on the "durable cross-run agent
memory" thread flagged as an open ingest target in
[`kernelevolve.md`](kernelevolve.md#open-thread) — where it noted that thread's only prior wiki instance was
`pi-autoresearch-vkf`'s VKF card store (see
[`closed-loop-experiment-design`](../concepts/closed-loop-experiment-design.md)). Its correctness discipline
(numerical diff plus an LLM soft-verification pass specifically added after AI CUDA Engineer's documented
reward-hacking exploit, §4.4 p.8) is directly relevant to
[`verification-independence`](../concepts/verification-independence.md). See
[`auto-optimization`](../topics/auto-optimization.md) for the topic-level context this paper sits inside.
