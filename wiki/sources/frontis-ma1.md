# Frontis-MA1 / OpenMLE: Training an AI4AI Model towards Recursive Self-Improvement in Machine Learning Engineering

**Source:** Junlin Yang, Che Jiang, Yu Fu, Tianwei Luo, Can Ren, Weizhi Wang, Kaikai Zhao, Hongyi Liu,
Yuxin Zuo, Yuru Wang, Yuchen Fan, Kai Tian, Zhenzhao Yuan, Xiaojian Lin, Li Sheng, Rushi Qiang, Guoli Jia,
Xingtai Lv, Ermo Hua, Dianqiao Lei, Youbang Sun, Ning Ding, Bowen Zhou, Kaiyan Zhang (Horizon Research,
Frontis.AI · Tsinghua University · Zhejiang University · SJTU · Georgia Tech), "Frontis-MA1: Training an
AI4AI Model towards Recursive Self-Improvement in Machine Learning Engineering," arXiv:2607.28568v1
[cs.CL] (30 Jul 2026). Technical report, 61 pp. Correspondence: Kaiyan Zhang.
Raw source: [`../../raw/papers/frontis-ma1.pdf`](../../raw/papers/frontis-ma1.pdf).

**Release surface** (title-page links, recoverable only from the PDF's link annotations — they are icon
glyphs in the rendered text): project page <https://frontisai.github.io/OpenRSI> · code
<https://github.com/FrontisAI/OpenRSI> · weights
<https://huggingface.co/collections/FrontisAI/frontis-ma1>. **Ingested as a code silo** —
[`code/openrsi/overview.md`](../code/openrsi/overview.md) grounds OpenMLE-Gym's task contract, OpenMLE-ERL's
reward shaping and RL rollout, the SFT trajectory-collection harness, and OpenMLE-Evo's storage/grading/
async-search layers against real symbols. The single most load-bearing finding from grounding it: the
Draft/Improve/Debug/Crossover operator vocabulary below is **not** uniformly realized in the wired code
paths — the primary SFT scheduler and the RL rollout this ingest cites only ever emit `draft`/`improve`;
`Debug`/`Crossover` as distinct operators only fire through the vendored, third-party AIRA-Dojo `Evolutionary`
solver. See the overview's comparison table for the full per-mechanism grounding (which paper claims are
directly cited, opt-in-but-off-by-default, or live in a sibling module outside the packet subgraph).

> [!note] **This is the first paper in this wiki where the improver's *weights* are the thing being
> improved.** Every self-improvement system ingested so far — `autoresearch`, DGM, Bilevel Autoresearch,
> AlphaEvolve/openevolve — modifies *text*: a training config, an agent scaffold, a search mechanism, a
> candidate program, all proposed by a **frozen** backbone model. Frontis-MA1 closes the other loop: the
> evolutionary search's own transformation operators are **post-trained** (SFT + RL) on the execution
> outcomes that same search produces. See [`meta-evolution`](../concepts/meta-evolution.md) — the concept
> page this paper anchors, and the rung of the ladder the wiki was missing.

## What this paper is

A technical report releasing **OpenMLE**, a three-layer open stack for studying **recursive
self-improvement (RSI)** in the concrete, executable testbed of **machine learning engineering (MLE)**, and
**Frontis-MA1-35B**, the model post-trained on it. The framing (§1, §2, Figure 2 p.4) is *AI4AI* — "AI for
AI," using AI systems to build and improve AI systems — with MLE chosen as the testbed because an MLE
agent's work is verifiable by execution: build an ML solution for a real task, iterate under sandbox
feedback, get a scalar score back.

The report's central architectural claim is that **post-training and inference-time search should share one
interface**, and that interface is a set of four atomic program-evolution operators:

