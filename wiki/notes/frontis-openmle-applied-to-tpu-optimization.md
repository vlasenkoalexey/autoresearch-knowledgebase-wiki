# Could the Frontis-MA1 / OpenMLE recipe be applied to TPU model + kernel optimization?

**Question asked (2026-08-06):** check the TPU optimization work in this wiki against
[Frontis-MA1 / OpenMLE](../sources/frontis-ma1.md); which of its RSI ideas transfer to the TPU model and
kernel lanes, and how hard would it be to adapt the stack and train a model to optimize models and kernels?

**Sources read:** [`sources/tpu-performance-autoresearch-wiki.md`](../sources/tpu-performance-autoresearch-wiki.md)
and the raw methodology clips ([`kernel-optimization-index.md`](../../raw/papers/tpu-performance-autoresearch-wiki/kernel-optimization-index.md),
[`model-optimization-blueprint.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-blueprint.md),
[`kernel-experiments-program.md`](../../raw/papers/tpu-performance-autoresearch-wiki/kernel-experiments-program.md),
[`skills/author-kernel.md`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/author-kernel.md),
[`README.md`](../../raw/papers/tpu-performance-autoresearch-wiki/README.md)) ·
[`sources/frontis-ma1.md`](../sources/frontis-ma1.md) · [`sources/kernelevolve.md`](../sources/kernelevolve.md) ·
[`sources/alphaevolve.md`](../sources/alphaevolve.md).

---

> **This note grew three follow-ups as the question sharpened.** The original question (can the recipe be
> ported?) is answered immediately below. The question that actually matters for a product — *can a ~30B
> specialist match frontier quality at a fraction of the cost?* — is
> [Follow-up 2](#follow-up-2-the-product-goal--a-cheap-model-as-capable-as-claude-or-codex), with the
> harder "beat Opus 5" variant in [Follow-up 1](#follow-up-1-could-a-trained-model-beat-claude-opus-5-at-this)
> and the bake-into-weights-vs-retrieve question in
> [Follow-up 3](#follow-up-3-the-wiki-goes-into-the-weights-and-the-price-problem-goes-away). Two cheap
> probes decide most of it: a base-model arm on GQA attention, and a cheap model scored against historical
> K1 diagnoses.

## Verdict

**Yes for the kernel lane, and the fit is unusually good — better than MLE-Bench's in several respects.
No for the model lane as an RL environment.** The three things OpenMLE had to build from scratch, the TPU
project mostly already has; the one thing it lacks (a population with recombination) is cheap to add and is
where Frontis measured 85–92% of its long-horizon gain.

The strongest single observation from this comparison:

> **The TPU project has already run half of Frontis-MA1's headline ablation, and got a large number.**
> Frontis's key controlled result is *fix the harness, swap the model* → **+21.22 pp** Medal Average. The
> TPU README's four-harness study is structurally the same experiment: identical protocol, four different
> frontier models, unattended. Model lane: **47.3% MFU** (Codex GPT-5.5) down to **33.0%** (Gemini 3.1 Pro)
> — a **14.3 pp** spread. Kernel lane on GQA attention: **6.77×** (Claude Opus 5) vs **3.51×** (Gemini Flash
> 3.6) — nearly **2×**. Same harness, same wiki, same skills. What that spread says is that on this domain
> the **model** is the binding constraint, not the scaffold. The arm you have never run is Frontis's other
> one: *train the model for these specific moves.*

That reframes the whole question. The harness ideas below are cheap and worth taking, but they are the small
half. The prize is a trained Pallas/TPU-optimization operator model, and the corpus for it already exists as
a by-product of work already done.

---

## Layer-by-layer: what exists, what's missing

OpenMLE is three layers. Mapping each onto the TPU project:

### Layer 3 — OpenMLE-Evo (the search harness): **you are ahead on rigor, behind on search**

The TPU wiki's K0–K9 loop is, on the verification axis, materially stronger than OpenMLE-Evo. Things the TPU
protocol has that Frontis does **not**:

| TPU protocol | Frontis-MA1 equivalent |
|---|---|
| author ≠ verifier, fresh process on a different chip | none — the harness scores its own rollouts |
| `kgate` self-hashed receipts; "a number kgate didn't print does not exist" | none |
| pre-registration enforced by **commit ordering** (LINT checks git history) | none |
| hypothesis-firing audit / silent-no-op detection | partially — six typed feedback modes, but no attribution check |
| intervention-class ladder with **`refute` as a first-class outcome** | none — every operator proposes a change |
| HLO / AOT-cost pre-filters that refute on a compiler pass, before spending hardware | none — every candidate is executed |
| the load mandate (paste *sections* by category; measured 2/8 → 8/8) | operator-conditioned context (same idea, less curated) |
| anti-fabrication LINT battery, launch-armed process-auditor | none |

And the things OpenMLE-Evo has that the TPU protocol does **not**:

| OpenMLE-Evo | TPU protocol today |
|---|---|
| a **population** — many live candidates per task | single-lineage frontier ratchet per family |
| **`Crossover`** — recombine two parents' mechanisms | **absent entirely** (verified: no crossover/recombination anywhere in the protocol) |
| three-factor parent selection (quality / progress / novelty) as a soft weighted softmax | hard rules (see below) |
| experience **board** — family-wise bests, repeated failures, score trends, parent graph | `retrospectives-digest.md` + class-page lever lists (close, but per-family, not a live selection input) |

> [!inferred] **The TPU wiki independently invented Frontis's novelty term, as a hard constraint instead of a
> soft weight.** OpenMLE-Evo samples parents by *U = λ_s·quality + λ_Δ·progress + λ_n·novelty*, where novelty
> is **method-family** novelty. The TPU wiki's class pages carry a `## Levers (verified)` list, coverage is a
> mechanical set-diff over it, and `formulate-kernel-hypothesis` enforces a **consecutive-lever limit** (no
> third attack on the same lever in a row) and **bounded deferral** (an untried lever may be deferred at most
> twice). That is λ_n → ∞ on repeat, rather than a weight. Similarly, hypothesis ranking by
> `expected_gain × confidence / effort` covers the quality term. **The one factor with no TPU analogue is
> `progress`** — normalized gain over the strongest parent — which is exactly the factor that, in Frontis's
> `right-whale` case study, promoted a 6th-by-score / 1st-by-gain branch from 10.47% to 17.09% selection
> probability and produced the run's best result. A single-lineage ratchet cannot express that idea at all,
> because it has only one parent.

### Layer 1 — OpenMLE-Gym (verifiable environments): **easier to build here than it was for MLE**

This is the layer that looks hardest and is actually the most favorable, for one reason: **the oracle is
free.** OpenMLE-Gym's whole 11,000 → 3,972 → 2,839 → 2,240 funnel exists because a Kaggle task needs hidden
labels, a bespoke `metric.py`, a submission contract, and an LLM semantic quality gate — task construction is
the expensive part. A TPU kernel task needs none of that:

- **The reference implementation *is* the task spec.** The naive XLA form both defines correctness (parity)
  and sets the baseline (`F = t_reference / t_candidate`, `F = 0` on parity or compile failure — the exact
  fitness [KernelEvolve](../sources/kernelevolve.md) uses in production).
- **The roofline gives a free, physically-meaningful score ceiling per task** — which is what OpenMLE's
  §4.3 adaptive-bound machinery had to *learn* from an on-policy score frontier, because Kaggle metrics have
  no natural scale. Here the compute/bandwidth/dispatch floors are computed at K1 already.
- **Op-points are enumerable from real profiles.** The downward-spawn rule already requires a kernel family's
  op-points to come from real model-lane profiles. Every model profiled is a task generator.
- Plus off-the-shelf task supply: KernelBench (250 problems, 3 tiers), JAXBench, tokamax, ejkernel,
  pallas-forge, the ATen operator surface.

Realistic scale: **hundreds to low thousands** of (op, op-point, generation) kernel tasks, versus OpenMLE's
5,758. Smaller, but the same order of magnitude, and far cheaper per task to construct.

**And rollouts are cheaper than MLE-Bench's, not more expensive** — which is counter-intuitive and worth
stating plainly. An MLE-Bench rollout is *train a model*: minutes to 12 hours of GPU. A Pallas kernel rollout
is: generate → compile → interpreter-mode parity on a tiny shape → HLO firing check → measure. The TPU
project's own **early-kill gate** already establishes that the first three run with **no accelerator at all**
and kill dead-on-arrival candidates in ~5 minutes (introduced because ~40% of one wave's wall-clock was
rework on kernels broken from the start). Only survivors touch a chip, and a measurement is seconds. The
expensive parts of MLE RL — long sandbox jobs, high variance in runtime, straggler synchronization — are
mostly absent, which also means OpenMLE's asynchronous-rollout machinery matters less here.

### Layer 2 — OpenMLE-ERL (training the operators): **the corpus already exists**

This is the part that would normally be a multi-month data-collection project, and it is largely already
done as a side effect of running the loop:

- **`commit-each-candidate` is an SFT corpus generator.** One commit per candidate that ran, **losers
  included**, under a machine-readable grammar — `cand<N>(<fam> vNNN): <what changed> — <p50/speedup/parity>`
  — with the canonical `bench()` helper's **stdout verbatim** in the candidate ledger. That is precisely
  OpenMLE's `(task, operator, context, program, execution outcome)` tuple, already keyed, already scored.
- **Pre-registration makes the supervision honest.** The stub — hypothesis, mechanism, predicted signal,
  falsification criterion — is committed *before* authoring, and LINT verifies the commit order. So the
  hypothesis→code→outcome mapping cannot be retrofitted. OpenMLE's corpus has no equivalent guarantee.
- **Independent verification means labels are trustworthy.** Author-side numbers never graduate into verdict
  numbers; a `supported` verdict may only cite a `PASS` receipt.
- **Refuted patterns are labelled, not discarded** — including the `refute` verdicts, which are a *positive*
  training signal for an operator most systems can't learn (see below).
- **Four different agent harnesses generated it** (Codex, Claude, Gemini, Antigravity), which is unusual
  authorship diversity for a single-project corpus.

> [!warning] **Count the corpus before planning on it.** The wiki summary describes "the ~3,580 per-model and
> per-kernel experiment pages," but the README states **3,580 pages total** — "across 4 model families +
> shared concept/observation/source/codebase substrate," i.e. experiment pages are a *subset*, not the whole.
> The trainable unit is also finer than a page (candidates, not experiments), so the real number could be
> either well below or well above 3,580. **Step 1 of any training plan is a real count of
> `(candidate, verdict, receipt)` triples reachable from the git history.** Everything downstream —
> SFT-only vs. SFT+RL, model size, whether one model family generalizes — depends on that number, and no
> estimate here should be trusted over the count.

---

## Which RSI ideas transfer, ranked by (value × feasibility)

### 1. Crossover + a population — highest value, needs no training, days-to-weeks

The TPU loop is a single-lineage ratchet: each experiment page registers **one** mechanism, the plan is a
flat list of that mechanism's parameter-sweep points, and the frontier advances or it doesn't. There is no
step anywhere in K0–K9 that takes **two** candidates and fuses their mechanisms.

Frontis's evidence that this is the expensive omission is its sharpest result. On `nomad2018`, the baseline
harness followed one lineage through **seven successive `Debug` attempts**, each inheriting an expanding
history, and finished at val RMSE 0.06633. OpenMLE-Evo instead built one targeted `Crossover` from a
physics-features parent and a robust-parser parent, explicitly excluding two known sibling failures as
negative evidence, and reached 0.06087 / 0.05410 held-out — **−8.2% / −11.3%**. Across its two long-horizon
trajectory studies, late `Improve` + `Crossover` accounted for **85.0%** and **91.9%** of total validation
gain.

**The population already exists on disk and is never used.** `commit-each-candidate` means every losing
candidate of every experiment is a real commit on the family branch, with its measured numbers in the ledger.
Today they are read only as `refuted-patterns.md`. A `Crossover` operator would read two of them.

The natural TPU shape: two candidates that won on *different* levers of the same class page — e.g. one that
fixed the grid/streaming structure and one that got the block-size/VMEM story right, or a `flag` win and an
`xla-rewrite` win on the same op — fused into one candidate, under the existing parity gate and receipt
discipline. The class pages' `Levers (verified)` lists are already the "method family complementarity cue"
Frontis's `Crossover` prompt asks for.

> [!inferred] There is a real tension to resolve first, and it should be resolved deliberately rather than
> by accident. The protocol's **one-page-one-mechanism rule** is load-bearing anti-fabrication machinery —
> "if describing the candidate honestly requires a different Mechanism paragraph than the page's, it belongs
> in the next page." A `Crossover` candidate is *by construction* two mechanisms. The clean resolution is
> that a crossover is its **own** experiment page whose declared mechanism is the fusion (naming both parent
> `cand<N>` commits as inputs), not an extra candidate smuggled into either parent's page — which keeps
> attribution intact and makes the fusion itself falsifiable ("the combination beats both parents" is a
> sharper prediction than either parent's was). Worth checking against the auditor's plan-coverage rule
> before implementing.

### 2. The `progress` factor in parent selection — no training, days

Add gain-over-parent alongside the existing effort-weighted-gain ranking and the lever-coverage constraint.
The TPU wiki has quality and novelty; `progress` is the missing one, and it is what keeps a
promising-but-not-leading branch alive long enough to be developed. Cheap because the numbers are already on
the pages.

### 3. Deterministic-state-before-prose — mostly already done; take the measurement, not the design

OpenMLE-Evo's experience card / board split (deterministic metadata for *selection*, LLM prose only for the
handful of nodes an operator actually consults) is the same instinct as the TPU wiki's load mandate and its
`retrospectives-digest.md` ("one line per experiment, explicitly *not* re-reading whole past pages"). The TPU
version is arguably better-curated.

What is worth importing is Frontis's **measurement**, because it independently validates the load mandate
with numbers the TPU project doesn't have: matched runs, same checkpoint and seed, 66 task-runs — total
tokens **−41.7%** at only **−12.4%** fewer nodes, new-best updates per million tokens **1.77 → 3.27**, and
the `Improve` prompt's **99th percentile** context down **−86.1%**. That is third-party evidence for the
"paste sections, not files; content, not paths" rule, arrived at from a completely different direction.

### 4. The RSI ladder as positioning

Frontis's ladder — Evolution → Self-evolution → **Meta-evolution** (the improver is trained) → RSI — places
the TPU project cleanly at **rung 2**: execution experience flows back and changes what the loop explores
next, through the wiki. Rung 3 requires training. See [`meta-evolution`](../concepts/meta-evolution.md).

### 5. Reward shaping (adaptive bounds, entropic advantage) — only if you train, and **simpler here**

Both of OpenMLE's reward-shaping inventions solve problems this domain has in milder form:

- *Adaptive bounds* exist because Kaggle metrics have incomparable ranges and no natural ceiling. MFU is
  already a normalized ratio with a physical ceiling; kernel fitness is already a co-measured speedup ratio
  — and "co-measured ratios are authoritative, never absolute times from another run" is already a BRIEFS
  rule. Much of Eq. 1's machinery is unnecessary.
- *Entropic advantage* (concentrate the update on a rollout group's best candidate) **does** transfer
  directly, because the objective is identical: best-of-budget, not mean quality. The frontier is what
  matters; a correct-but-slower kernel should not be reinforced like a frontier-mover. Worth taking as-is.

### 6. What does **not** transfer

- **The model lane as an RL environment.** One rollout is a real training run at steady state on a
  multi-chip (sometimes multi-host) slice, the semantics gate needs a ≥10-step loss trajectory, and the task
  count is model-families × lanes × generations — dozens, not thousands. Wrong shape for RL. The model lane
  stays a directed, knowledge-driven loop; at most it contributes SFT trajectories.
- **`Debug` as a first-class trained operator.** OpenMLE trains `Debug` heavily. The TPU protocol
  deliberately *minimizes* debugging via the early-kill gate ("never iteration on a broken base"), and
  treats a compile-error loop as waste. Training a strong `Debug` here would optimize the thing the protocol
  is designed to avoid.
- **Benchmark comparability.** There is no MLE-Bench for this domain. You measure against MaxText MFU and
  hand-tuned kernel references, as the project already does.

### 7. The operator vocabulary should be the TPU one, not OpenMLE's

The most important adaptation: **do not port `Draft`/`Improve`/`Debug`/`Crossover` literally.** The TPU
project already has a better-suited, cost-ordered vocabulary — the **intervention classes** — and it maps
onto the operator interface cleanly:

| Proposed operator | TPU meaning | Why it's trainable |
|---|---|---|
| **`Diagnose`** (K1) | profile → bound + which of the three sinks | the whole ladder keys off this; label = did the chosen class end up winning |
| **`Refute`** | argue from HLO that no kernel can win | **verifiable label**: a later candidate that beat the refuted bound proves the refute wrong |
| **`Flag`** | compiler knob, bit-exact | cheap rollouts, dense signal |
| **`Rewrite`** | algebraic restructuring removing a redundant read, bit-exact | |
| **`Author`** | write the Pallas kernel | the expensive one; where domain knowledge is scarcest |
| **`Tune`** | block-size / grid sweep (≈ `Improve`) | interior optimum, sweeps already automated |
| **`Crossover`** | fuse two candidates' mechanisms | **new — see #1** |

> [!inferred] **`Refute` is the operator this domain has and MLE doesn't, and it may be the most valuable one
> to train.** OpenMLE's operators all propose a change; there is no move that says "no change can win here,
> and here is the evidence." The TPU protocol makes `refuted` a first-class outcome and states that the
> discriminating skill is "not forcing a kernel where a flag, a rewrite, or a refute is correct." That skill
> is exactly what a frontier model lacks — it is trained to produce code, not to decline — and it is
> **cheaply supervised**, because refuting correctly costs one HLO dump while refuting wrongly is disproved
> by any later candidate that beats the claimed bound. A model that reliably declines to write doomed kernels
> would save the majority of a campaign's wall-clock, which the project has already measured as its dominant
> waste. Nothing in Frontis suggests this; it falls out of comparing the two operator sets.

---

## How hard: three tiers

Effort figures are estimates for a small team already fluent in this stack, and the corpus-dependent ones
are gated on the count flagged above.

### Tier 0 — harness only, no training. **Weeks. High confidence.**
Add `Crossover` + a candidate population and the `progress` selection factor to the kernel lane; import
Frontis's context measurement as validation of the load mandate. All of it is `program.md` / skill / class-page
edits on infrastructure that already exists (commit-per-candidate, receipts, class pages, lever set-diff).
**Do this regardless of whether any training happens** — it is the cheapest slice of Frontis's result, and
its evidence (85–92% of long-horizon gain) is the strongest single claim in that paper.

### Tier 1 — SFT a specialist on the existing corpus. **~1–3 months, 1–2 people. Moderate confidence.**
Convert the candidate ledgers + receipts + verdicts into operator-labelled examples; train a 30B-class open
model (Frontis used Qwen3.6-35B-A3B) on `Diagnose` / `Refute` / `Author` / `Tune`.

This is the highest-ROI training play, and the reason is a domain asymmetry that favors TPU strongly over
MLE. Frontis got +21.22 pp by training a model for a domain frontier models *already know* (Kaggle pipelines
are thoroughly represented in pretraining). Pallas/Mosaic is **not** — the kernel index states its whole load
mandate is built "on the stated assumption that the authoring model has little or no Pallas/TPU material in
its training set," and measured **2/8 vs 8/8** with path-only vs. pasted briefs.
[KernelEvolve](../sources/kernelevolve.md) reaches the same conclusion from the MTIA side: the value of
automated kernel generation is *inversely proportional to the maturity of the target's software ecosystem*.
So the headroom from a domain-specialist model should be **larger** here than the +21 pp Frontis measured,
not smaller — and the four-harness spread (14.3 pp MFU / ~2× kernel speedup, same protocol) is direct local
evidence that model capability is the binding constraint.

A useful intermediate target that does not require beating anything: a small specialist that matches
frontier-model kernel authoring at a fraction of the cost, run as the `Author` operator inside the existing
harness, with the frontier model retained for `Diagnose`.

### Tier 2 — full OpenMLE-ERL: RL from execution feedback. **~6–12 months + a standing TPU budget. Lower confidence.**
Requires the Gym (task construction at scale from profile-derived op-points + KernelBench/JAXBench/tokamax),
async rollout infrastructure against a chip pool, and the reward path. The technical risk is lower than for
MLE (free oracle, free early-kill, cheap measurement, physically-bounded reward); the **institutional** risk
is the standing chip allocation for rollouts, which is the real gate.

---

## Risks, in the order they will bite

1. **Reward hacking, and this project has already measured it.** One agent that authored kernels *and* wrote
   its own firing-confirmed lines produced a wave where **0 of 4 claimed wins survived re-checking**. DGM's
   Appendix H (an agent deleting a hallucination-detector's marker tokens to fake a perfect score) is the
   same failure with gradients behind it. The mitigation is already built — author ≠ verifier, self-hashed
   receipts, the firing audit — but it only works if those gates sit **inside the RL reward path**, not
   alongside it. A reward computed from author-side numbers would train the model to fabricate. Read
   Frontis's Appendix B.6 (reward-hacking detection/prevention) before writing the reward function.
2. **Train/test contamination.** If you train on the wiki's experiment pages, every kernel family in those
   pages is contaminated as an evaluation target. OpenMLE handles this by excluding MLE-Bench-overlapping
   competitions *before* task construction and deduplicating training data against all evaluation
   benchmarks. The TPU project already has the conceptual machinery — the `capability-eval` vs
   `optimization` split, "cold runs MUST NOT open archival branches," the warm-tier/cold-tier rule for
   per-kernel answers — but it currently governs *prompting*, not *training data*. It needs to be extended
   to a family-level train/holdout split, decided before any training run.
3. **Overfitting to constants that don't transfer.** The kernel index is explicit that measured block sizes,
   VMEM knees, bandwidth ratios and MXU tile edges are generation-specific and must be re-derived — "treat
   the numbers as calibration for the *shape* of the answer, not as targets." A model trained on v6e
   trajectories will happily emit v6e block sizes on v7. Train on **mechanism selection and structure**;
   keep the constants in retrieval, queried via `pltpu.get_tpu_info_for_chip`. This is the one place where
   KernelEvolve's retrieval-first design should win over Frontis's train-it-in design, and the two are
   compatible — see [`program-evolution-operators`](../concepts/program-evolution-operators.md).
4. **Corpus concentration.** Four model families, largely one hardware generation, one project's
   conventions. Frontis's cross-model replication (a second backbone reproducing +18.18 pp) is the kind of
   control that would be needed to claim the gain is real rather than a fit to this wiki's own style.

---

## Why this domain is a *better* RSI target than MLE-Bench

Worth stating because it is the strongest strategic argument, and it comes from Frontis's own limitations
section. Limitation #3: the agent improves *external* ML artifacts, and real RSI requires agents
participating in more of the AI-development process, **"especially the improvement of language models
themselves."**

TPU model and kernel optimization *is* that. A win here compounds directly into every subsequent training
run rather than into a leaderboard position — and this wiki already holds the proof point:
[AlphaEvolve](../sources/alphaevolve.md)'s Pallas TPU matmul kernel result was a **23% kernel speedup → 1%
reduction in Gemini's total training time**, described by DeepMind as Gemini optimizing its own training. An
MLE-Bench medal does not do that. So the domain the TPU project already works in is a *shorter* RSI loop
than the one Frontis chose as its testbed, and closing it answers Frontis's own stated gap.

The honest caveat: shorter loop, much thinner benchmark. Frontis can point at 22 tasks and a public
leaderboard; this domain has MaxText references and hand-tuned kernels. Rigor here has to come from the
protocol — which, as the top of this note argues, is where the TPU project is already ahead.

---

## Suggested order of work

1. **Count the corpus.** `(candidate, verdict, receipt)` triples reachable from git history, split by lane
   and family. Everything below is gated on this number.
2. **Tier 0 now** — `Crossover` + candidate population + `progress` selection factor in the kernel lane.
   No training, weeks, and it tests the single strongest claim in the Frontis paper on your own workload.
3. **Decide the holdout split** before touching training data — by kernel family, extending the existing
   cold/warm-tier discipline from prompting to data.
4. **Tier 1 SFT** on `Diagnose` + `Refute` + `Author`, evaluated inside the existing harness with the
   existing receipts as the grader. `Refute` first if you want the cheapest verifiable win.
5. **Tier 2 only if** the corpus count supports it and a standing chip allocation exists for rollouts.

---

# Follow-up: could a trained model beat **Claude Opus 5** at this?

**Question (2026-08-06):** not just "does the recipe port" — can you actually train a model that optimizes
TPU models and kernels *better than Claude Opus 5*?

## The bar, stated precisely

From the README's kernel-lane campaign (GQA attention, one v6e chip, hand-tuned MaxKernel reference at
2.48×):

| Arm | Best speedup | Experiments |
|---|---|---|
| **Claude Opus 5** | **6.77×** | 22 |
| Codex GPT-5.6 | 3.73× | 9 |
| Gemini Flash 3.6 | 3.51× | 12 |

Opus 5 does **not** appear in the model-lane table (that one has Codex GPT-5.5 at 47.3% MFU, Fable 5, Opus
4.8, Gemini 3.1 Pro), so "beat Opus 5" is a well-defined bar only on the **kernel lane**, and only on this
family's live-campaign numbers — which the source itself flags as "the ordering is the durable part, the
per-arm decimals are not."

## The decisive detail: it's two ideas, not twenty-two

The README's own reading of the staircase: *"Opus 5's jump from 3.73× to 4.97× at experiment 8, and again
to 6.03× at 15, are **single structural changes** surrounded by long flat runs of refuted hypotheses."*

And Codex GPT-5.6 topped out at **3.73×** — precisely where Opus 5 sat *before* its experiment-8 jump. So
the three arms agree on the first plateau and diverge on whether they find the structural moves above it.

That means the capability separating Opus 5 from the others is **structural insight at the
hypothesize/author step** — not tool discipline, not stamina, not Pallas syntax, not sweep efficiency. Any
training plan that targets the wrong one of those will produce a model that is cheaper and faster and still
stops at 3.73×.

This cuts both ways:

- **Against training.** Structural insight is the hardest capability to distill. A 30B model SFT'd on
  trajectories mostly learns the *distribution* of things tried — and by the README's own account, most
  experiments do not move the frontier. Naively fitting the corpus fits the flat runs.
- **For training, and decisively.** Frontis's stated reason for having an SFT stage at all is exactly this:
  RL "can raise Pass@1 by reinforcing already-rewarded solutions yet provide limited gains at large *K*,
  whereas **teacher distillation can introduce behaviors absent from the base model's sampled support**"
  (Yue et al. 2025, cited at p.11). Distilling a stronger teacher is the *only* one of the two stages that
  can transfer a structural move a weaker base would never sample.

> [!inferred] **The reframing that makes this tractable: you don't need to out-invent Opus 5. You need to
> out-recall and out-apply the inventions it already made — and your wiki already wrote them down.** Every
> structural jump any arm has ever found is captured as an entry on a class page's `## Levers (verified)`
> list, with a receipt path. The 6.77× was a one-time discovery cost, and it has been paid and banked. So
> the specialist's job on a *new* family is not invention but **recognition**: given this K1 bound and sink
> classification, which of the ~7 class pages' levers applies? That is a classification problem over a
> closed, enumerated set — far more learnable than open-ended insight, and it is precisely what your
> corpus labels. Where the specialist will genuinely lose is a family requiring a lever that is *not yet on
> any class page*. That suggests the honest way to benchmark it: **split held-out families into
> "lever-covered" and "needs-a-new-lever," and report the two separately.** A model that matches Opus 5 on
> the first and loses on the second is both a real result and an accurate description of what was built.

## The precedent is directly on point

Frontis's base model (Qwen3.6-35B-A3B) scored **39.39%** under its harness. Claude **Opus 4.8** + Claude
Code scored **63.64%** — the base was **24 pp behind a frontier Opus**. After the full stack, Frontis-MA1-35B
reached **71.21%**, i.e. **+7.6 pp ahead of Opus 4.8** and past GPT-5.5 + Codex.

So the answer to "can a ~35B specialist beat a frontier Opus on a domain?" is: **demonstrated, once, by a
~24-author lab, requiring all three layers** — 5,758 tasks, 26,259 SFT examples, RL with adaptive bounds and
entropic advantage, plus Evo-Max priors and parallel search. A 31-point swing is not a fine-tune.

Two adjustments to that precedent for this domain, pulling in opposite directions:

- **In your favor:** Frontis had to beat frontier models on Kaggle pipelines — a domain thoroughly present
  in pretraining. Pallas/Mosaic is not; your own kernel index is built on the stated assumption that "the
  authoring model has little or no Pallas/TPU material in its training set," measured as **2/8 vs 8/8**
  path-only vs. pasted briefs. The specialist's headroom should be larger here.
- **Against you:** Frontis had 5,758 tasks and a benchmark. You have 40+ kernel families and no leaderboard.

## What "better than Opus 5" can mean, in increasing difficulty

| | Target | Verdict |
|---|---|---|
| **A** | Beat Opus 5 on **`Author`** — given the same K1 diagnosis and the same pasted brief, a higher fraction of candidates that compile, pass parity, fire, and beat baseline | **Most likely to land, and economically the biggest lever.** The project already measured ~40% of one wave's wall-clock as rework on kernels broken from the start — that is headroom on compile/parity/fire alone, before any speedup comparison. Cheap to evaluate: `kgate` is already the grader. |
| **B** | Beat Opus 5 on **`Refute`** precision/recall | **Plausible and cheap.** Frontier models are trained to produce code, not to decline; the label is verifiable (a later candidate beating the claimed bound disproves the refute). Nothing in Frontis has an equivalent. |
| **C** | Beat Opus 5 **end-to-end on a lever-covered held-out family** | **Genuinely uncertain — call it a coin flip after Gym + SFT + RL.** Requires `Diagnose` at rough parity, which is long-context reasoning over messy profiler output and the step a 30B model is weakest at. |
| **D** | Beat Opus 5 end-to-end on a **family needing a new lever** | **Unlikely.** This is the 6.77× capability itself. |
| **E** | Beat Opus 5 on the **model lane** | **Not a realistic target.** Task scarcity, expensive rollouts, and the lever space is judgment across a huge heterogeneous surface rather than code authoring. |

> [!inferred] **The hybrid is not a hedge — it is what Frontis's own architecture implies.** Their design
> principle is "local skill in the weights, global composition in the harness." `Author`, `Tune` and
> `Refute` are *local* skills over a bounded context; `Diagnose` is *global* reasoning over a long, messy
> artifact. Nothing requires one model to serve all operators — OpenMLE-Evo already runs a **separate memory
> model** for its lazy summarization. So the configuration that most likely beats Opus-5-alone *first* is:
> **specialist for `Author`/`Tune`/`Refute`, frontier model retained for `Diagnose`.** That wins on
> cost-adjusted throughput long before any single model wins outright, and it is a strictly easier
> engineering target because each operator can be swapped and measured independently.

## The path runs *through* Opus 5, not around it

Your existing corpus is very likely too small for a 31-point swing. Rough scale from the README: 40+ kernel
families, with per-arm frontier lines across them and candidate ledgers underneath every experiment — call
it low thousands of candidate-level examples against Frontis's 26,259. Same order of magnitude, but with far
less task diversity.

So you would **generate** training data, exactly as Frontis did — 17,245 of its SFT examples came from
independently sampling and executing complete solutions, not from harvesting a prior campaign. The TPU
version:

1. Enumerate kernel tasks (40+ existing families + op-points from real model profiles via the
   downward-spawn rule + KernelBench/JAXBench/tokamax ops).
2. For each, sample many single-shot `Author` candidates **from Opus 5 as teacher**, with the load
   mandate's pasted brief — this is a cheap operator call, not a 22-experiment agent campaign.
3. Filter through the gates you already have. **The early-kill gate makes most of this free**: interpreter
   parity on a tiny shape and the HLO firing check need no accelerator, so only survivors consume chip time,
   and a measurement is seconds.
4. Distill the survivors; then RL on-policy against `F = t_reference / t_candidate` to push past the teacher.

Order-of-magnitude: ~500 tasks × ~40 samples ≈ 20,000 candidates → perhaps 6–10k high-quality examples after
filtering, comparable to Frontis's 9,014 trajectory-step examples. The dominant cost is teacher inference on
large pasted briefs, not TPU time — which is an unusual and favorable cost structure.

**This also resolves the structural-insight worry.** You are not asking the 30B model to rediscover the
experiment-8 jump; you are asking it to absorb a jump Opus 5 already made, from a teacher sample, in the
one training stage that can introduce out-of-support behavior.

## The moving-target problem, and the one thing that beats it

Opus 5 will not hold still. Frontis's own table shows the frontier moving fast (Sonnet 4.6 54.55 → Sonnet 5
59.09 → Opus 4.8 63.64 → GPT-5.6 Sol 72.73), and a specialist trained on a frozen corpus does not track
that. Any claim of the form "our 30B beats the best available model" has a short shelf life.

The durable claim is different, and it is the actual RSI argument:

> **A frontier model does not learn from your wiki. Your specialist does.** Every campaign adds candidates,
> receipts, verdicts and levers; each retraining folds them in. The gap compounds *on your workload*, on
> your hardware generation, in your framework lanes — the exact axes where general capability transfers
> worst. That is rung 3 of the [meta-evolution](../concepts/meta-evolution.md) ladder, and it is the only
> version of "better than Opus 5" that does not decay when the next Opus ships.

## The cheapest decisive experiment, before any of this

**Run an open ~30B model as a fourth arm in the existing harness on GQA attention.** Same protocol, same
skills, same gates, same family — you already run exactly this comparison for three arms.

That single number is the base-model starting point, and without it none of the above can be stated the way
Frontis states its result (a delta over its own base under an identical harness). It also settles the
question directly: if an untrained open 30B lands near 3.5× — Codex/Gemini territory, the first plateau —
then the gap to 6.77× is two structural moves and the distillation plan above is aimed correctly. If it
lands near 1.5× and cannot author compiling Pallas at all, then `Author` capability is the binding
constraint and Tier A is the whole project for a while. Days of work; it changes what everything else
should be.

## Bottom line

Beating Opus 5 **outright, end-to-end, on kernel campaigns** is a lab-scale program — Frontis's own
precedent says all three layers, and its 31-point swing came from a well-resourced team with a benchmark
you don't have. Treated as the primary goal it is likely to disappoint.

Beating Opus 5 **on the operators where a specialist has structural advantage**, inside the harness you
already trust, and compounding on a corpus a frontier model can never see — that is achievable, testable in
tiers, and worth more anyway, because it makes each subsequent campaign cheaper rather than winning one
comparison. And you can find out which regime you're in for the price of a fourth arm on one kernel family.

---

# Follow-up 2: the product goal — a *cheap* model as capable as Claude or Codex

**Restated goal (2026-08-06):** SFT on all relevant wiki data, plus generate many trajectories across models
and kernels, aiming at a **product built on a cheap model that is as capable as Claude or Codex** at TPU
model and kernel optimization. Is that realistic given Frontis's results?

## Yes — and this is the result Frontis actually demonstrated

The previous section asked whether a specialist could *beat* Opus 5, and had to answer "in tiers, with
caveats." **Parity-at-low-cost is a materially easier target, and it is the thing Frontis's paper literally
reports.** Read their headline table for cost rather than for rank:

| System | Medal Avg | What it costs |
|---|---|---|
| Qwen3.6-35B-A3B (base) | 39.39% | **3B active params** |
| **Frontis-MA1-35B** + OpenMLE-Evo | **60.61%** | 3B active |
| **Frontis-MA1-35B** + Evo-Max | **71.21%** | 3B active |
| Frontis-MA1-30B + Evo-Max | **66.67%** | 3B active |
| Claude Sonnet 5 + Claude Code | 59.09% | frontier |
| Claude Opus 4.8 + Claude Code | 63.64% | frontier |
| GPT-5.5 + Codex | 68.18% | frontier |
| GPT-5.6 Sol + Codex / Kimi K3 | 72.73% | frontier / 2.8T |

The `A3B` suffix is the product fact: these are MoE backbones with **~3 billion active parameters**. And the
whole evaluation ran under **12 h per task on a single RTX 4090 capped at 12 GB VRAM** — which the paper
notes is a *smaller* sandbox budget than most reported MLE-Bench evaluations.

So: **both** of their models beat Claude Opus 4.8 (63.64%). The 35B beat GPT-5.5 + Codex and landed within
**1.5 pp** of GPT-5.6 Sol and of a 2.8T model. That is not "approaching frontier capability" as a
projection — it is a measured result at roughly two orders of magnitude less active compute per token.

**Your stated goal is strictly weaker than what they achieved.** They aimed past parity and got there; you
are aiming at parity.

## Your two data sources map exactly onto their two SFT paths

This is not a coincidence of framing — it is the same corpus design:

| Frontis's SFT path | Your equivalent | Volume there |
|---|---|---|
| **Parallel path** — independently sample complete `Draft` solutions, threshold-filter on score | **Generate trajectories** across models/kernels | 17,245 full-response examples |
| **Evolutionary path** — retain useful `Improve`/`Debug`/`Crossover` steps from high-quality trajectory segments | **SFT on existing wiki data** — the candidate ledgers, verdicts, and receipts already on disk | 9,014 trajectory-step examples |
| | **total** | **26,259** |

Two things about your version of the second path are *better* than theirs, and worth being explicit about
because they raise the value per example:

1. **Your corpus is already frontier-authored.** Codex, Claude, Gemini and Antigravity generated it across
   40+ kernel families and 4 model families. SFT on the wiki *is* multi-teacher distillation — you have
   been collecting a distillation corpus as a by-product of doing the work.
2. **Your labels are verified, theirs are auto-filtered.** Frontis filters by execution score. Yours are
   receipt-backed (`kgate`, self-hashed), independently re-measured (author ≠ verifier), pre-registered
   (commit-order-enforced), and firing-audited. Higher label quality per example, and — unusually — the
   *negative* examples are labelled too (`refuted-patterns.md`, the refuted verdicts, the losing
   `cand<N>` commits).

## The one number the paper does not give you — and it's the one your plan needs most

**Frontis reports no SFT-vs-RL decomposition.** The word "ablation" appears **zero times** in the 61-page
report. There are two component comparisons (Figure 8: with/without entropic weighting; Figure 16:
OpenMLE-Evo vs original AIRA-Evo) but nothing that separates what the supervised warm start contributed
from what reinforcement learning added. The +21.22 pp is reported only as base → final.

That matters more for your plan than for anyone else's, because **both of your stated data sources feed
SFT**. The paper's own theory of the split (§4, citing Yue et al. 2025) predicts the shape:

- **SFT** distills behaviors *absent from the base model's sampled support* — it is what closes a capability
  gap to a teacher.
- **RL** moves probability toward the better candidates *within* that broadened distribution — it is what
  pushes past the teacher.

If that theory holds, then **SFT alone is the right and sufficient tool for your stated goal**, because
parity-with-the-teacher is exactly what distillation buys; RL is what you would add later to exceed it. But
the paper gives you no measurement of how far SFT alone gets. Treat "SFT-only reaches most of the gain" as
a **hypothesis to test cheaply on one kernel family**, not as something Frontis established.

> [!inferred] Worth noting this is a genuine weakness of the paper relative to others in this wiki. DGM
> ablates the archive, the self-improvement of the mutator, and greedy-vs-probabilistic selection.
> AlphaEvolve removes one mechanism at a time and reports that every component contributes. Frontis
> reports controlled *model* and *harness* swaps — which are excellent — but never decomposes its own
> training stack. For a team planning an SFT-weighted program, that is the single most decision-relevant
> missing number in the report.

## Where the cheap model reaches parity, and where it won't

The product does not need one model at parity on everything. Frontis's own principle — *local skill in the
weights, global composition in the harness* — says to split by operator:

| Operator | Volume in a campaign | Parity outlook on a cheap model |
|---|---|---|
| `Author` | **high** (5–12 candidates/experiment) | **Good.** Narrow, data-rich, and out-of-distribution for frontier models — your kernel index's own premise, measured 2/8 vs 8/8 path-vs-pasted. |
| `Tune` | **high** (sweep points) | **Good.** Near-mechanical once structure is fixed. |
| `Refute` | medium | **Good, and cheaply supervised.** Frontier models are biased against declining. |
| `Diagnose` (K1) | **low** (~1/experiment) | **The crux risk.** Long-context reasoning over messy profiler/HLO output — where a 3B-active model is weakest, and every downstream step depends on it. |

The economics fall out of that table: `Author` + `Tune` are where the token spend lives, and `Diagnose` is
roughly one call per experiment. **A hybrid that keeps a frontier model only for `Diagnose` moves ~90% of
calls onto the cheap model while risking almost none of the campaign's quality.** That is a shippable
product on day one, and it is strictly de-risked relative to training a single model to do everything.

Frontis did get one model to serve all four operators — so full-stack parity is demonstrated, not
speculative — but they had 5,758 tasks to do it with.

## The structural advantage you have over Frontis

They had to train before they had anything. **You already have a working system, and the harness is the
product; the model is a swappable operator.** That permits an incremental path where every step is measured
against the incumbent by machinery you already trust:

1. Ship the hybrid (cheap `Author`/`Tune`/`Refute`, frontier `Diagnose`).
2. Replace one operator at a time, graded by `kgate` receipts against the frontier incumbent on held-out
   families.
3. Absorb `Diagnose` last, once trajectory volume supports it.

No big-bang training run, no moment where the product is worse than what you have today, and each swap is
independently justifiable. This is the main reason the product framing is more realistic than the
"beat Opus 5" framing — it converts one large bet into a sequence of small, reversible, measured ones.

## Risks specific to *this* goal

1. **`Diagnose` capability is the gate — test it first and separately.** It is also the cheapest thing to
   test, because the wiki already contains labelled K1 diagnoses whose downstream verdicts reveal whether
   the chosen intervention class was right. Score a candidate cheap model on historical K1s before
   committing to anything else.
2. **Task diversity, not example count, is probably the binding constraint.** 40+ families × 40 samples
   gives volume but not variety, and risks a model that recognizes *your* families rather than the bound
   classification. The fix is cheap and already sanctioned by the protocol: **op-point enumeration**. The
   same op at different shapes/dtypes/batch is a genuinely different bound and a different correct answer —
   40 families × 10–20 op-points ≈ 400–800 tasks, plus KernelBench's 250. Diversity comes from op-points,
   not from more samples per family.
3. **The teacher is the ceiling without RL.** SFT-only yields "as good as the teacher, on distribution,
   much cheaper" — which *is* the goal as stated, but means the product inherits the teachers' blind spots
   (including their bias against `Refute`). Worth deciding deliberately whether that is acceptable for v1.
4. **Generation-specific overfit**, as flagged earlier: train mechanism selection, keep measured constants
   in retrieval.
5. **Internal product vs external product changes the data strategy.** If it optimizes *your* model families
   on *your* hardware, the existing corpus is close to representative and family-shaped overfit is
   tolerable. If it must handle customer models, frameworks and TPU generations it has never seen,
   op-point and generation diversity stop being a nice-to-have and become the whole data program. Worth
   settling before the generation run, because it changes what you generate.

## Answer

**Realistic — and better-supported by the evidence than the "beat Opus 5" framing.** Frontis is a direct
existence proof: a 3B-active MoE, post-trained on execution-grounded data, beat Claude Opus 4.8 and GPT-5.5 +
Codex and came within 1.5 pp of the best system in its table, on cheap hardware. Your domain is *more*
favorable than theirs (Pallas is out-of-distribution for the frontier; Kaggle is not), your labels are
better verified, and part of your corpus already exists.

The three things that decide it, in order: **(1)** whether a cheap model can do `Diagnose` — testable
against historical K1s in days; **(2)** whether you can reach a few hundred *diverse* tasks via op-point
enumeration rather than a few dozen families; **(3)** whether SFT-only closes most of the gap, which
Frontis's own theory predicts but its paper never measures.

---

# Follow-up 3: "the wiki goes into the weights, and the price problem goes away"

**Claims to evaluate (2026-08-06):** with a trained specialist, (a) the wiki no longer needs to ship as a
runtime knowledge base, since its content is in the training set; (b) LLM price is solved; (c) the model can
be slightly bigger — something that fits on an **H100**.

**Short version: (b) and (c) hold and are stronger than stated. (a) is half right, and the half that's
wrong is the expensive half — the wiki's own `regeneratable vs. earned` classification already draws the
line in exactly the right place.**

## (b) Price — right, and it's two multiplicative levers, not one

Frontis's backbones are `A3B` MoEs: **~3B active parameters**, evaluated inside a 12 GB VRAM sandbox. That
is the per-token lever. But the campaign cost in this domain is dominated by **input** tokens — the load
mandate pastes large briefs, and Frontis's own matched study shows prompt tokens at 41.5M of 75.3M total
(55%), with `Improve` prompts averaging 35.7K characters *after* their context work and 102.8K before.

So training buys a second, independent reduction: **a model that knows Pallas doesn't need the mechanics
pasted into every brief.** The load mandate currently pastes `pallas-kernel.md` through `## Debugging` — the
annotated skeleton, memory spaces, the (8,128) rule, scalar prefetch, the compile-gotcha table — into
*every* author brief, on the explicit premise that the model has none of it. That premise is what training
removes. Combined with operator-conditioned bounded context (Frontis: −41.7% total tokens, −86.1% at the
`Improve` p99), the two effects compound.

> [!inferred] **The metric that decides whether the product works is cost per *frontier-advancing
> experiment*, not cost per token.** A cheap model that needs 3× the candidates has spent its savings — and
> worse, candidates cost chip time for measurement, not just tokens. Frontis tracks exactly this ratio
> (new-best validation updates per million model tokens: 1.77 → 3.27) and it is the right product KPI here
> too. One structural feature of this domain makes the small-model case easier than it looks: the
> **early-kill gate** rejects broken candidates at interpreter-mode parity and the HLO firing check, with no
> accelerator involved — so a higher candidate count is far less punishing here than in MLE, where every
> candidate is a real training run. Cheap-but-noisier is a much better trade on TPU kernels than it would be
> on MLE-Bench.

## (c) H100 sizing — agree, but go **MoE-bigger, not dense-bigger**

80 GB of HBM is a comfortable envelope, and the shape matters more than the parameter count:

| Config on one H100 80 GB | Weights | Notes |
|---|---|---|
| ~30–35B **MoE, ~3B active**, fp8 | ~30–35 GB | **The Frontis shape.** Leaves ~45 GB for KV cache — important, because 40–60K-token briefs make KV the real constraint on batching. Computes like a 3B model. |
| ~30–35B MoE, bf16 | ~60–70 GB | Fits, but KV-starved at long context; batching suffers. |
| ~32B **dense**, fp8 | ~32 GB | Same footprint, **~10× the compute per token** for arguably less capability than a larger-total MoE. |
| ~70–100B MoE, 4-bit | ~35–50 GB | The "slightly bigger" direction that actually pays. |

The recommendation: **increase *total* parameters via MoE before increasing *active* parameters via dense.**
Frontis's choice of `A3B` is not incidental — it is the entire cost thesis, and it is what lets a 35B model
serve at 3B-model economics.

Two caveats worth holding:

- **`Diagnose` may be the operator that wants dense.** Long-context reasoning over messy profiler/HLO output
  is precisely where a 3B-active MoE is weakest relative to a dense model of the same footprint. If the
  `Diagnose` probe comes back poor, the fix is per-operator: a dense ~14–32B for that one call, or keep the
  frontier model there. The harness already supports per-operator model choice — OpenMLE-Evo itself runs a
  separate memory model.
- **You may not need an H100 at all.** You have TPUs. A 30B-A3B MoE serves comfortably on a v5e/v6e slice,
  which removes both the GPU purchase and the per-token API bill — and makes the serving stack itself a
  workload this wiki optimizes. H100 is the right target if the product ships *externally* and must be
  portable; it is not required if it runs beside the optimization work.

## (a) "No need to ship the wiki" — the half that's wrong

The wiki does **four** jobs. Training displaces one of them, partially.

| Role | Displaced by training? |
|---|---|
| 1. Runtime knowledge base — the pasted author brief | **Partially.** The stable mechanics can move into weights. |
| 2. **Training-corpus generator** — candidate ledgers, receipts, verdicts, levers | **No — and it becomes more important.** |
| 3. **Verification substrate** — `kgate` receipts, lever-coverage set-diff, LINT, the auditor | **No.** |
| 4. Human-readable record and product surface | **No.** |

And within role 1, the wiki has *already published the correct split* — it just wasn't written as a
training-vs-retrieval decision:

| Wiki's own classification | Training analogue |
|---|---|
| **Regeneratable synthesis** — the indexes and blueprint, "derived… throw it away and rebuild it… nothing original lives here" | **Bake into weights.** Stable, shaped, re-derivable knowledge: the core thesis, the three sinks, the intervention-class ladder, the ordering, the dispatch floor, category routing. |
| **Earned, non-regeneratable rules** — `BRIEFS.md`, which "accretes one hard-won lesson at a time and must never be rebuilt from a prompt, because no prompt can re-derive an incident that already happened" | **Keep retrieved.** Append-only, incident-driven, and current. |

Three things in the "keep retrieved" pile are not negotiable, and each has a measured incident behind it in
this very wiki:

1. **Generation-specific constants.** The kernel index enumerates what must be re-derived per target — MXU
   tile edge (128 ≤v5p / 256 v6e+), MXUs per TensorCore, VMEM budget and OOM wall, VMEM:HBM ratio,
   issue-slot counts, HBM bandwidth, available profiling signals, "and every measured block size and
   speedup below — all v6e" — with the instruction to **query** them via `pltpu.get_tpu_info_for_chip` and
   to treat measured numbers "as calibration for the *shape* of the answer, not as targets." A model trained
   on v6e trajectories will confidently emit v6e block sizes on v7. Baking constants in is not neutral, it
   is actively harmful.
2. **Version drift.** "Framework-version kernel-API drift is real — primitive names and in-kernel-legal ops
   move between releases; assume the target version's API, not memory." A trained model *is* memory. The
   MaxText DeepSeek flag bundle silently rejected on an April-2026 libtpu cost ~5–8 experiments; that class
   of fact must reach the agent the day it's discovered.
3. **New hardware.** When v7/Ironwood ships, a v6e-trained model is stale, but a knowledge base gets a new
   `hardware/` directory the same afternoon. This is precisely
   [KernelEvolve](../sources/kernelevolve.md)'s MTIA argument — a hand-authored KB "enabl[es] immediate
   LLM-based kernel generation **without model retraining**" for an accelerator absent from all training
   corpora. That paper is the existence proof for the retrieval side of this trade.

> [!inferred] **The operational framing that makes this concrete: dropping the wiki converts a config change
> into a model release.** Today, when a libtpu version rejects a flag or a new generation lands, you edit
> `BRIEFS.md` and every subsequent run is correct within minutes. Bake it in and that fix waits for the next
> training run. For a product with users on different libtpu/JAX/hardware versions, that is a serious
> regression in operability, and it shows up exactly when you least want it — at a hardware transition,
> which is also when demand for the product peaks.
>
> The opposite error is just as real, though: keeping the *whole* brief after training wastes the price win
> you paid for. The target is **a much smaller brief, not no brief** — drop the Pallas mechanics, keep
> BRIEFS, the class page's lever list, and the queried hardware constants.

**And the flywheel argument is the decisive one.** The wiki is what generates the corpus for v2. Stop
maintaining it and you freeze the model at v1 — you would be dismantling the meta-evolution loop
([`meta-evolution`](../concepts/meta-evolution.md)) to save context tokens. The correct reading is the
inverse of the claim: **training makes the wiki *less* necessary at inference time and *more* necessary as
infrastructure.**

This is the same asymmetry already recorded on
[`retrieval-augmented-prompt-synthesis`](../concepts/retrieval-augmented-prompt-synthesis.md): systems
retrieve either *what the system has learned* or *what the system was told*, and only the first can be
bootstrapped by the loop. Curated hardware facts are the second kind. Training absorbs the shape of the
reasoning; it cannot absorb next quarter's silicon.

## Net

Both problems do get solved, with one correction to the framing:

- **Price: solved, twice over** — cheaper per token *and* fewer tokens, self-hosted on hardware you already
  have. Measure it as cost per frontier-advancing experiment.
- **H100: fine, and the right move is a larger-total MoE at ~3B active, not a dense model** — with a
  possible dense or frontier exception for `Diagnose`.
- **Shipping the wiki: still required, but it shrinks at inference and grows as infrastructure.** The brief
  loses the Pallas mechanics and keeps BRIEFS, the class-page levers, and queried hardware constants. The
  ledger/receipt/lever machinery is untouched, because it is the training pipeline and the grader.

## See also
- [`../sources/frontis-ma1.md`](../sources/frontis-ma1.md) · [`../concepts/meta-evolution.md`](../concepts/meta-evolution.md)
  · [`../concepts/program-evolution-operators.md`](../concepts/program-evolution-operators.md)
- [`../sources/tpu-performance-autoresearch-wiki.md`](../sources/tpu-performance-autoresearch-wiki.md) ·
  [`../sources/kernelevolve.md`](../sources/kernelevolve.md) · [`../sources/alphaevolve.md`](../sources/alphaevolve.md)
- [`../concepts/evolutionary-self-improvement.md`](../concepts/evolutionary-self-improvement.md) — the
  population shapes discussed in #1 · [`../topics/mle-agents-and-benchmarks.md`](../topics/mle-agents-and-benchmarks.md)
