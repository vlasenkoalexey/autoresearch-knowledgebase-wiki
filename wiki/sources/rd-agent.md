# RD-Agent (Microsoft Research)

Microsoft Research's **R&D-Agent** is a framework that automates the "high-value generic R&D
processes" of AI development — data and model engineering — by formalizing them as an explicit,
decoupled **Research → Development** loop, with a fixed six-component design underneath it. The
GitHub project (https://github.com/microsoft/RD-Agent, not itself ingested here — that is a
separate, later step) bundles two published evaluations of essentially the same architecture:

1. **The general framework paper** — *"R&D-Agent: An LLM-Agent Framework Towards Autonomous
   Data Science"* (arXiv:2505.14738v2, Microsoft Research Asia / Microsoft GenAI), evaluated on
   **MLE-Bench** (real Kaggle competitions). Downloaded to
   [`raw/papers/rd-agent.pdf`](../../raw/papers/rd-agent.pdf).
2. **The quant-finance specialization** — *"R&D-Agent-Quant: A Multi-Agent Framework for
   Data-Centric Factors and Model Joint Optimization"* (arXiv:2505.15155v2, accepted NeurIPS 2025),
   which instantiates the same Research/Development split as **RD-Agent(Q)** for automated
   quantitative-trading strategy R&D — coordinated **factor–model co-optimization**. Downloaded to
   [`raw/papers/rd-agent-quant.pdf`](../../raw/papers/rd-agent-quant.pdf).

> [!inferred] The two papers share several authors (Xu Yang, Xiao Yang, Weiqing Liu, Jiang Bian) and
> both point at the same `microsoft/RD-Agent` GitHub repo, but they are formally **separate arXiv
> submissions** with non-overlapping experiments — the general paper (`2505.14738`) never mentions
> quant finance or RD-Agent(Q), and the quant paper (`2505.15155`) never mentions MLE-Bench. This
> summary treats them as one project told in two papers, per the task that motivated this ingest.

## The general R&D-Agent framework (`raw/papers/rd-agent.pdf`)

### Motivation
Machine learning engineering (MLE) — going from a raw dataset to a trained, evaluated solution — is
still slow and labor-intensive even for expert data scientists, and prior LLM-agent systems for MLE
(AIDE, ML-Master, KompeteAI, MLE-STAR, AIRA) each optimize only a narrow slice of the workflow, per
Table 1 of the paper (rd-agent.pdf, p.2). The paper's framing: "all the existing methods can be
summarized as a partial optimization from our framework's simple baseline" (rd-agent.pdf, p.2).

### The Research / Development split
R&D-Agent formalizes the MLE workflow into **two phases and six components** (rd-agent.pdf, pp.4–6):

**Research phase** — discover and refine promising ideas before costly implementation:
1. **FC-Planning** — dynamically allocates exploration effort over time (explore early, exploit
   late), adjusting budget/guidelines as the time budget is consumed.
2. **FC-Exploration Path Structuring** — how candidate solutions are organized/referenced (chain vs.
   tree search); R&D-Agent uses an adaptive DAG that maximizes diversity in the first layer, then
   greedily exploits the best branch.
3. **FC-Reasoning Pipeline** — turns memory context into concrete ideas via dataset analysis,
   hypothesis formulation, and trade-off assessment.
4. **FC-Memory Context** — stores/retrieves historical solutions and insights across iterations.

**Development phase** — turn the chosen idea into a bug-free, evaluated solution:
5. **FC-Coding Workflow** — idea → runnable code, emphasizing early bug detection via rapid
   prototyping on sampled data.
6. **FC-Evaluation Strategy** — reliable, consistent scoring (stable metrics, fixed validation
   splits, aggregated evaluation to filter noise/overfitting).

The high-level loop (Algorithm 1, rd-agent.pdf p.6) is: while time remains, run
**Planning → SelectParents (exploration path) → Memory Context → Reasoning Pipeline** (Research),
then **Dev (coding workflow) → Eval (evaluation strategy)** (Development), appending the result
`(parents, idea, code, score)` to a growing exploration graph `G`; a **research-and-development
loop** in the paper's own terminology is called an **"R&D loop."**

### The SOTA configuration (`Module Design`, rd-agent.pdf pp.6–7)
Guided by human-expert workflows, the authors instantiate each of the six components concretely:
dynamic time-aware planning (light compute early, ensembles/cross-validation later); an adaptive
DAG exploration structure; a "scientific multi-step" reasoning pipeline (problem → hypothesis →
implementable idea, with an LLM-based **virtual evaluation** step that filters multiple candidate
ideas down to one before development); **collaborative memory** — a probabilistic interaction kernel
(Eq. 1, rd-agent.pdf p.19) that lets parallel exploration branches share their best/similar
hypotheses without collapsing diversity; an **efficient & iterative debug workflow** — prototype on
a small data sample first, only promote validated code to full-scale runs; and an **aggregated
evaluation strategy** with standardized train/val/test splits plus a cross-branch re-validation
layer.