| Operator | What it does |
|---|---|
| **Draft** | write a fresh solution program from the task spec + data |
| **Improve** | refine one existing scored program (exactly one improvement idea per call, evaluation held constant) |
| **Debug** | repair a program that errored / produced no valid submission |
| **Crossover** | synthesize two parent programs into a hybrid "that transcends its predecessors" (Appendix C.2, p.53) |

These four are simultaneously (a) the SFT/RL training targets and (b) the moves the evolutionary search
composes at inference. "This interface lets verified evolutionary transitions supervise the same
transformations that search later composes, making the trained model the variation engine of the
evolutionary harness and forming the meta-evolutionary loop … in which the improver itself is trained"
(p.5). The operator vocabulary is inherited from AIDE / AIRA-style code-space search (Jiang et al. 2025;
Toledo et al. 2025; Hambardzumyan et al. 2026) — OpenMLE's contribution is turning it into **explicit
open-model post-training targets** rather than prompt roles for a frozen model.

## The mechanism ladder (Figure 2, right, p.4)

The paper's own four-rung ladder, which is the single most useful organizing device it offers this wiki:

1. **Evolution** — variation + selection.
2. **Self-Evolution** — experience flows back into the search.
3. **Meta-Evolution** — *the improver is trained* on that experience. ← where this work sits; the model is
   named for it (**M**eta-evolution **A**gent, generation 1).
4. **Recursive Self-Improvement** — the limiting goal: each upgraded system further improves the process
   that produces its successors.

The authors are careful not to overclaim rung 4: OpenMLE "provides a concrete testbed for studying progress
toward RSI in executable MLE, rather than a claim that OpenMLE realizes general, autonomous recursive
self-improvement" (§7, p.30).

## Problem formulation (§2, p.6)

At step *t* the search picks an operator *aₜ* and builds its context *cₜ* from zero or more parent programs
plus their execution feedback; the model samples a program and the sandbox scores it:

> *pₜ ~ g<sub>θ</sub>(· | τ, aₜ, cₜ)*,  *sₜ = R<sub>τ</sub>(E(pₜ, τ))*

where *g<sub>θ</sub>* is the **operator-conditioned program-generation policy**. Within a finite budget the
objective is the single best candidate, *p★ = p<sub>argmax s̃ₜ</sub>* — not average quality. Meta-evolution
then improves *θ* so that *g<sub>θ</sub>* puts more mass on programs with strong execution outcomes; both
SFT and RL are cast as one weighted log-likelihood objective *L<sub>evo</sub>(θ)* differing only in how the
weight *w(sᵢ)* is derived from the execution score.

> [!inferred] The "best-of-budget, not mean" objective is what drives nearly every downstream design choice
> in the paper — adaptive reward bounds, entropic upper-tail weighting, novelty-aware parent selection. It
> is the same objective this wiki's [`autoresearch`](../code/autoresearch/overview.md) ratchet optimizes
> implicitly (keep the best `val_bpb` ever seen), but here it is written down and then propagated into the
> *training* loss, which is the step no other system in this wiki takes.

## Layer 1 — OpenMLE-Gym: verifiable environments at scale (§3, pp.7–10)

**Environment contract** (§3.1): task = spec + public data + hidden evaluator + resource budget + workspace;
action = a submitted MLE program; transition = sandbox execution; observation = a structured record (status,
score, logs, error type, artifacts, runtime); reward = the task-specific evaluator's score. Six feedback
modes are distinguished — success, runtime error, missing code, missing submission, scoring failure,
timeout — "allowing the agent to distinguish invalid execution from weak task performance" (p.10).

**Scale**: **5,758 quality-gated executable tasks**, from three sources trading quality against scale
(Figure 3–4, pp.8–9):

- **156 Curated Anchors** — hand-selected from existing papers/benchmarks; highest confidence, no scale.
- **3,362 Kaggle Dataset tasks** — generated by extending the MLE-Smith dataset→task pipeline, then
  package-level QC.
