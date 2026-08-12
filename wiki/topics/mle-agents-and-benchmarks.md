# MLE agents and their benchmarks

**Machine learning engineering (MLE) agents** build and iteratively improve an ML solution for a real task
under execution feedback: inspect data, write a pipeline, run it, read the error or the score, revise.
They sit at the intersection of this wiki's two topics — the *loop* is [autoresearch](autoresearch.md)
(hypothesize → implement → evaluate → feed back), the *object* is [auto-optimization](auto-optimization.md)
(feature engineering, model selection, hyperparameters, ensembling — classical AutoML's target, reached
through open-ended code rather than a predefined search space).

MLE matters disproportionately to this wiki because it is the one autoresearch domain where **the loop
closes without a human and the reward is not an LLM judge**. A submission either parses and scores or it
doesn't. That makes MLE the standard testbed for "AI systems that build AI" (AI4AI) and, by extension, for
measuring progress toward recursive self-improvement — the framing
[Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md) builds its whole stack around.

## Three strands, and the gap between them

[Frontis-MA1](../sources/frontis-ma1.md) (§1, p.5) gives the field's cleanest decomposition — prior work
advances MLE agents along three strands that overlap but are rarely spanned by one system:

1. **Inference-time harnesses** — structured or evolutionary search over candidate programs, wrapped around
   a frozen model. *AIDE, AIRA-dojo/AIRA2, ML-Master, MLE-STAR, AutoMLGen, MLEvolve, MLZero, SELA.*
2. **Executable tasks and environments** — the substrate that makes execution feedback available at scale.
   *MLE-Bench, MLE-Dojo, MLE-Smith, MLGym, MLAgentBench, DSBench, SandMLE.*
3. **Post-training from execution feedback** — internalizing verifiable outcomes into the model's weights.
   *ML-Agent, MLE-RL, AceGRPO, RL-MLE.*

The paper's audit (Appendix E, Table 11 — 18 systems scored on Data / Sandbox / Train code / RL method /
Eval / Weights, as of July 2026) finds that **no prior public system spans all three**: high-scoring
systems release an inference framework and an eval entry point but no training stack; resource projects
release tasks and environments but no model; training papers describe an RL method but release neither
weights nor data. OpenMLE claims the first all-six row.

> [!inferred] The three-strand split is a useful lens for reading *any* MLE-agent paper in this wiki, and
> it explains why comparisons across them are so treacherous: a strand-1 result depends almost entirely on
> which frontier model it wrapped (and therefore ages in months), a strand-2 result isn't a score at all,
> and a strand-3 result is usually reported on a weaker backbone than the leaderboard leaders use. Only a
> comparison that holds two strands fixed and varies the third — which is exactly what Frontis-MA1's
> matched harness/model tables do — carries much information.

## The benchmark landscape

Ordered roughly from "build a competition-grade pipeline" to "reproduce or beat published science":

| Benchmark | What it asks | Scale / notes |
|---|---|---|
| **MLE-Bench** (Chan et al. 2024) | end-to-end Kaggle-style competitions; medal thresholds against real human leaderboards | 75 competitions; the **Lite** split is a 22-task low-complexity subset. The de-facto standard. |
| **MLE-Bench Lite** | same, 22-task subset | what nearly every 2026 result quotes — **not** interchangeable with the full 75 |
| **MLE-Dojo** (Qiang et al. 2025a) | standardized *interactive* MLE environments (Gym-style contract) | 200+ tasks; the environment-contract ancestor of OpenMLE-Gym |
| **MLE-Smith** (Qiang et al. 2025b) | automated dataset→task construction | 606 tasks; extended by OpenMLE-Gym's 3,362 Kaggle-dataset branch |
| **OpenMLE-Gym** ([Frontis-MA1](../sources/frontis-ma1.md)) | training substrate, not a leaderboard | **5,758** quality-gated executable tasks (full data released for 1,415) |
| **MLAgentBench** / **DSBench** / **MLGym** | write-execute-debug-submit on realistic ML / data-science tasks | 13 / 74 / 13 tasks |
| **MLS-Bench** (Lyu et al. 2026) | improving ML *components* in ways that generalize across settings and scales | "building better AI" rather than winning one competition |
| **RE-Bench** (Wijk et al. 2025) / **PostTrainBench** (Rank et al. 2026) | open-ended AI R&D; autonomous model post-training | the closest existing benchmarks to literal RSI |
| **[ResearchGym](../sources/researchgym.md)** (Garikaparthi et al. 2026) | withholds the paper's own method from 5 oral/spotlight ICML/ICLR/ACL 2025 repos; agent must beat the paper's human-expert baseline | 39 sub-tasks, single-GPU (12GB), 12–24h, $10–20 budget. GPT-5 `rg-agent`: 6.7% improvement rate (1/15 runs beat baseline), 26.5% avg sub-task completion — the sharpest capability-reliability split in this table. |
| **AIRS-Bench** / **MLRC-Bench** | research-oriented problem solving, end-to-end ML projects | |
| **PaperBench** (Starace et al. 2025) | reproduce a paper | |
| **NatureBench** (Wang et al. 2026) | recover or *improve upon* published scientific results | 90 containerized tasks from Nature-family papers, 6 domains; hidden evaluator; scored by direction-normalized relative gap *g* vs. the paper's SOTA — **Match-SOTA** (*g* ≥ 0) and **Surpass-SOTA** (*g* > 0.1). The **Lite** 10-task subset is Frontis-MA1's transfer test. |

