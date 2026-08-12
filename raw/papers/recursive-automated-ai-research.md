# First Steps Toward Automated AI Research

- **Author/org:** Recursive
- **URL:** https://www.recursive.com/articles/first-steps-toward-automated-ai-research
- **Published:** 2026-06-11 (article's own byline date; the requesting task referred to it generically as "2026-06")
- **Fetched:** 2026-08-06
- **Companion artifacts repo:** https://github.com/recursive-org/first-steps-toward-automated-ai-research (Apache 2.0,
  with attribution to MIT-licensed upstream code it builds on)
- **Capture method:** This is a structured, detailed **paraphrase** of the article's content assembled from an
  automated fetch/extraction pass over the live page and its linked GitHub repo, not a verbatim scrape or
  reproduction of the publisher's text. Section order follows the article's own headings. Numbers and named
  techniques are reported as facts; short technical terms are quoted where the article's own phrasing is the
  citable artifact (e.g. a named mechanism), but full sentences are paraphrased rather than block-quoted. No
  fuller technical report, paper, or arXiv id for the system itself was found linked from the article — the
  only outbound arXiv links are to two cited *prior-work* papers (DeepSeek Engram, NorMuon; see below). If a
  fuller writeup exists, it was not discoverable from the article page as fetched.

## Section 1 — Framing / what the system is

The article frames the work as early results from an automated research system built at Recursive that closes
a full research loop with no human step inside it: propose an idea, implement it, run an experiment, validate
the result, and use what was learned to pick the next experiment. The system runs many research threads in
parallel over long horizons, retains useful context from prior experiments rather than starting cold each
time, combines promising branches from different threads, and routes every claimed result through a
validation stage before it is treated as real progress. The article states the system was built to scale, and
that it draws on principles from open-ended search algorithms and on prior published work (the article does
not further specify which open-ended-algorithm lineage beyond this general framing).

A cross-cutting concern named explicitly, before any of the three case studies, is **reward hacking**: as the
search becomes more capable, distinguishing a genuine improvement from a metric exploit becomes harder, and
the article states the team built and iterated on a reward-hacking detector using both AI-assisted and human
feedback, tightening it over time. The article's closing framing (see "What's Next" below) treats getting this
right — aligning the system to the *spirit* of a task rather than gaming its *letter* — as the central open
problem for any system that automates research and self-improves.

## Section 2 — Case study 1: NanoChat Autoresearch

Explicitly built on **Andrej Karpathy's `autoresearch` repository** (linked as
`github.com/karpathy/autoresearch` — the exact repo this wiki's own `wiki/code/autoresearch/` silo documents),
and benchmarked against the community effort **autoresearch@home**
(`ensue-network.ai/lab/autoresearch`), which runs the same repo/benchmark competitively.

Reported numbers:
- Best community (autoresearch@home) validation bits-per-byte (val BPB): **0.9372**.
- Recursive's system: **0.9109** val BPB — described as roughly a 1.3x "speedup-equivalent" improvement (i.e.
  the gap in val BPB translates to that much less compute needed to reach the same loss, per the article's own
  framing).
- A separate, harder run starting from a vanilla Transformer baseline (rather than the community's already
  tuned starting point) improved from **1.059 BPB** to **0.9344 BPB** — still beating the autoresearch@home
  community best of 0.9372, starting from scratch.

