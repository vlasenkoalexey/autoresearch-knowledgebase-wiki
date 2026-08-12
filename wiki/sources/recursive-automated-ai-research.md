---
title: "First Steps Toward Automated AI Research"
type: source
authors: Recursive (organization; no individual authors credited)
venue: "blog/article, Recursive, 2026-06"
source: ../../raw/papers/recursive-automated-ai-research.md
updated: 2026-08-06
---
# First Steps Toward Automated AI Research — summary

## What it is
A blog-published early-results report from Recursive describing an automated research system that closes a
full research loop with **no human step inside it**: propose an idea, implement it, run an experiment,
validate the result, and use what was learned to choose the next experiment
([raw/papers/recursive-automated-ai-research.md](../../raw/papers/recursive-automated-ai-research.md), §1). The
system runs many research threads in parallel over long horizons, retains useful context from prior
experiments, combines promising branches across threads, and routes every claimed result through a validation
stage before counting it as progress. The article reports three case studies as evidence: **NanoChat
Autoresearch** (built directly on Andrej Karpathy's `autoresearch` repo — the same repo this wiki's own
[`code/autoresearch/overview.md`](../code/autoresearch/overview.md) silo documents, pinned at `228791f`, repo
URL `github.com/karpathy/autoresearch` in both places), a **NanoGPT speedrun** result against Keller Jordan's
`modded-nanogpt` community leaderboard, and a **GPU-kernel-optimization** result against NVIDIA's
**SOL-ExecBench**. There is no linked full technical report, paper, or arXiv id for the system itself — the
article and its companion GitHub artifacts repo are the only primary sources found.

## The method, as described

### The loop
The article's own description of the loop is thin on mechanism detail relative to this wiki's other
autoresearch systems — it names the four stages (propose → implement → run → validate → pick next) but does
not specify the search algorithm, the LLM(s) used, the ratchet/keep-discard rule, or how "promising" is scored
prior to validation (§1). It states the system "harnesses principles of open-ended algorithms, building on
ideas from previous work," without naming which lineage.

### Validating against reward hacking
The article treats reward hacking as the load-bearing risk, not an afterthought: as the search grows more
capable, telling a genuine improvement from a metric exploit gets harder, and the team reports having built
and iteratively tightened a reward-hacking detector using both AI-assisted and human feedback (§1, "What's
Next"). For the kernel case study specifically, the article states that promising kernel improvements were
passed through "increasingly strict automated checks designed to distinguish genuine kernel improvements from
benchmark-specific exploits" before being counted (§4). Neither the general detector nor the kernel-specific
checks are described mechanistically (no worked example of a caught exploit is given), which is a real gap
relative to, e.g., the Darwin Gödel Machine's own worked reward-hacking case study (see Comparison below).

### Long-horizon context and combining branches
The article states the system "keeps useful context from prior experiments" and "combines promising branches"
across its many parallel research threads (§1), but does not describe the data structure this lives in (no
analogue of a `Trace`, `Journal`, archive, or card store is named — contrast the mechanisms this wiki already
tracks on [`concepts/closed-loop-experiment-design.md`](../concepts/closed-loop-experiment-design.md)), nor
how "combine" is implemented (crossover of code, ensembling of ideas, or something else). This is the single
biggest documentation gap in the source: the *outcomes* (beating two community leaderboards and one industry
benchmark) are reported precisely; the *mechanism that produced them* is reported only at the level of a
four-stage loop diagram in prose.

> [!inferred]
> Everything in this "method" section is what the article states; none of it is this wiki's synthesis. The gap
> is flagged, not filled — this wiki has no basis to guess at the missing mechanism and does not attempt to.

## The three reported results

Numbers below are exactly as stated in the article
([raw/papers/recursive-automated-ai-research.md](../../raw/papers/recursive-automated-ai-research.md), §§2–4);
none are independently verified by this wiki (see Caveats).

### NanoChat Autoresearch (vs. the `autoresearch@home` community leaderboard, §2)
- Best community result (`autoresearch@home`, running the same `karpathy/autoresearch` repo/benchmark):
  **val BPB 0.9372**.
- Recursive's system: **val BPB 0.9109** — reported as roughly a 1.3x "speedup-equivalent" improvement (i.e.
  the article's own framing of what the val-BPB gap corresponds to in compute terms, not an independently
  measured wall-clock speedup).