> [!inferred] NatureBench's *g*-against-published-SOTA metric is the most interesting scoring design in
> this table for the wiki's purposes, because it sidesteps the failure mode that dogs every AI-scientist
> system on [autoresearch.md](autoresearch.md#hypothesis-generation-and-idea-evaluation): it needs no LLM
> judge and no novelty assessment. The paper's result is the reference point. The cost is that it can only
> score problems someone has already published a result on — it measures *catching up*, not discovery. It
> is the natural complement to
> [`evolutionary-algorithm-discovery`](../concepts/evolutionary-algorithm-discovery.md)'s regime, which
> needs an automatable evaluator but can exceed any known result.

## Systems in this wiki

- **[RD-Agent](../sources/rd-agent.md)** (Microsoft) — strand 1 + a formalized Research→Development split;
  35.1% Any-Medal on the **full 75-task** MLE-Bench (12 h / 1×V100, GPT-5), and 68.18% on **Lite** in
  Frontis-MA1's audit table under the same backbone and setting. Code ingested at
  [`code/rd-agent/overview.md`](../code/rd-agent/overview.md). See
  [`research-development-loop`](../concepts/research-development-loop.md).
- **[Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md)** (Frontis.AI · Tsinghua) — all three strands in one
  stack: OpenMLE-Gym (environments) → OpenMLE-ERL (operator post-training) → OpenMLE-Evo (long-horizon
  search). 71.21% on MLE-Bench Lite from a **35B open model** on a single 12 GB RTX 4090, above GPT-5.5 +
  Codex. See [`meta-evolution`](../concepts/meta-evolution.md).
- **[The AI Scientist-v2](../sources/ai-scientist-v2.md)** — adjacent rather than in-domain: its agentic
  tree search over experiment code is the same machinery, but the target is a *paper*, not a leaderboard
  submission, so its judge is an LLM/VLM rather than a held-out metric.
- **[AlphaEvolve](../sources/alphaevolve.md) / [openevolve](../code/openevolve/overview.md)** — same
  execution-graded evolutionary recipe pointed at algorithms and kernels instead of Kaggle pipelines.
- **[autoresearch](../code/autoresearch/overview.md)** (Karpathy) — the minimal instance, and cited by
  Frontis-MA1 (p.4) as an example of the AI4AI direction: one file, one 5-minute budget, one frozen metric.
- **[ResearchGym](../sources/researchgym.md)** (TCS Research · Yale) — not an MLE-agent system but the
  sharpest benchmark counterpoint on this page: withheld-method, execution-graded evaluation against a
  paper's own human-expert baseline (not an MLE-Bench medal threshold). GPT-5 `rg-agent` improves over
  baseline in only 1/15 runs (6.7%) despite occasionally reaching (TIM: 1.07× normalized) or matching
  (CL, CMR: 93–96%) the withheld SOTA — the clearest evidence in this wiki that best@k capability and
  reliable improvement are different quantities.

## Reading results in this area without being misled

Three hazards, all visible in Frontis-MA1's own numbers and caveats:

1. **Split.** Lite (22) vs. full (75) differ by tens of points. Always check which.
2. **Budget and hardware.** Table 11's run settings span 12 h · 1×RTX 4090 (12 GB) to 24 h · 8×A100-40G —
   an order of magnitude of sandbox compute, and the table's own footnote says the scores "are not strictly
   comparable" across backbone, budget, hardware, run count, and aggregation.
3. **Run count and variance.** With 22 tasks, one task is 4.5 pp. Frontis-MA1 reports ±5.7 to ±8.6 pp over
   three epochs; the Codex / Claude Code / Gemini CLI references in the same table were run **once**. Any
   cross-vendor gap smaller than ~8 pp is noise.

The comparisons that survive all three are the **matched** ones — hold the harness fixed and swap the
model, or hold the model fixed and swap the harness — which is why those are the numbers this wiki quotes
from [Frontis-MA1](../sources/frontis-ma1.md) rather than its leaderboard position.

## See also
- [`../concepts/meta-evolution.md`](../concepts/meta-evolution.md) — training the improver, on MLE as testbed
- [`../concepts/program-evolution-operators.md`](../concepts/program-evolution-operators.md) — Draft/Improve/Debug/Crossover
- [`../concepts/research-development-loop.md`](../concepts/research-development-loop.md)
- [`autoresearch.md`](autoresearch.md) · [`auto-optimization.md`](auto-optimization.md)