- **2,240 Kaggle Competition tasks** — the paper's own crawler + auto-construction pipeline over the Meta
  Kaggle catalog. The funnel is stated explicitly: ~11,000 competitions → 3,972 eligible (36%, after
  leaderboard-length screening, **MLE-Bench overlap removal**, licensing/rules) → 2,839 executable packages
  (26%, after auto-generating `prepare.py`/`metric.py` and validating by execution) → **2,240** (20%) after
  a separate LLM semantic quality gate scoring task validity, data sufficiency, raw-data usage, task
  complexity, and data quality, keeping only the strict `recommended` verdict.

Every task compiles to one shared package layout — `raw/`, `data/public/` (agent-visible),
`data/private/test_answer.csv` (hidden), `utils/prepare.py` + `utils/metric.py` — so heterogeneous sources
present one interaction surface. 44% tabular / 18% image / 13% time-series / 11% multimodal / 9% text; 56%
classification + 31% regression. Execution runs on a centralized scheduler dispatching to CPU/GPU Docker
workers with control, execution, and storage separated. **Release caveat (footnote 2, p.10):** full task
data is released for only **1,415** of the 5,758 tasks; the other 4,343 ship as `prepare.py` + `metric.py`
scripts without redistributing the source data, for licensing reasons.

## Layer 2 — OpenMLE-ERL: training the operators (§4, pp.10–15)

**Why train operators and not trajectories** (§4.1): training whole controller trajectories yields sparse,
controller-specific supervision. Training a compact set of reusable *local* transformations lets different
search procedures compose the same learned skills under one sandbox protocol. This separation — local skill
in the weights, global composition in the harness — is the paper's design principle.

**SFT — execution-grounded, budget-adaptive** (§4.2, Figure 7 p.13). Two collection paths feed a
**26,259-example** released corpus:
- *Parallel path*: independently sampled complete `Draft` solutions, threshold-filtered on score →
  **17,245** full-response examples.
- *Evolutionary path*: `Improve`/`Debug`/`Crossover` steps taken over already-executed programs → **9,014**
  trajectory-step examples. The neat detail: when a valid endpoint only emerges after a run of repeated
  `Debug` steps, they **trace back to the preceding non-debug operator** and use an LLM to retain the useful
  steps of that repair trace, rather than supervising on the whole flailing sequence.

Collection stops per task at either an accepted-example quota **or** an execution-budget limit — so easy
tasks terminate early and sparse-success tasks get more attempts. The SFT/RL division of labor is justified
by the RLVR literature (Yue et al. 2025): RL raises Pass@1 by reinforcing already-sampled solutions but
gains little at large *K*, whereas teacher distillation can introduce behaviors *absent from the base
model's support* (p.11).

**RL — three changes for the executable, long-latency regime** (§4.3):

1. **Adaptive reward bounds.** A fixed base reward `r_base = clip((s̃ − b_worst)/(b_best − b_worst), 0, 1)^α`
   (Eq. 1) gives a common interval, but leaderboard/theoretical extrema are far wider than where the current
   policy actually scores — so "meaningfully different programs collapse to nearly identical rewards."
   OpenMLE instead derives tighter bounds from each task's **historical on-policy score frontier**, evolving
   with the policy, preserving resolution where candidates actually live.
2. **Entropic advantage** (Eq. 2) — an exponential-tilt transform *A<sup>ent</sup>ᵢ ≈
   exp(βr<sub>proc,i</sub>) / [mean<sub>j≠i</sub> exp(βr<sub>proc,j</sub>)] − 1*, with β chosen under a
   fixed entropy/KL budget, **replacing GRPO's group-normalized advantage**. It amplifies reward gaps near
   the top of a rollout group, because "a barely viable submission should not receive the same positive
   reward as a top-performing one" (p.13). Measured effect (Figure 8, p.14): mean processed advantage on the
   best candidate rises **1.58 → 6.39 (4.0×)**, and with adaptive bounds the test medal rate goes
   **24.2±5.7 → 34.8±4.3** (on a simpler early-stage harness, not OpenMLE-Evo).
