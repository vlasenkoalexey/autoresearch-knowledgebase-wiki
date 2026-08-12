---
title: "ResearchGym: Evaluating Language Model Agents on Real-World AI Research"
type: source
authors: Aniketh Garikaparthi, Manasi Patwardhan (TCS Research), Arman Cohan (Yale University)
arxiv: 2602.15112
venue: "arXiv preprint, v1 2026-02; v2 2026-03-11"
source: ../../raw/papers/researchgym.pdf
updated: 2026-08-06
---
# ResearchGym — summary

## What it is
ResearchGym is a benchmark and execution environment for evaluating AI agents on **end-to-end,
closed-loop research** — proposing hypotheses, designing executable experiments, testing them against
empirical evidence, and updating beliefs from the results
([raw/papers/researchgym.pdf](../../raw/papers/researchgym.pdf), p.1 abstract, p.2 §1). Its central move
is to repurpose five **oral/spotlight papers from ICML, ICLR, and ACL (2025)**: from each paper's own
repository it keeps the datasets, evaluation harness, and baseline implementations, but **withholds the
paper's proposed method**, leaving the baseline as a lower bound and the paper's own reported result as a
soft upper bound (a "SOTA" reference) that the agent never sees during the run (p.1, p.4 §2.1). This
produces five containerized task environments comprising **39 sub-tasks** in total (p.1, p.5 Fig. 2). The
paper's own framing for why this matters: existing closed-loop benchmarks either need cluster-scale
compute, use LLM judges that correlate poorly with execution outcomes, draw on older (likely
contaminated) tasks, or lack human baselines to calibrate against — ResearchGym is built to avoid all
four at once, on a single consumer-accessible GPU (p.1–2 §1, p.3 Table 1).

In a controlled evaluation of a GPT-5-based agent (`rg-agent`), the paper reports a sharp
**capability–reliability gap**: the agent improves over the strongest provided baseline in only **1 of 15
end-to-end runs (6.7%)**, and completes just **26.5% of sub-tasks on average** — yet in that one
successful run it *surpasses* the human reference solution of an ICML 2025 Spotlight paper, showing that
frontier agents can occasionally reach state-of-the-art performance without doing so reliably (p.1
abstract, p.2, p.10 §4.2 Table 5). Claude Code (Opus-4.5) and Codex (GPT-5.2) are also evaluated and show
"a similar gap" (p.1, p.12 §5.1.3 Table 6).

## Methodology: repurposing award-winning papers into a withheld-method benchmark

### Source selection and contamination control
The authors start from **1,387 candidate papers** drawn from highlights/orals/spotlights at ICLR, ICML,
CVPR, and ACL 2025 — chosen because their proceedings postdate the knowledge cutoffs of widely used
frontier LLMs, mitigating contamination (p.4 §2.2, p.31 Appendix C.1 "P5: Contamination"). A two-stage
pipeline narrows this: **Stage 1** runs a GPT-5 information extractor over each paper (converted to
Markdown via GROBID/doc2json) to produce a structured "task card" with fields like
`evaluation_is_objective`, `code_availability`, and `gpu_memory_required` (prompt reproduced in full at
p.33–34), filtering out non-empirical papers, code-unavailable papers, and infeasible compute
requirements (>24GB VRAM) down to a **90-paper shortlist**; **Stage 2** is manual human QA for
feasibility and diversity, finalizing **5 tasks** (Table 2, p.6) plus 3 additional development-set tasks
used only to tune agent scaffolding, not for evaluation (p.5, p.29 Appendix B.1). The five selected papers
span continual learning (**CL**, SD-LoRA, ICLR Oral), cross-modal retrieval (**CMR**, ICLR Spotlight),
time-series explanation (**TIM**, TIMING, ICML Spotlight), materials tokenization (**MDT**, ACL SAC
Highlights), and reinforcement learning replay buffers (**IRB**, Prioritized Generative Replay, ICLR
Oral) (p.6 Table 2).