- A separate, from-scratch run starting at a vanilla Transformer baseline improved **1.059 → 0.9344 val BPB** —
  still beating the community's tuned-baseline best of 0.9372, starting with no prior tuning.
- Headline technical finding: hashed bigram/trigram embedding tables mixed into the attention value path
  through learned gates, using disjoint hash-prime pairs per layer to reduce collisions — flagged by the
  article itself against DeepSeek's "Engram" paper (arXiv:2601.07372) as prior published work the underlying
  model may already have known, which the article names as a direct caveat on how much credit to give the
  system for independent discovery (§5).

### NanoGPT Speedrun (vs. the `modded-nanogpt` community leaderboard, §3)
- Prior leaderboard record (time to reach 3.28 validation loss, 8×H100): **79.7 s**.
- Recursive's system: **77.5 s** in the article's own text (the companion GitHub repo's README states **77.3 s**
  for the shared reproduction — a small, unexplained discrepancy between the two primary sources this wiki
  flags rather than silently resolves).
- A separate run starting from a much weaker point (leaderboard entry #5, originally ~15 minutes) was brought
  to **~185 s**, close to where the community leaderboard stood around May 2025 (~180 s) — offered as evidence
  the system can recover most of a large amount of prior human optimization effort largely unaided.
- Named techniques: FP8 (`float8_e4m3`) forward-pass attention projections with bf16 backward for stability;
  an annealed-noise modification to the NorMuon optimizer (arXiv:2510.05491) injecting per-row-scaled Gaussian
  noise onto the orthogonalized update, warmed up over ~50 steps then annealed to zero by roughly a quarter of
  training; extending "cautious" masked updates to embedding tables, not just weight matrices; and a fused MLP
  kernel avoiding an HBM round-trip for squared-ReLU activations.

### SOL-ExecBench (NVIDIA GPU-kernel benchmark, §4)
- Mean SOL (speed-of-light) score across 235 tested kernels: baseline **0.699** → Recursive's system
  **0.754** — reported as an **18% reduction in the remaining gap to the 1.0 theoretical ceiling**, not an 18%
  absolute score increase (0.699→0.754 is a ~7.9-point absolute gain; the 18% figure is `(0.754−0.699)/(1−0.699)`).
- Ten of the 235 generated kernels are shared in the companion GitHub repo; the rest are withheld to avoid
  biasing the public leaderboard.
- Named techniques, one per shared kernel family: a fused Linear→GELU→GRN→Linear kernel that rewrites its own
  weight matrices per forward pass to algebraically fold GRN's affine transform into a prescaled second weight
  matrix; group-limited top-k MoE routing via a bit-packed `(score, expert_index)` key executed as a single
  atomic reduction; an NVFP4-quantized MoE expert-linear kernel using native PTX FP4 packing
  (`cvt.rn.satfinite.e2m1x2.f32`) with FP32 SwiGLU between FP4 layers to avoid cascading rounding error; and a
  GQA paged-decode kernel with fused last-block reduction (atomic "done" counter electing the last-arriving
  block) plus a log2-based online softmax.

> [!inferred]
> None of these three numbers can be independently checked from this wiki — they rest entirely on the
> article's own report plus its companion GitHub repo's partial artifacts (full code for NanoGPT speedrun and
> nanochat_autoresearch scripts; only 10/235 kernels for SOL-ExecBench). Flagging precisely, per the task
> brief: the NanoGPT speedrun number has an unexplained 77.5s (article) vs. 77.3s (repo) discrepancy; the
> SOL-ExecBench "18%" figure describes gap-reduction, not score-delta, and is easy to misquote as the latter;
> and the article's own text explicitly disclaims that the NanoChat n-gram "discovery" may be recall of
       published prior art rather than novel search. Hardware/leaderboard-submission caveats the article
> itself states: results were measured on Modal and independently re-confirmed within noise on Andromeda
> HGX H100 8-GPU nodes, but at publication the team was still awaiting access to PrimeIntellect HGX H100 nodes
> — the official hardware — to formally submit to the leaderboard(s), so neither result had cleared an
> independent leaderboard confirmation at time of writing.

## Relation to `autoresearch` (Karpathy) — same repo, different loop

What the article **states**: the NanoChat Autoresearch case study runs Recursive's system against the exact
same repository this wiki's [`autoresearch` silo](../code/autoresearch/overview.md) documents
(`github.com/karpathy/autoresearch`, verified identical URL in this wiki's `.gitmodules`), scored by that
repo's own `val_bpb` metric, and compared against `autoresearch@home`, a community effort that runs the same
repo/benchmark. That is the full extent of what is stated.

What is **not** stated, and this wiki should not claim: whether Recursive's system operates *inside*
Karpathy's own harness — i.e., using `program.md`'s single-branch edit→train→keep/discard ratchet as-is, one
agent at a time — or whether it wraps the repo's fixed substrate (`prepare.py`'s frozen data pipeline and
`evaluate_bpb` metric, per [`code/autoresearch/overview.md`](../code/autoresearch/overview.md)) inside its own,
separately-built orchestration layer that runs many parallel threads and combines branches. The article's own
description of the general system ("runs many research threads over long horizons... combines promising
branches," §1) is a description of *general* system behavior repeated identically across all three case
studies, not a claim specific to how it interacts with Karpathy's repo.

> [!inferred]
> Reading the two facts together — (a) Karpathy's harness as documented in this wiki is explicitly
> **single-branch**: it keeps only the current best branch and discards a worse attempt outright, with no
> archive of alternatives (see [`code/autoresearch/overview.md`](../code/autoresearch/overview.md) and the
> DGM comparison already in [`topics/autoresearch.md`](../topics/autoresearch.md#darwin-gödel-machine--archive-based-empirically-validated-self-modification));
> and (b) the article's system-wide claim of running many parallel threads and *combining* branches — the most
> defensible reading is that Recursive's system treats `karpathy/autoresearch`'s `train.py`/`prepare.py`/
> `val_bpb` as a **fixed evaluation environment** (the same role it plays for `autoresearch@home`'s human
> competitors) and supplies its own, more capable outer search/orchestration on top, rather than running
> Karpathy's own `program.md` ratchet literally as written. On that reading this is closer in kind to
> [Bilevel Autoresearch](../sources/bilevel-autoresearch.md) (an outer loop wrapped around the same unmodified
> inner benchmark) or the [Darwin Gödel Machine](../sources/darwin-godel-machine.md)'s archive-with-combination
> pattern than to a literal fork of `program.md`'s single-branch keep/discard rule — but the article gives no
> direct evidence either way, and this wiki flags the distinction rather than asserting it. What *is* certain:
> the benchmark, the metric (`val_bpb`), and the frozen data/tokenizer substrate that makes the metric
> hard-to-game are all inherited unmodified from Karpathy's repo — the article reports no change to
> `prepare.py`'s frozen half, only better-scoring edits to the `train.py`-equivalent surface.

The "combines promising branches" claim, if accurate, is itself notable against this wiki's existing
self-improvement systems: Karpathy's own harness has no combination step at all (worse attempts are discarded,
not merged); DGM's archive keeps weak nodes only as *stepping stones* for future single-parent mutation, not
as material to merge; Bilevel Autoresearch's Level 2 replaces one active search mechanism at a time rather than
combining several. If Recursive's system genuinely merges independently-discovered improvements from separate
threads into one candidate, that is a mechanism (closer to genetic crossover, or to Frontis-MA1/OpenMLE's
`Crossover` operator — see
[`concepts/program-evolution-operators.md`](../concepts/program-evolution-operators.md)) this wiki has not
seen demonstrated end-to-end on the `autoresearch` benchmark specifically before. The article does not,
however, show a worked example of two branches being combined, so this remains a claim to track rather than a
verified mechanism.

## Relation to the kernel-optimization results (SOL-ExecBench vs. KernelEvolve / AlphaEvolve)

The SOL-ExecBench result sits in the same family as this wiki's two existing production kernel-optimization
systems — [KernelEvolve](kernelevolve.md) (Meta) and [AlphaEvolve](alphaevolve.md) (DeepMind) — but the metrics
are not directly comparable, which is worth stating precisely rather than eliding:

- **KernelEvolve** reports fitness as `t_pytorch / t_triton`, a wall-clock speedup ratio against a PyTorch
  baseline, with `F = 0` on any correctness failure — see
  [`sources/kernelevolve.md`](kernelevolve.md), §"The system." Headline: 1.25–17× across production workloads,
  480/480 correctness.
- **SOL-ExecBench**'s score is a *speed-of-light* fraction — how close a kernel gets to a hardware-imposed
  theoretical ceiling of 1.0 — which is a different quantity from a speedup ratio over a specific reference
  implementation. Recursive's 0.699→0.754 mean-score improvement cannot be converted into an equivalent "×"
  speedup without knowing each kernel's baseline-vs-ceiling relationship, which the article does not supply.
- Both systems share the same defensive posture against reward hacking that this wiki's
  [`concepts/llm-kernel-generation.md`](../concepts/llm-kernel-generation.md) page identifies as the domain's
  core advantage: a free, mechanically-checkable oracle (correctness via differential testing; here,
  "increasingly strict automated checks... to distinguish genuine kernel improvements from benchmark-specific
  exploits," §4) rather than an LLM judge. Recursive's own framing of this as an evolving, iteratively-tightened
  detector (rather than a fixed rule set, as in KernelEvolve's hand-authored `constraints/` anti-cheating
  subtree) is a difference worth tracking if a fuller technical report ever surfaces — it implies gaming
  attempts were observed and had to be patched against, which the article does not detail but which would be
  a direct data point for
  [`concepts/verification-independence.md`](../concepts/verification-independence.md)'s catalog of observed
  gaming failure modes (DGM's marker-token deletion, Sakana's AI CUDA Engineer memory exploit).
- Both KernelEvolve and Recursive report withholding some fraction of generated artifacts from public release
  (KernelEvolve for competitive/production reasons; Recursive explicitly to avoid biasing the SOL-ExecBench
  public leaderboard) — a shared caveat for anyone trying to independently verify either paper's numbers.

> [!inferred]
> The NanoGPT-speedrun result has no existing counterpart anywhere in this wiki — `modded-nanogpt` is not
> currently tracked as a benchmark on [`topics/auto-optimization.md`](../topics/auto-optimization.md) or
> [`topics/mle-agents-and-benchmarks.md`](../topics/mle-agents-and-benchmarks.md). If this wiki starts tracking
> LLM-agent results against community speedrun leaderboards as a benchmark category, this source page is the
> first data point.

## Where this fits in the wiki

- **[`code/autoresearch/overview.md`](../code/autoresearch/overview.md)** — the exact repo (`karpathy/autoresearch`)
  the NanoChat Autoresearch case study targets; read this first for what the frozen `val_bpb`/`prepare.py`
  substrate this result was scored against actually enforces.
- **[`topics/autoresearch.md`](../topics/autoresearch.md)**, section "Self-improving research loops" — the
  natural landing section; see the DGM and Bilevel Autoresearch entries there for the two existing archive/
  outer-loop patterns this source's "combines promising branches" claim most resembles.
- **[`concepts/closed-loop-experiment-design.md`](../concepts/closed-loop-experiment-design.md)** — this
  source's "keeps useful context... combines promising branches" claim is a feedback-state mechanism this wiki
  cannot yet place on the existing tree/trace/card-store/database axis, because the article does not specify
  the data structure; flagged there as an open gap rather than added to the taxonomy.
- **[`sources/kernelevolve.md`](kernelevolve.md)** and **[`sources/alphaevolve.md`](alphaevolve.md)** — the
  wiki's two other production kernel-optimization systems; see "Relation to the kernel-optimization results"
  above for why the SOL score and the speedup-ratio metrics don't convert directly.
- **[`concepts/llm-kernel-generation.md`](../concepts/llm-kernel-generation.md)** and
  **[`concepts/verification-independence.md`](../concepts/verification-independence.md)** — where
  Recursive's reward-hacking-detector claim would be catalogued if a fuller technical writeup ever supplies a
  worked example of a caught exploit.
- Raw source: [`raw/papers/recursive-automated-ai-research.md`](../../raw/papers/recursive-automated-ai-research.md)
  (structured capture; companion artifacts at
  [`github.com/recursive-org/first-steps-toward-automated-ai-research`](https://github.com/recursive-org/first-steps-toward-automated-ai-research)).