3. **Asynchronous rollouts.** In MLE-RL the dominant latency is *program execution*, not token generation,
   and runtimes vary wildly; a synchronous batch idles on its slowest sandbox job. OpenMLE launches
   generation-and-execution groups independently and lets the trainer consume completed groups from a queue,
   preserving group-level advantages. The speedup claim is deliberately kept **qualitative** in the main
   text since it depends on the task-runtime distribution (measurement deferred to Appendix B.4).

**Which program state to train on** (§4.3, Eq. 3). Non-`Draft` operators need a parent. Uniform parent
sampling wastes updates on exhausted regions; greedy sampling trains repeatedly on the incumbent and kills
diversity. So parents are sampled proportional to a three-term fitness
*F(p) = norm(R<sub>p</sub>) + norm(Var<sub>c∈child(p)</sub> R<sub>c</sub>) + norm(C<sub>p</sub>)*: parent
reward (exploit), **child-reward variance** (regions where operator outcomes are still informative), and a
**visit-cooling** coefficient (stop one incumbent monopolizing the rollout budget).

## Layer 3 — OpenMLE-Evo: experience-driven long-horizon search (§5, pp.15–17)

OpenMLE-Evo adopts an **AIRA-Evo-style population loop** but redesigns how it uses execution evidence. The
paper states the delta against original AIRA-Evo precisely — AIRA-Evo "stores largely free-form memory,
synthesizes it eagerly, selects parents primarily by scalar fitness, and supplies different operators with
broadly similar histories" (p.15). OpenMLE-Evo changes all four:

- **Structured experience accumulation** (§5.1). Every evaluated node gets a deterministic **experience
  card** (provenance, method family, delta-vs-parent, rank, execution outcome, resource usage), and all
  cards aggregate into a task-global **experience board** (explored method families, family-wise bests,
  underexplored directions, repeated failures, score trends, parent graph). Deterministic state first;
  language-model prose only later, on demand.
- **Experience-guided parent selection** (§5.2, Eq. 4). Instead of softmax over normalized fitness alone,
  a three-factor utility *Uᵢ = λ<sub>s</sub>s̃ᵢ + λ<sub>Δ</sub>Δ̃ᵢ + λ<sub>n</sub>νᵢ* over **quality**
  (validation score), **progress** (normalized positive improvement over the strongest parent), and
  **novelty** (method-family novelty), sampled by softmax at temperature τ within an island.
- **Operation-triggered memory synthesis** (§5.3). AIRA-Evo eagerly LLM-summarizes every evaluated node —
  spending inference budget on nodes never selected, and producing a summary *before* the decision context
  that should shape it exists. OpenMLE-Evo defers synthesis until an `Improve`/`Crossover`/`Debug` call has
  already selected its nodes, then summarizes only those, and caches the result.
- **Operator-conditioned context** (§5.4). `Improve` gets the parent's deterministic record + a *vertical*
  trace of recent ancestors + a *horizontal* set of direct siblings (ranked by the same score/gain/novelty
  utility, truncated to the most informative) + the global board. `Crossover` applies this to both parents
  and adds a method-family **complementarity** cue. `Debug` retrieves prior attempts with the **same error
  signature**. Prompts also carry remaining search budget, remaining steps, and per-run execution limit.

**OpenMLE-Evo-Max** (§6.1) adds two things on top: benchmark-independent **experience priors** distilled
from public competition artifacts (all MLE-Bench-related sources excluded before distillation), and
**asynchronous multi-GPU parallel search** at unchanged total sandbox compute.

## Results (§6, pp.17–29)

**Setup.** Official 22-task **MLE-Bench Lite** split, 3 independent runs, **12 h per task on a single RTX
4090 capped at 12 GB VRAM** — the paper notes this is a smaller per-task sandbox budget than the vast
majority of reported MLE-Bench evaluations. Metrics: Valid Rate (*x*/22), **Medal Average**, **Human Rank**
(fraction of human leaderboard participants beaten).