### Benchmark results
Evaluated on **MLE-Bench** (75 real Kaggle competitions, Chan et al. 2024) under a harder-than-usual
setup — 12h budget vs. the standard 24h, and a single V100 GPU vs. competitors' A10/A100/H200
(rd-agent.pdf, p.7):
- R&D-Agent (GPT-5) reaches **35.1% ± 0.4% Any-Medal Rate**, a new SOTA, beating the prior best
  ML-Master (29.3% with DeepSeek-R1) by 5.8 points (rd-agent.pdf, Table 2, p.8). A hybrid
  `o3(Research) + GPT-4.1(Development)` configuration also beats all baselines at 29.7%.
- Controlling for the LLM (re-running ML-Master with GPT-5 in the same environment gives only
  16.9%), the paper argues the gain is architectural, not just a stronger backend model.
- **Ablations** (Table 3, rd-agent.pdf p.8) show exploration-path structuring matters most (removing
  it costs 28% relative Any-Medal Rate), followed by reasoning pipeline and planning (~24% each),
  then memory context (~9%). On the development side, removing the efficient debug workflow drops
  performance immediately and persistently (34.7% → 24.0%), while removing the aggregated evaluation
  strategy only hurts after ~2 hours, once solutions get complex enough to overfit.
- A **case study** on the Jigsaw Toxic Comment Classification task (rd-agent.pdf, Appendix F, pp.29–33)
  contrasts R&D-Agent's generated solution (custom `AsymmetricLossMultiLabel` loss, OOM-adaptive batch
  sizing, head+tail text truncation, dropout-regularized RoBERTa head) against ML-Master's more
  generic solution (standard `BCEWithLogitsLoss`, un-modified pretrained model) — R&D-Agent won a
  bronze medal, ML-Master finished just above median.
- Surprisingly, adding a retrieval-augmented-generation (RAG) knowledge base of 85 other Kaggle
  competitions **hurt** overall performance (35.1% → 32.0%), helping only on high-difficulty tasks
  (rd-agent.pdf, Appendix C.2, p.16) — the paper's interpretation is that modern LLMs already
  internalize common ML patterns, and retrieval mostly injects noise on standard tasks.

## RD-Agent(Q): quant-finance factor–model co-optimization (`raw/papers/rd-agent-quant.pdf`)

### Motivation
Quantitative-investing research pipelines have historically split into **factor mining**
(hand-crafted features → symbolic regression → RL-optimized factor combinations) and **model
innovation** (classical ML → deep sequence models → market-aware architectures like MASTER), run as
two siloed workflows with limited automation, weak interpretability of LLM-only signal generation,
and no cross-stage feedback (rd-agent-quant.pdf, p.2). **R&D-Agent(Q)** is presented as "the first
data-centric multi-agent framework designed to automate the full-stack research and development of
quantitative strategies via coordinated factor-model co-optimization" (rd-agent-quant.pdf, Abstract).

### Five units implementing the same Research/Development split
RD-Agent(Q) decomposes the quant pipeline into five LLM-powered units across the same two phases
(rd-agent-quant.pdf, Fig. 3, p.3):

- **① Specification Unit** (top of Research) — dynamically encodes the task tuple
  `S = (B, D, F, M)` (background/prior knowledge, data interface, expected output format, execution
  environment i.e. Qlib backtesting) so every downstream unit shares one operational contract.
- **② Synthesis Unit** (Research) — generates the next hypothesis from a "knowledge forest" of prior
  hypotheses/feedback, conditioned on the current optimization action `a ∈ {factor, model}`
  (Eq. 1, rd-agent-quant.pdf p.4); factor hypotheses decompose into multiple sub-tasks, model
  hypotheses map to one task, mirroring their different structural coherence.
- **③ Implementation Unit** (Development) — runs **Co-STEER**, a dedicated code-generation agent that
  (a) builds a DAG over candidate tasks and derives a complexity-aware topological schedule, and
  (b) retrieves similar past task/code/feedback triples from a persistently growing knowledge base
  to seed new code generation (rd-agent-quant.pdf, Fig. 4 and Algorithm 1, pp.4,17). Co-STEER is
  benchmarked against Few-shot/CoT/Reflexion/Self-Debugging/Self-Planning on **RD²Bench** and wins on
  every metric (execution rate 0.889, avg. correlation 0.646 vs. next-best 0.454 — Table 10,
  rd-agent-quant.pdf p.27), and an "evolving scheduler" beats random scheduling at every top-k budget
  (Table 11, p.28).
- **④ Validation Unit** (Development) — de-duplicates new factors against the current SOTA factor
  library by pairwise IC correlation (factors with `IC_max ≥ 0.99` against an existing factor are
  dropped as redundant), then backtests the survivors via **Qlib** under realistic transaction costs.