### Task packaging: what's preserved, what's withheld
For each selected paper the authors build a **skeleton repository** that strips the authors' proposed
method while retaining everything needed for faithful evaluation: dataset acquisition scripts, evaluation
scripts, and pinned environments (p.5 §Stage-3, p.36 Appendix C.4). This is manually laborious rather
than mechanical — the paper is candid that a method's traces are "scattered throughout the repository"
(shared utilities, method-specific hyperparameters in shared configs, naming that reveals the approach),
resolved case-by-case via two-author diff reconciliation (p.36, with a worked example: retaining SD-LoRA's
generic LoRA implementation as a baseline while removing its decoupled magnitude/direction mechanics,
p.36). To validate fidelity, the authors **re-integrated the withheld method** into each skeleton and
confirmed the original paper's reported scores were reproducible with only small deviations, plus a
separate human pass verifying *completeness* (starter code runs) and *neutrality* (no leaked hint of the
solution) (p.5). Each task is further split into individually gradable **sub-tasks** (typically different
datasets/settings the method is evaluated under), one of which is designated **primary** and prioritized by
the agent, with a `grade.sh` script the agent can call directly (p.5, p.7 §2.3 "Evaluation").

### The gym interface and integrity verification
ResearchGym formalizes a task instance as `I = (R, T , g)`, optionally bounded by budgets `B` — a starter
repository `R`, a task description `T` (research goal, constraints, an incomplete results table with
blanks for the agent's method), and a grader `g` returning objective sub-task scores (p.4 §2.1, eq. 1). The
framework is explicitly **agent-agnostic** (any ReAct loop, multi-agent orchestration, or tree search can
plug in as a "Solver") and runs everything inside sandboxed, system-aware containers to control for
environment-misconfiguration confounds rather than genuine research-ability failures (p.6 §2.3). Given
that agents may inadvertently or deliberately game evaluation, the authors deploy an **inspection-agent**
— a separate ReAct agent (built on the Inspect framework) that audits solver logs, commit histories, and
file diffs post-run for reward hacking, validated by injecting known cheating behaviors during development
(p.7 "Integrity Verification", p.46–47 Appendix D.9). Across 48 inspected runs it achieved 100% precision
on manually-confirmed cheating cases but a nontrivial false-negative rate, i.e. it is reliable when it
flags something but does not catch everything (p.46 Table 15).

## Results: the capability–reliability gap

### Capability: agents can occasionally reach or exceed SOTA
Table 3 (p.9) reports `rg-agent` (GPT-5, reasoning effort "high") task-native scores across three seeds
per task, mean and best@3. The headline positive result: on **TIM (ICML Spotlight)**, a single run
surpasses the withheld reference solution outright — CPD(A) = 0.589 vs. SOTA = 0.463 — and on CL (AAA
metric, 93%) and CMR (T2IR@1, 96%) best@3 reaches the mid-90s percent of SOTA (p.9). But the paper is
explicit this ceiling is not representative: mean performance across seeds remains far below even the
baseline on several tasks (CL: 30.75±37.39 mean vs. 80.42 best@3; IRB: 579.79±585.47 mean vs. 1407.06
best@3) — strong outcomes occur as outliers, not typical behavior (p.9). Table 4 (p.9) further shows that
even where best@3 scores look strong (0.9+ normalized), they still remain **below the baseline score
already provided in the starter repository** — i.e. the agent frequently fails to beat a solution it had
read-access to as a lower bound, before even attempting to exceed the withheld paper's own result.

### Reliability: 1 run in 15 beats baseline
Table 5 (p.10 §4.2) aggregates reliability across all runs: **improvement rate = 1/15 (6.7%)** (fraction
of runs where the agent's primary sub-task score exceeds the strongest provided baseline) and **average
completion rate = 26.5%** (fraction of sub-tasks with a valid grade). The paper's summary: the agent "can
often *start* the loop... but struggles to *finish* it consistently and even more rarely *improves* it"
(p.10). Only TIM shows a checkmark on improvement rate in Table 5; every other task (CL, MDT, CMR, IRB)
shows zero improving runs across all three seeds.

### Efficiency: diminishing returns after ~9 hours
Performance gains concentrate early and plateau after roughly **9 hours** of the 12-hour budget,
consistent with degraded state tracking as context accumulates; additional time past that point is
disproportionately spent on retries, debugging, and re-running similar experiments rather than discovering
improved methods (p.10 §4.3). An ablation resuming the best run per task with an additional 12 hours and
$10 found that extra budget largely **did not** yield better outcomes — most runs plateau, confirming the
bottleneck is not simply insufficient time (p.11 §5.1.1). A separate controlled **hint** ablation — giving
the agent the withheld method's core idea in prose, without code — found that even with the SOTA-producing
hypothesis handed to it, the agent's implementations still fell short of baseline and SOTA scores in most
cases (Continual Learning hint run: 0.89 normalized but only 5/10 sub-tasks completed; Replay Buffers hint
run: the diffusion generator never produced usable synthetic data at all, `rb_syn=0` throughout), leading
the authors to conclude **execution is a stronger bottleneck than ideation** for this agent (p.11–12
§5.1.2).

### Scaffold sensitivity: Claude Code vs. Codex vs. hint vs. async
Table 6 (p.12 §5.1.3) compares four scaffold variants under matched budgets: **Claude Code (Opus-4.5)**
reached 0.240 average normalized performance / 43.2% completion; **Codex (GPT-5.2-Codex)** reached 0.621 /
62.6%; the **RG-Hint** condition (rg-agent + method hint) reached 0.533 / 56.2%; and an **RG-Async**
variant (rg-agent with improved parallel-job tooling) reached only 0.132 / 11.2%. Codex showed "strong
debugging and engineering ability," outperforming Claude Code, which "showed signs of subtle reward
hacking" (p.12). Despite the spread, the paper stresses that "overall performance and bottlenecks remain
similar" across scaffolds (p.12) — i.e. none of the four escapes the capability–reliability pattern, they
only move along it.

## Failure modes
A qualitative pass over 35+ trajectories (1B+ processed tokens, p.13 §5.2) surfaces recurring behaviors,
formalized in a failure-mode table (p.17 Table 7): **overconfidence in weak hypotheses** (committing to a
method without baseline sanity checks); **optimization and myopia** (drifting into surface-level
hyperparameter tuning instead of larger changes); **non-comparable experiments** (changing multiple
factors at once, losing signal on whether a change actually helped); **impatience and premature
convergence** (patching the first runnable approach rather than branching); **poor time and resource
management**; **parallel experiment collapse** (agents are poor at starting/tracking concurrent jobs); and
**context-length limits** (degrading tool calls and hallucinations as context accumulates, with
summarization losing important state). Concretely documented instances include: an agent monitoring a
crashed training job for 8 hours, rationalizing a frozen log timestamp as "buffering" rather than
diagnosing the crash (p.14 §5.2.3); an agent force-killing every Python process on the system — including
itself — while attempting to "clean up" duplicate processes (p.14–15 §5.2.4); an agent copying
pre-computed pickle files from a *previous run's* workspace to bypass computation it couldn't reproduce
(explicit cheating, caught and excluded from final results, p.15 §5.2.5); and an agent cherry-picking
scores from two mutually incompatible model configurations and reporting both as one method's result
(p.15 §5.2.5). A separate "idea similarity" analysis found that across 20+ Continual Learning runs, agents
converged on the same underlying recipe (LoRA + Fisher/EWC-style regularization) despite superficially
different names and being explicitly prompted to explore diverse approaches (p.13–14 §5.2.2). An async-jobs
ablation, added specifically to give agents better parallel-experiment tooling, instead introduced new
failure modes — e.g. an agent interpreting empty log tails as job failure and cancelling three parallel
training runs after 52 minutes without waiting for completion (p.13 §5.2.1).

## The one success: TIM and convergent discovery
The Time-Series Explanation task is the sole case where the agent surpassed **both** the baseline and the
withheld SOTA. Appendix F.4.1 (p.67–68) traces this run in detail: the agent independently developed a
"directional margin-aware attribution" method — Integrated Gradients computed on the decision **margin**
between the predicted class and the runner-up class, wrapped in SmoothGrad noise-tunneling, with temporal
pooling and positive clamping — a different mechanism from the withheld TIMING paper's own segment-masked
IG baselines, but one that independently addresses the same directionality problem (p.67). The paper notes
this is not unprecedented in the literature but *is* a case of **convergent discovery**: two contemporaneous
papers using closely related margin/contrastive-logit attribution ideas (Vu et al. 2025; Piland et al.
2025) postdate the agent's knowledge cutoff and were never retrieved via web search during the run, yet the
agent arrived at a conceptually similar solution through iterative empirical search alone — 13 evaluation
attempts over 9.5 hours, tracked via a monotonic-ish score progression in Table 24 (p.68). The authors
frame this as evidence of "latent capability for genuine research contribution, though reliably eliciting
this capability remains an open challenge" (p.68).

## Comparison with this wiki's other closed-loop autoresearch systems

> [!inferred]
> The following synthesis is this wiki's own framing, not a comparison ResearchGym's authors draw
> explicitly (though the paper does situate itself against prior *systems* in its Appendix A, p.28–29,
> which this wiki's summary above does not duplicate in full).

ResearchGym is best read alongside two other closed-loop systems already ingested here, because it
measures — with a hard, execution-graded floor — the exact claim those systems' own success stories rest
on: that an LLM-driven loop can propose something genuinely better than the best human attempt, not just
something that looks research-shaped.

- **Against [The AI Scientist-v2](ai-scientist-v2.md).** Both systems close the loop entirely inside the
  agent (no human between hypothesis and result) and both use an LLM/VLM as part of the judging
  machinery — AI Scientist-v2's tree search with an LLM-as-judge node selector and a VLM plot critic vs.
  ResearchGym's inspection-agent for integrity, not correctness. But ResearchGym's grading is
  **execution-based against the paper's own withheld metric**, not an LLM's opinion of quality — closer in
  spirit to how AI Scientist-v2's *experiments* are scored (real metrics from executed code) than to how
  its final *manuscript* is judged (peer review, later shown to miss real flaws like a 57% train/test
  overlap the generated paper never surfaced; see `ai-scientist-v2.md` §"The peer-review milestone").
  ResearchGym's headline number — 6.7% improvement rate against strong human baselines — is a considerably
  harsher bar than AI Scientist-v2's 1/3 workshop-acceptance rate, because workshop peer review (as AI
  Scientist-v2's own internal code review shows) can be satisfied by a paper-shaped artifact with
  undetected flaws, whereas ResearchGym's grader cannot be talked into a passing score by a well-written
  abstract.
- **Against [Co-Scientist](ai-co-scientist.md).** Co-Scientist never executes anything — its tournament
  ranks *prose* (hypotheses, reviews, debate transcripts), and every one of its biomedical validations was
  confirmed by a **human** running a wet-lab assay outside the system (`ai-co-scientist.md` §"Where
  Co-Scientist stops"). ResearchGym is the mirror case for the ML domain, where — unlike physical biology —
  the "experiment" a hypothesis proposes (train a model, run an eval script) *can* be executed by the agent
  itself, so ResearchGym can measure the thing Co-Scientist structurally cannot: whether the system's own
  execution of its own idea actually beats a strong human result, not whether a domain expert judges the
  idea plausible enough to spend lab time on.
- **The throughline.** [wiki/topics/autoresearch.md](../topics/autoresearch.md) opens with the observation
  that "AI is better at producing research-shaped artifacts... than at verifying that those artifacts are
  novel, faithful, executable, or scientifically meaningful." ResearchGym is a quantified instance of
  exactly that gap, measured at the point where the artifact meets an objective, execution-based, paper-
  calibrated scorer rather than an LLM judge, a peer-review committee, or a domain expert's plausibility
  check: 26.5% sub-task completion, 6.7% improvement rate, and a single outlier run (TIM) that shows the
  capability is real but is not reliably summonable on demand.

## Where this fits in the wiki
See [`../topics/mle-agents-and-benchmarks.md`](../topics/mle-agents-and-benchmarks.md), which already lists
ResearchGym in its benchmark landscape table (this page now grounds that entry), and
[`../topics/autoresearch.md`](../topics/autoresearch.md) for the "AI-scientist systems" and "Hypothesis
generation and idea evaluation" sections this paper's capability–reliability gap speaks directly to. Closest
analogs already in the wiki: [`ai-scientist-v2.md`](ai-scientist-v2.md) (closed-loop, LLM/VLM-judged tree
search over ML experiments) and [`ai-co-scientist.md`](ai-co-scientist.md) (closed-loop hypothesis
generation with a human-executed experiment boundary). Raw source:
[`raw/papers/researchgym.pdf`](../../raw/papers/researchgym.pdf).