Training and search gains **compose** (Table 1, p.18; Table 9, p.60 gives ±σ over three epochs):

| Model | Harness | Valid | Medal Avg | Human Rank |
|---|---|---|---|---|
| Qwen3.6-35B-A3B (base) | OpenMLE-Evo | 19.67/22 | 39.39% ±5.67 | 0.5828 |
| **Frontis-MA1-35B** | OpenMLE-Evo | 21.67/22 | **60.61%** ±7.73 | 0.7647 |
| **Frontis-MA1-35B** | OpenMLE-Evo-Max | 22.00/22 | **71.21%** ±8.57 | 0.8126 |
| Frontis-MA1-35B | *original* AIRA-Evo | — | 53.03% | — |
| Qwen3-30B-A3B-Thinking (base) | OpenMLE-Evo | 17.33/22 | 34.85% ±2.14 | 0.5573 |
| Frontis-MA1-30B | OpenMLE-Evo | 21.67/22 | 53.03% ±4.29 | 0.7055 |
| GPT-5.6 Sol | Codex | 22.00/22 | 72.73% | 0.8891 |
| Kimi K3 (2.8T) | Claude Code | 22.00/22 | 72.73% | 0.8574 |
| GPT-5.5 | Codex | 21.00/22 | 68.18% | 0.7833 |
| Claude Opus 4.8 | Claude Code | 22.00/22 | 63.64% | 0.8219 |

- **Post-training** is worth **+21.22 pp** at fixed harness (39.39 → 60.61), reproduced at **+18.18 pp** on
  a second backbone/scale (34.85 → 53.03) — the cross-model replication that makes it more than one lucky
  checkpoint.
- **Harness** is worth **+7.58 pp** at fixed model against original AIRA-Evo (53.03 → 60.61), and
  OpenMLE-Evo beats general-purpose Claude Code / Codex scaffolds on four *other* frontier models too
  (GLM-5.2 59.09→62.12, MiniMax M3 54.55→59.09, Kimi K2.6 59.09→66.67, MiniMax M2.7 45.50→50.00) — so the
  harness gain isn't one favorable model–harness pairing.
- **Composed**, a 35B open model reaches 71.21%, above GPT-5.5+Codex (68.18%) and approaching GPT-5.6 Sol
  and the 2.8T Kimi K3 (both 72.73%).
- **Quality, not just threshold-crossing** (§6.4, Figure 15): the medal-tier decomposition shifts toward
  **Gold**, matching Kimi K3's Gold rate — not merely more Bronze.
- **Modality-stratified** (§6.6, Figure 19): Human Rank rises in all five groups and group Medal Rate never
  falls; the 14 extra medals spread across image/text/tabular/audio/multimodal as +2/+4/+1/+4/+3.

**Search efficiency — the mechanism evidence** (§6.5, Figure 16, p.25). Same Frontis-MA1-35B checkpoint,
same seed, 12 h budget, 66 matched task–runs, OpenMLE-Evo vs. original AIRA-Evo:

| | AIRA-Evo | OpenMLE-Evo | Δ |
|---|---|---|---|
| Total model tokens | 129.3 M | 75.3 M | **−41.7%** |
| Prompt tokens | 83.5 M | 41.5 M | **−50.3%** |
| Evaluated nodes | 3,430 | 3,004 | −12.4% |
| New-best validation updates | 229 | 246 | +7.4% |
| New-best updates / 1M tokens | 1.77 | 3.27 | **+84.3%** |
| `Improve` calls that set a new best | 44/931 (4.73%) | 72/769 (9.36%) | **+98.1%** |
| `Improve` prompt, mean / p99 chars | 102.8K / 389.0K | 35.7K / 54.3K | −65.3% / **−86.1%** |
| `Crossover` prompt, mean / p99 chars | 140.4K / 419.2K | 55.3K / 78.4K | −60.6% / −81.3% |