- **⑤ Analysis Unit** (bridges phases) — scores each round against the current SOTA, feeds
  structured feedback back to the Synthesis Unit, and — the paper's key coordination mechanism —
  decides whether the **next** iteration should optimize the factor set or the model, formulated as a
  **contextual two-armed bandit** solved via linear Thompson sampling over an 8-dimensional
  performance-state vector (IC, ICIR, rank-IC, rank-ICIR, ARR, IR, −MDD, SR) (rd-agent-quant.pdf,
  §2.5 and Appendix A.2, pp.5,16).

### Benchmark results
On the CSI 300 constituent-stock dataset (train 2008–2014 / val 2015–2016 / test 2017–2020),
compared against factor libraries (Alpha 101/158/360, AutoAlpha) and ML/DL baselines
(LightGBM, XGBoost, GRU/LSTM/Transformer, PatchTST, iTransformer, Mamba, TRA, MASTER)
(rd-agent-quant.pdf, Table 1, p.7):
- **R&D-Factor** alone (fixed LightGBM model, factor set optimized from a 20-factor seed) reaches
  IC up to 0.0497 and ARR up to 14.61%, beating static libraries while using far fewer factors.
- **R&D-Model** alone (fixed Alpha-20 factor set, model optimized) reaches the best Rank IC (0.0546)
  and lowest max drawdown (−6.94%) among all baselines and configurations.
- **R&D-Agent(Q)** — joint factor+model co-optimization — achieves the **highest overall
  performance**: IC 0.0532, ARR 14.21%, IR 1.74 (o3-mini backend), exceeding the strongest single-axis
  baselines by a wide margin — the paper's central empirical claim that joint optimization unlocks
  complementary gains neither axis alone can reach.
- Out-of-sample generalization was checked on **CSI 500** and **NASDAQ 100** with a 2024–2025 test
  window chosen so the LLM backends' training cutoffs precede the test period (avoiding leakage);
  R&D-Agent(Q) again tops both markets (Table 2, rd-agent-quant.pdf p.9), e.g. IR (SHR*) 2.17 on
  CSI 500 and 1.77 on NASDAQ 100 with the o4-mini backend.
- **Ablation** of the Analysis Unit's scheduler (Table 3, rd-agent-quant.pdf p.9) shows the bandit
  scheduler beats both an LLM-based scheduler and random scheduling on IC, ARR, and number of SOTA
  selections found under the same 12-hour compute budget.
- **Cost**: full R&D-Agent(Q) runs stay **under $10 per optimization cycle** (rd-agent-quant.pdf,
  Appendix D.5, p.28), and a real-world validation on the Kaggle "Optiver Realized Volatility
  Prediction" competition (Appendix D.6, pp.28–29) shows the system autonomously discovering that
  bid-ask-spread temporal dynamics (multi-window rolling means/stds) were the most useful feature
  family for that task, through iterative hypothesis-conclusion loops rather than being told this
  upfront.

> [!inferred] Reading the two papers together, RD-Agent's contribution is less about a single novel
> algorithm and more about **making the Research/Development boundary a first-class, swappable
> interface**: the same "propose a hypothesis, implement it, get feedback, decide what to try next"
> loop is instantiated once generically (six components, MLE-Bench) and once with domain-specific
> units bolted onto the same two phases (Specification/Synthesis/Implementation/Validation/Analysis,
> Qlib backtesting) for quant finance. The bandit-based **factor-vs-model** scheduling in RD-Agent(Q)
> is a concrete instance of the general framework's "FC-Planning" component (deciding *where* to
> spend the next iteration's budget), specialized to a two-armed action space.

## Cross-references
- `wiki/topics/autoresearch.md` — RD-Agent belongs in an "industrial R&D loop" section: unlike
  academic AI-scientist systems that target novel scientific discovery, RD-Agent targets routine,
  repeatable MLE/quant-research labor with a hard split between idea generation and implementation.
- `wiki/concepts/research-development-loop.md` — the six-component Research/Development
  decomposition and the `Algorithm 1` R&D-loop formalization live here.
- `wiki/concepts/closed-loop-experiment-design.md` — the Analysis Unit's feedback into Synthesis
  (general paper) and the bandit-scheduled factor/model feedback loop (RD-Agent(Q)) are both
  instances of a closed hypothesis → implementation → validation → feedback loop.

## Sources
- [`raw/papers/rd-agent.pdf`](../../raw/papers/rd-agent.pdf) — arXiv:2505.14738v2 (also the target of
  the `aka.ms/RD-Agent-Tech-Report` redirect used on the GitHub repo).
- [`raw/papers/rd-agent-quant.pdf`](../../raw/papers/rd-agent-quant.pdf) — arXiv:2505.15155v2, NeurIPS
  2025.