Named technical discovery (the article's headline finding for this case study): **hashed bigram and trigram
embedding tables mixed into the attention value path through learned gates** — a cheap mechanism for injecting
local n-gram statistics into the model without a full embedding table, using different hash functions (disjoint
hash-prime pairs) across layers to reduce collisions. The article links this to prior published work on hashed
n-gram embeddings — **DeepSeek's "Engram"** paper (arXiv:2601.07372) is cited as related/prior art the model
may have known about, which the article flags as a caveat on how much to credit the system with independent
discovery (see Limitations below).

Beyond the n-gram mechanism, the article describes the accepted change set as touching architecture, a
short-context memory mechanism, auxiliary losses, attention, optimizer behavior, weight-decay schedules, and
compiler settings, without enumerating each individually. The from-scratch (vanilla-Transformer-start) run
converged on a different, independently-derived set of changes, including causal token shifting (blending a
token's query/key projections with those of the preceding token via learned coefficients) and byte-level
feature embeddings (embeddings capturing sub-token/byte composition information).

## Section 3 — Case study 2: NanoGPT Speedrun

Benchmarked against **Keller Jordan's `modded-nanogpt` speedrun leaderboard**
(`github.com/KellerJordan/modded-nanogpt`) — the community record for time-to-reach a fixed validation-loss
target (3.28) on 8×H100.

Reported numbers:
- Prior leaderboard record: **79.7 seconds**.
- Recursive's system: **77.5 seconds** (the companion GitHub repo's README states 77.3s for the shared
  reproduction) — roughly a 2.2-second improvement over the prior record.
- A separate run starting from a much weaker point (leaderboard entry #5, originally ~15 minutes) was brought
  down to approximately **185 seconds**, close to where the community leaderboard stood around May 2025
  (~180 seconds) — used as a demonstration that the system can recover most of a large amount of prior human
  optimization effort largely on its own.

Named technical discoveries:
- **FP8 in the attention projection path.** A custom operation performs the forward matmul in the `float8_e4m3`
  format (4 exponent bits, 3 mantissa bits) for roughly double tensor-core throughput, while keeping the
  backward pass in bf16 for numerical stability.
- **Annealed exploration noise inside the optimizer.** A modification to the **NorMuon** optimizer
  (arXiv:2510.05491, cited as the base optimizer the system's variant builds on) injects zero-mean Gaussian
  noise onto the orthogonalized, variance-reduced update, with the noise's standard deviation scaled per row;
  the noise is warmed up over the first ~50 steps, then linearly annealed to zero by roughly a quarter of the
  way through training.
- **Cautious updates extended to embedding tables.** "Cautious" weight decay/updates (masking parameter updates
  where the adaptive step direction opposes the raw gradient direction) were extended to the bigram and
  value-embedding tables, not just the main weight matrices.
- **A fused MLP kernel.** The forward pass stores only the squared-ReLU activations; the backward pass
  reconstructs the unsquared activations on the fly inside the kernel, eliminating a full activation tensor's
  round trip to HBM.
- In the weaker-starting-point run, the system independently arrived at: stitched-stream attention (packing
  eight sequences into a single stream), a per-layer window pyramid (mixing local and longer-range attention
  spans by layer), narrowed attention (four heads rather than a wider configuration), and a cross-layer
  difference mechanism (later layers blending in earlier layers' outputs).

## Section 4 — Case study 3: SOL-ExecBench

Benchmarked against **NVIDIA's SOL-ExecBench** (`research.nvidia.com/benchmarks/sol-execbench`), a leaderboard
that scores generated GPU kernels by a "SOL" (speed-of-light) score — how close a kernel gets to a theoretical
hardware-limited optimum of 1.0 — across a set of representative kernel tasks.

Reported numbers:
- Mean SOL score across the tested 235 kernels: prior baseline **0.699** → Recursive's system **0.754** —
  described as an 18% reduction in the remaining gap to the 1.0 (speed-of-light) ceiling.
- The companion GitHub repo shares 10 representative kernel implementations out of the 235 the system produced;
  the article/repo state the majority were withheld deliberately to avoid biasing the public leaderboard.

Named technical discoveries, one representative example per kernel family the article walks through:
- **A fused Linear→GELU→GRN→Linear kernel** that rewrites its own weight matrices on every forward pass to
  algebraically absorb GRN's (Global Response Normalization's) affine transform into a prescaled second weight
  matrix with precomputed per-channel scales, removing a separate normalization step.
- **Group-limited top-k routing** (for a Mixture-of-Experts-style gate) implemented via a bit-packed
  `(score, expert_index)` key — the upper 24 bits hold the IEEE-754 bit pattern of the score, the low byte
  holds `255 − expert_idx` as a tie-breaker — letting the whole top-k selection execute as a single atomic
  reduction.
- **An NVFP4-quantized MoE expert linear kernel** using native PTX FP4 packing
  (`cvt.rn.satfinite.e2m1x2.f32`) to pack two FP4 values per byte directly rather than soft-emulated
  quantization, with the SwiGLU nonlinearity computed in FP32 between the FP4 layers specifically to avoid
  cascading rounding error.
- **A GQA paged-decode kernel** (for the FlashInfer-Bench task family) using a fused last-block reduction with
  an atomic "done" counter to elect the last-arriving thread block to merge partial results, plus a
  log-base-2 online-softmax formulation using the `ex2.approx.f32` PTX instruction.

The article states that "promising improvements were passed through increasingly strict automated checks
designed to distinguish genuine kernel improvements from benchmark-specific exploits" before being counted —
the SOL-ExecBench-specific instance of the article's general reward-hacking-validation claim.

## Section 5 — What's Next / limitations and caveats stated in the article

- **On independent discovery:** the article is explicit that matching or rediscovering a published technique
  (e.g. the n-gram embedding idea overlapping DeepSeek's Engram paper) "does not necessarily prove independent
  rediscovery, since the underlying models may know many public techniques including those used by or created
  by the autoresearch@home community" — i.e. the article itself flags that some of what looks like discovery
  could be recall of pretraining-corpus knowledge rather than genuine novel search.
- **On hardware/leaderboard submission status:** results were obtained on Modal HGX H100 8-GPU nodes and
  independently re-confirmed within noise on Andromeda HGX H100 8-GPU nodes; at time of publication the team
  was still awaiting access to PrimeIntellect HGX H100 8-GPU nodes — the official hardware required to submit
  to the (implied: NanoGPT speedrun and/or SOL-ExecBench) leaderboard(s).
- **On auditing generated kernels:** the team states they manually checked a subset of the highest-performing
  kernels and may still have missed errors in kernel optimizations outside their own specialist expertise —
  explicitly framed as part of the point, since the techniques came from the system rather than from the
  authors' own prior domain expertise.
- **Scope claim:** the article characterizes these as early results showing the system "can push the frontier
  on AI training and infrastructure tasks, especially when the goal is well-defined, measurable, and quick
  enough to evaluate many times" — i.e. an explicit scoping to fast-feedback, well-specified benchmark tasks,
  not a general claim about open-ended scientific discovery.
- **Grand-challenge framing:** the closing paragraph names reward hacking as an increasingly central risk as
  the search grows more powerful, and frames aligning such systems to the spirit rather than the letter of a
  task as "a grand challenge of creating systems that automate knowledge discovery and recursively self-improve
  in a way that is safe and helpful."
- **Hiring call-to-action:** the article closes with an invitation to apply to join the team building this
  work, contact `talent@recursive.com`, alongside the mention of open-sourcing artifacts at the GitHub repo
  linked above.

## Outbound links found in the article body

1. `github.com/karpathy/autoresearch` — "Andrej Karpathy's NanoChat autoresearch repo"
2. `ensue-network.ai/lab/autoresearch` — "autoresearch@home"
3. `arxiv.org/abs/2601.07372` — "DeepSeek Engram"
4. `github.com/KellerJordan/modded-nanogpt` — "NanoGPT Speedrun"
5. `arxiv.org/abs/2510.05491` — "NorMuon"
6. `research.nvidia.com/benchmarks/sol-execbench` — "SOL-ExecBench"
7. `github.com/recursive-org/first-steps-toward-automated-ai-research` — "open-sourcing artifacts" (linked
   twice in the article)

## Companion GitHub repo contents (for grounding)

- `nanoGPT_speedrun/` — the training-optimization implementation reaching the ≤3.28 FineWeb validation-loss
  target in 77.3s on 8×H100, built on the MIT-licensed `modded-nanogpt` codebase with attribution retained.
- `SOL-ExecBench/` — 10 of the 235 generated GPU kernels shared as representative examples (the rest withheld
  to avoid biasing the public leaderboard).
- `nanochat_autoresearch/` — training scripts and validation metrics across 10 random seeds, measuring
  bits-per-byte on a single B200 GPU within a 5-minute budget window.
- License: Apache 2.0 for Recursive's own contributions, with MIT-licensed upstream code (from Karpathy's and
  Jordan's repos) attributed per its original license.