The tokens fall far more than the node count does, which is the paper's argument that the saving comes from
**making each expansion cheaper**, not from searching less. The p99 compression is the sharpest signal:
bounded operator-conditioned context stops an ever-growing history from being re-serialized into every
request.

**Long-horizon behavior** (§6.3). Two grounded trajectories where late `Improve`/`Crossover` — not repeated
repair — produce the gain: `leaf-classification` (Debug establishes viable image and tabular branches →
Crossover fuses them → a late Improve swaps in ConvNeXt-Tiny; the two operator classes account for **85.0%
of total validation gain**; held-out Human Rank **0.9455**, Bronze, vs. 0.732/no-medal for the strongest
comparison) and `mlsp-2013-birds` (**91.9%** of gain; held-out **0.8889**, Silver).

**Two mechanism case studies** (§6.5) isolate the individual components:
- *Targeted Crossover vs. single-branch Debug loop* (`nomad2018`, Figure 17). AIRA-Evo follows one lineage
  through seven successive `Debug` attempts inheriting an expanding full history → val RMSE 0.06633 /
  held-out 0.06096. OpenMLE-Evo's step-81 `Crossover` fuses a physics-features parent (0.06309) with a
  robust `.xyz`-parser parent (0.06573) while horizontal Memory marks an RDF-cache `TypeError` and a
  3328×94 feature mismatch as **negative evidence** to exclude → val 0.06087 / held-out 0.05410, **−8.2%**
  and **−11.3%**.
- *Three-factor selection preserves a complementary parent* (`right-whale`, Figure 18). Parent A leads on
  score (AUC 0.99187); Parent B ranks **6th by score** (0.98773) but **1st by gain** and carries a distinct
  Log-Mel + delta/delta-delta representation. With Score/Gain/Novelty = **1.0 / 0.6 / 0.3**, B's selection
  probability in the same ten-parent pool rises **10.47% → 17.09% (+63.2% relative)**; B is chosen for
  `Improve` and its child reaches val AUC 0.99203 / held-out 0.99386. The paper is careful: the weights
  "do not force a lower-scoring branch to win," they keep a high-gain structurally-distinct branch
  *actionable long enough* to be selected — and the end-to-end delta shouldn't be attributed to the three
  weights alone since targeted Memory changed too.

**Transfer — NatureBench Lite** (§6.6, Table 2, p.28). 10 tasks distilled from Nature-family papers across
six scientific domains, hidden evaluator, web search disabled, 4 h/task; scored by direction-normalized
relative gap *g* against the paper's SOTA — **Match-SOTA** (*g* ≥ 0) and **Surpass-SOTA** (*g* > 0.1). Both
halves transfer, cleanly separated:

| | All S | All M |
|---|---|---|
| Qwen3.6-35B-A3B + *original* AIRA-Evo | 1/10 | 2/10 |
| Qwen3.6-35B-A3B + OpenMLE-Evo NB adapter | 2/10 | 5/10 |
| **Frontis-MA1-35B + OpenMLE-Evo NB adapter** | **3/10** | **7/10** |

Model fixed, swapping the harness: +30 pp Match-SOTA. Harness fixed, swapping the model: +20 pp. The
combined system matches GPT-5.4 / GLM-5.1 / MiniMax-M3 on this subset and beats the reported
DeepSeek-V4-Pro / Claude Opus 4.6 / MiniMax-M2.7 configurations — though it stays well behind Claude Opus
4.7 and GLM-5.2 under Claude Code (both 7/10 S, 10/10 M).

## Release surface — the paper's own comparative audit (Appendix E, Table 11, p.61)

The paper audits 18 representative MLE systems on six artifacts (Data, Sandbox, Train code, RL method,
Eval, Weights) as of July 2026. The finding: high-scoring systems typically release an inference framework
and eval entry point but no training stack; resource projects release tasks and environments but no model;
training papers describe an RL method but release neither weights nor data. **OpenMLE is the only row with
all six ticks.** Selected entries (MLE-Bench Lite Medal Rate, run setting, backbone):

| Work | Medal Rate | Setting |
|---|---|---|
| Famou-Agent 2.0 / MLEvolve | 80.30% | 24 h·1×A800 / 12 h·1×H200, Gemini-3-Pro-Preview |
| AIBuildAI | 77.27% | 24 h·1×A100, Claude-Opus-4.6 |
| ML-Master 2.0 | 75.76% | 24 h·2×RTX 4090, DeepSeek-V3.2-Speciale |
| MLE-STAR-Pro-1.5 | 68.18% | 24 h·2×A100-40G, Gemini-2.5-Pro |
| **R&D-Agent** | **68.18%** | 12 h·1×V100, GPT-5 |
| AutoMLGen / InternAgent | 62.12% | 12 h·1×A800, DeepSeek-R1 |
| AIRA-dojo | 55.00% | 24 h·1×H200, o3 |
| AceGRPO (post-trained) | 51.52% | 12 h, Ace-30B |
| AIDE | 35.91% | 24 h·1×A10, o1-preview |
| MLE-RL (post-trained) | 33.30% | 12 h·A10, MLE-RL-32B-S |
| **OpenMLE (Frontis-MA1-35B)** | **71.21%** | **12 h·1×RTX 4090 (12 GB)** |

The authors state plainly that these scores "are not strictly comparable" across differing backbones,
budgets, hardware, run counts, and aggregation.

> [!note] **Contextualizes, but does not contradict, a claim in this wiki.**
> [`sources/rd-agent.md`](rd-agent.md) records RD-Agent as MLE-Bench SOTA at 35.1% ± 0.4% Any-Medal Rate.
> Table 11 here reports R&D-Agent at **68.18%** — same **GPT-5** backbone, same 12 h · 1×V100 setting. The
> entire difference is the split: RD-Agent's paper reports the **full 75-competition** MLE-Bench, this table
> reports the **22-task Lite** subset, which is the easier low-complexity slice. Two measurements of the
> same system, not a revision. What *is* superseded is the framing — "SOTA on MLE-Bench" was a mid-2025
> statement, and by July 2026 this table alone lists eight systems at or above 68% on Lite (Famou-Agent 2.0
> and MLEvolve at 80.30%). The `index.md` entry and the rd-agent source page are annotated accordingly
> rather than rewritten, since the original result stands exactly as reported.
>
> **Watch the split when comparing any number on this page.** Every Medal Average in this report is
> MLE-Bench **Lite** (22 tasks); every Medal Rate on [`sources/rd-agent.md`](rd-agent.md) is the full 75.
> They are not interchangeable.

## Limitations (the authors' own, §8, pp.30–31)

Five named capability boundaries between OpenMLE and real RSI — unusually specific, and each one maps onto
a gap this wiki tracks:

1. **Richer objectives for improving the improver.** Training learns only from *measured execution outcome*
   — whether a program works and how well it scores. That signal says nothing about whether a research
   *direction* is promising, generalizable, robust, or worth more compute. "The system is better equipped
   to optimize solutions than to judge which ideas deserve to be pursued."
2. **Integrating evolutionary search with general coding agents.** Trained operators are composed by an
   *external* harness, which bounds the actions the model can initiate on its own.
3. **Broader participation in AI development.** The agent improves *external* ML artifacts; RSI needs
   agents participating in more of the AI-development process, "especially the improvement of language
   models themselves."
4. **Evolving the evolutionary system.** Evolution operates over candidate *solutions*; the evolutionary
   system itself stays fixed. Making it an object of evolution is named as the next step.
5. **Richer use of experience in node expansion.** The experience card records a broad set of deterministic
   metadata but parent selection consumes only three hand-picked factors with **fixed** weights; learning
   task-dependent weights — and ultimately letting the search policy *discover which experience signals are
   predictive* — is flagged as the path "from hand-designed experience guidance toward an evolutionary
   system that improves its own search behavior."

## Where this sits in this wiki

- **The ladder.** Limitations 3 and 4 are exactly the boundaries
  [`self-referential-code-rewriting`](../concepts/self-referential-code-rewriting.md) and
  [`mechanism-level-self-improvement`](../concepts/mechanism-level-self-improvement.md) are about. DGM
  rewrites its own scaffold but its backbone weights are frozen; Frontis-MA1 trains its own weights but its
  harness is fixed and human-authored. **Neither system does both** — they are orthogonal halves of the
  same ambition, and naming that is the most useful synthesis this paper enables. See
  [`meta-evolution`](../concepts/meta-evolution.md).
- **The operators.** Draft/Improve/Debug/Crossover is the same vocabulary AIDE gave The AI Scientist-v2's
  tree search and that openevolve realizes as SEARCH/REPLACE diffs — see
  [`program-evolution-operators`](../concepts/program-evolution-operators.md).
- **Karpathy's `autoresearch` is cited by this paper** (p.4, "Karpathy, 2026") as an instance of the AI4AI
  direction — the harness already ingested at [`code/autoresearch/overview.md`](../code/autoresearch/overview.md).
- **Benchmarks.** MLE-Bench, MLE-Bench Lite, NatureBench, MLE-Dojo, MLE-Smith, MLGym, DSBench,
  MLAgentBench, RE-Bench, PaperBench, MLS-Bench, ResearchGym, AIRS-Bench, PostTrainBench — the landscape
  this report surveys is collected in
  [`topics/mle-agents-and-benchmarks.md`](../topics/mle-agents-and-benchmarks.md).

> [!warning] **No component ablations — the word "ablation" appears zero times in the 61 pages.** The paper
> reports excellent *controlled swaps* (fix the harness and swap the model; fix the model and swap the
> harness) and two component comparisons (Figure 8: with/without entropic weighting; Figure 16: OpenMLE-Evo
> vs original AIRA-Evo), but it never decomposes its own training stack. In particular **there is no
> SFT-only number** — the +21.22 pp is reported only as base → final, so how much came from the supervised
> warm start versus from RL is unknown. Compare [DGM](darwin-godel-machine.md), which ablates the archive,
> the mutator's self-improvement, and greedy-vs-probabilistic selection, and
> [AlphaEvolve](alphaevolve.md), which removes one mechanism at a time and reports that each contributes.
> This matters for anyone planning an SFT-weighted program: the paper's own theory (§4, citing Yue et al.
> 2025 — distillation introduces out-of-support behavior, RL concentrates within support) predicts SFT
> should carry the capability-closing share, but the paper does not measure it. Worked through for the TPU
> case in [`notes/frontis-openmle-applied-to-tpu-optimization.md`](../notes/frontis-openmle-applied-to-tpu-optimization.md).

> [!inferred] **Read the headline number with the variance in view.** Medal Average carries ±7.73 pp
> (OpenMLE-Evo) and ±8.57 pp (Evo-Max) across three epochs, so the 3.03 pp margin over GPT-5.5+Codex sits
> well inside one standard deviation — and per §6.1 and Appendix D.1, the Codex / Claude Code / Gemini CLI
> references were run **once** each (point estimates, no dispersion) because of inference and sandbox cost.
> With 22 tasks, one task is 4.5 pp. The robust claims here are the *controlled* ones, where the paper
> changes exactly one thing and holds everything else fixed: +21.22 pp from post-training at fixed harness,
> reproduced at +18.18 pp on a second backbone; +7.58 pp from the harness at fixed model; and the 66-run
> matched token-efficiency study, which is a mechanism measurement rather than a leaderboard placement.
> The cross-vendor comparisons are the weakest evidence in the paper and the authors say so themselves.
