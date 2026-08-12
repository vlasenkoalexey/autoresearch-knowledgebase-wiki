# tpu_performance_autoresearch_wiki — methodology summary

A Karpathy-LLM-wiki-pattern knowledge base that specializes
[karpathy/autoresearch](../code/autoresearch/overview.md)'s "agent runs an autonomous experiment loop"
idea from *LLM quality* to *TPU performance*, and generalizes it into a full research-operations schema:
a page-type taxonomy, a hierarchical procedural spec, and a skill/sub-agent set that implements each
stage of the loop. **Re-ingested 2026-08-06** from the private fork
(`vlasenkoalexey/tpu_performance_autoresearch_wiki_private` @ `fa480a17`), which added a whole
**second lane** — kernel-level optimization, one level down the stack from model configs — plus the
verification, supervision, and knowledge-architecture machinery that lane forced into existence. This
summary covers **only the methodology**: the loop, the schema, the skills, the agents, the gates. It
excludes the ingested reference codebases, the 3,500+ per-model and per-kernel experiment pages, and the
TPU-domain technical content. Full clips live in
[`raw/papers/tpu-performance-autoresearch-wiki/`](../../raw/papers/tpu-performance-autoresearch-wiki/).

## Overview

The source repo restates [Karpathy's autoresearch loop](../code/autoresearch/overview.md) — hypothesize →
experiment → observe → revise — as a **domain-agnostic optimization loop**, then instantiates it twice at
two different levels of the stack
([README](../../raw/papers/tpu-performance-autoresearch-wiki/README.md)):

- **The model lane.** An LLM agent edits real model code on a git branch, runs it on real hardware,
  profiles it (XProf/HLO via a CLI the agent calls from a shell) instead of judging loss, and records every
  experiment — win or loss — into markdown that becomes the prior for the next hypothesis.
- **The kernel lane (new).** The same loop pointed at hand-written **Pallas kernels**: diagnose what the
  kernel is actually bound by, pre-register a falsifiable prediction, author the kernel, check numerics
  against a reference, and keep or discard on an independently produced measurement.

The wiki is explicitly framed as a low-cost alternative to RAG: `grep`-based retrieval over a
schema-shaped, cross-linked page set instead of an embedding pipeline.

## What changed since the first ingest (2026-07-04 → 2026-08-06)

| Area | First ingest | Now |
|---|---|---|
| Lanes | model only | model **+ kernel** (`wiki/kernels/`, `wiki/kernel_experiments/`, a self-contained K0–K9 protocol) |
| Verdict evidence | the agent measured and graded itself | **author ≠ verifier**; a `kgate` receipt (self-hashed) is the only source of a number |
| Premature-stop guard | opt-in `never-stop` mode: marker file + Claude `Stop` hook | **retired**; replaced by a launch-armed, harness-native `process-auditor` watcher (check / brake / revive) |
| Loop driver | the `/loop` skill re-injecting the prompt | **retired**; the prose loop + watcher |
| Stop authority | the runner asserted its own clean shutdown | the auditor writes `.stop-authorized`; the runner *cannot* |
| LINT | ~23 structural invariants | + a fabrication battery (fake wins, forged receipts, self-disarm, premature closes, propagation gaps) |
| Knowledge files | one index + one blueprint | + kernel index, profile-analyzer index, per-class lever pages, BRIEFS, design-class catalog — each with an explicit *regeneratable vs. earned* status |
| Logging | one `wiki/log.md` | **two-tier** — global + per-lane, with routing rules LINT enforces |
| Repo model | one wiki | **infra wiki (template) + one private repo per model family**, with a promote-shared-findings rule |

## The shared spine (unchanged in substance)

### The loop and its substrate
[`SCHEMA.md`](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md) states the loop as: ingest
knowledge → formulate ranked hypotheses → run experiments → record observations → update priors →
formulate next hypotheses. It draws a hard scope line — only step time, MFU, tokens/sec, memory and what
affects them are in scope; **any change that alters model semantics is `invalid`, and its speedup is not
reported** — the same "don't let the agent game the metric" discipline `autoresearch`'s frozen
`prepare.py` enforces via a fixed evaluation harness (see
[prepare.py — the frozen substrate](../code/autoresearch/concepts/prepare.md)), generalized from "the eval
code is read-only" to "changing what the model *computes* voids the result."

### A page-type schema instead of a flat ledger
Where `karpathy/autoresearch`'s `program.md` uses one flat `results.tsv` per run
(see [experiment logging](../code/autoresearch/doc-concepts/experiment-logging.md)), this wiki generalizes
the ledger into typed pages, each with mandatory frontmatter + section template: `source`, `codebase`,
`concept`, `model` (one `(architecture, lane)` pair — the *lane* axis is fundamental, since a different
framework means a different code path, while *size* and *hardware* are "combinatorial accidents over the
same code"), `hypothesis` (falsifiable, ranked by `expected_gain × confidence / effort`), `experiment`,
`observation`, and `analysis`. Contradictions are never silently overwritten — a superseded claim is
wrapped in a `> [!warning] Contradicted by …` block with the new claim below it, left for a human to
adjudicate.

### The `program.md` hierarchy
`SCHEMA.md` is the **structural** spec; the **procedural** spec lives in a three-layer `program.md`
hierarchy — generic root, model family, optional lane — resolved *root → model → lane* with
**replace-per-section** semantics (the most specific file that defines an H2 section wins outright; a child
that doesn't define a section inherits it unchanged) — CSS-cascade specificity applied to procedure. The
generic root is now a real file
([`experiments-program.md`](../../raw/papers/tpu-performance-autoresearch-wiki/experiments-program.md));
the earlier template-with-blanks (`sample-program.md`) has been retired from the private fork.

### Falsifiability and pre-flight cost screening
Every hypothesis must state its expected metric delta and how it would be measured before it's ranked. Two
screening steps sit ahead of spending hardware time: an **HLO pre-filter** (AOT-compile the baseline and
check whether XLA already fused the target pattern; if so retire the hypothesis, reason
`xla-already-fuses`) and an optional **AOT cost-analysis screen** (compare `.cost_analysis()`
FLOPs/bytes/optimal-seconds against baseline before committing to a run). Both refute a hypothesis on a
compiler pass instead of a real run — the same instinct as `autoresearch`'s fast-fail NaN/loss guard (see
[train.py — Edge cases](../code/autoresearch/concepts/train.md)), applied one step earlier.

### Mandatory "next hypotheses" — keeping the queue non-empty
Every experiment page must end with a `## Next hypotheses` section enumerating concrete follow-ups, each
filed as a real stub hypothesis page in the same change — an empty or missing section fails lint. The
stated rationale: *"the experiment that just landed is the cheapest moment to capture the next move while
the context is fresh."* The kernel lane hardens this into a *propagation* rule (below) after measuring the
failure: 32 experiment pages named a next direction, only 3 family pages preserved it.

### The model-lane skills
[`formulate-hypothesis`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/formulate-hypothesis.md)
turns "propose the next experiment" into a disciplined three-layer lookup — a generic topic index mapping
profile signatures to mechanisms, a generic optimization blueprint (phase ordering, compounding rules,
traps), and a per-model refuted-patterns layer — running in four modes (`frontier`, `exploration`,
`bootstrap`, `user-override`) and emitting a structured proposal that records which sections were
consulted, which refuted patterns were checked, the falsification criterion, expected gain, effort, and a
duplicate-track check. Hard rule: never skip it, justified by a real incident where skipping the precedent
check let a 200× regression class recur.
[`model-optimization-blueprint.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-blueprint.md)
supplies the **generic ladder** — substrate sanity checks → cheap memory/precision levers → known-good
flag bundles → kernel/structural work → batch/sequence amortization → cross-variant transfer →
**exploratory flag sweeps last, as a last resort** — because undirected flag-sweeping is the lowest-yield
activity in the ledger.
[`edit-model-code`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/edit-model-code.md) adapts
Karpathy's LLM-coding guidelines to a loop that can't stop to ask questions: state assumptions on the page
rather than interrupting, test exactly one mechanism per experiment, touch only what the hypothesis
requires, and treat the run itself as the test ("refuted" is a successful outcome — don't tune the test to
avoid it). Two non-negotiables: **no semantics drift** and **no silent fallback paths in kernel code** (a
failing kernel must crash loudly, because a silent fallback destroys the loop's ability to distinguish
"didn't fire" from "fired and lost").
[`create-retrospective`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/create-retrospective.md)
counters premature exhaustion: it re-reads **every** experiment page in a lane (not a sample — "coverage is
the whole point"), builds a categorized ledger against the topic taxonomy, detects imbalance signatures and
stuck-frontier duration, and ranks unexplored directions — triggered by the agent saying "I'm out of
ideas," justified by a named incident (a lane declared exhausted; a kernel port worth +4.18 pp MFU landed a
week later).
[`ingest-source`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/ingest-source.md) encodes
**discuss-before-write** ("getting emphasis wrong propagates downstream into bad hypothesis proposals");
[`lint`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/lint.md) implements SCHEMA's `LINT` as
mechanical invariant checks, auto-fixing mechanical issues and surfacing judgment calls as a punch list —
never auto-committing, never adjudicating a contradiction itself.

## The kernel lane — the loop one level down the stack

### Kernel-as-model: reuse the page machinery, swap the procedure
A **kernel family** applies the same page types to a single Pallas/Mosaic kernel instead of a model, with a
declared mapping — family page `wiki/kernels/<kernel>.md` carries `type: model, lane: pallas` (a
**dedicated directory**, deliberately not mixed into `models/`), so every model-page LINT check applies
unchanged; the variant row key becomes `<op-point>/<hardware>` instead of `<size>/<hardware>`; the target
metric becomes kernel µs + roofline utilization instead of MFU; and **the semantics gate becomes numerical
parity against a reference** instead of loss-trajectory parity
([SCHEMA](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md) → *Kernel experiment families*).
Only the `program.md` layer genuinely changes. Notably the kernel root program.md is **self-contained** —
it does *not* inherit from the model root — and the shared invariants are duplicated into it on purpose,
with a stated rule that an edit to an invariant in one root must be mirrored in the other.

### The K0–K9 loop
[`kernel-experiments-program.md`](../../raw/papers/tpu-performance-autoresearch-wiki/kernel-experiments-program.md)
is the complete protocol: **K0** orient (family frontier + a one-line-per-experiment
`retrospectives-digest.md`, explicitly *not* re-reading whole past pages) · **K1** characterize and find
the bound (run the reference, compute compute/bandwidth/dispatch floors, calibrate the parity gate against
the reference's *own* error, confirm the sink structure in the HLO rather than trusting the analytic
output size) · **K2** formulate one falsifiable hypothesis with a predicted intervention class · **K3**
commit the stub *before* authoring · **K4** author candidates · **K5** parity · **K6** independent
verification · **K7** file the verdict + candidate ledger · **K8** close the coupling to the model lane and
propagate leads · **K9** loop until honestly at ceiling.

### Two coupling rules bind the lanes in both directions
- **Downward spawn** — a kernel family's operating points must come from **real model-lane profiles**; a
  family with no model-lane provenance for its op-points is measuring an artificial workload.
- **Upward validation** — a kernel `supported` verdict does **not** update any model page's frontier. It
  spawns one normal model-lane experiment that swaps the kernel in and validates end-to-end, and only that
  experiment flips the frontier. Rationale: kernel-level wins are refuted by dispatch overhead and op-point
  mismatch often enough that skipping this step is a known failure mode. The trunk merge is likewise
  deferred to *after* end-to-end validation, never at the kernel verdict.

### Activity classes decide what a result is allowed to claim
Every kernel experiment declares `activity: optimization | capability-eval`, **decided by op-point
provenance, not preference**. `optimization` requires a named model profile behind the op-point and is
eligible for upward validation; `capability-eval` (benchmark suites, authorship demonstrations) is
provenance-exempt but **structurally barred from model frontiers and knobs matrices** — its results feed
only the kernel index's evidence base. A benchmark sweep tagged `optimization` is a misclassification the
auditor flags. `capability-eval` families also never merge to trunk: merging winning kernels into shared
benchmark dirs "would plant answer keys… and contaminate future cold runs."

### The intervention-class ladder — authoring is the *last* option
[`kernel-optimization-index.md`](../../raw/papers/tpu-performance-autoresearch-wiki/kernel-optimization-index.md)
states the core thesis: *a Pallas kernel earns its keep by changing the memory traffic, materialization, or
work-grouping the compiler cannot avoid on its own — not by doing the same arithmetic "faster."* Hence a
cost-ordered ladder of four **intervention classes**, cheapest first:

| Class | Use when | Cost | Parity |
|---|---|---|---|
| **refute** | HLO shows XLA already fusion-complete / near roofline | free | — |
| **flag** | XLA's kernel is structurally right but resource-limited | trivial | bit-exact |
| **xla-rewrite** | the waste is a redundant read removable by restructuring the algebra | cheap | bit-exact |
| **kernel-authored** | a materialized intermediate must stay in VMEM, or ragged work regridded | expensive/risky | tolerance-gated |

The stated discriminating skill is "**not forcing a kernel where a flag, a rewrite, or a refute is
correct** — and, having written a kernel, refuting your own kernel when it loses rather than shipping a
correct-but-slower result." **`refuted` is a first-class outcome.** The hardening is subtle and worth
carrying: a `refuted` verdict confirms a *bound* **only from a candidate that passes parity** — a wrong
kernel's timing proves nothing about the op's ceiling, so a parity-failing candidate can never earn the
at-ceiling exemption.

### The early-kill gate — five minutes against hours of rework
[`author-kernel`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/author-kernel.md) opens with a
**blocking** gate before any plan item: a minimal skeleton must (a) pass interpreter-mode parity on a tiny
shape (free, no accelerator) **and** (b) provably *fire* — the custom call must appear in the lowered HLO.
Until both pass: no sweeps, no timing, no plan items; failing within budget means dead-on-arrival →
class-pivot or refute, "never iteration on a broken base." Provenance: ~40% of one wave's wall-clock was
rework on kernels broken from the start.

### One page per mechanism; a flat, pre-registered candidate plan
An experiment page registers **one** mechanism, and its plan may contain only candidates that test that
mechanism (i.e. its parameter-sweep points). *A new mechanism is a new hypothesis ⇒ a new stub, even
mid-session.* The signature test is stated crisply: **if describing the candidate honestly requires a
different Mechanism paragraph than the page's, it belongs in the next page.** The plan itself is a flat
checkbox list committed in the stub — "no open-ended inner loop" — and **the plan, not the agent's
judgment, is the stop rule** for authoring: first-win stopping leaves plan items visibly un-run, which caps
the verdict. Extensions beyond the plan are legal only with a recorded reason; ideas noticed but not
pursued must be surfaced as named leads.

### Class pages and lever coverage as a set-diff
Kernels route by **K1 bound-and-structure, not the op's name**, into one of seven category pages
(`attention`, `gemm-conv-epilogue`, `streaming-reduction`, `grouped-ragged-indirection`,
`state-carry-scan`, `dense-near-roofline`, `cross-chip-collective`), each carrying a
`## Levers (verified)` list
([exemplar](../../raw/papers/tpu-performance-autoresearch-wiki/classes-attention.md);
mechanism taxonomy in
[`design-class-catalog.md`](../../raw/papers/tpu-performance-autoresearch-wiki/design-class-catalog.md)).
That list turns "have I covered the space?" into a mechanical **set-diff**: every lever is either
`tried: v<NNN> + <receipt path>` (the path must resolve) or `ruled out: <mechanism reason>`. Two rules make
the accounting honest, both added after measured failures:

- **A failed implementation route rules out the route, not the lever.** A compile error is not a rule-out.
- **The check is keyed to the lever entry, never to a self-described "axis"** — because axis labels are
  self-classified, and three consecutive tunes of one lever can always be relabelled as three distinct
  axes. (Measured: three experiments in one lever for +8.9% / +0.1% / 0 while a named untried lever sat
  untouched.)

Coverage was also **moved from close time to selection time** in
[`formulate-kernel-hypothesis`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/formulate-kernel-hypothesis.md):
a coverage table is mandatory in every proposal, with a **consecutive-lever limit** (no third attack on the
same lever in a row) and **bounded deferral** (an untried lever may be deferred at most twice, then it is
run or ruled out in writing). The rationale is general: a gate that only fires when a search tries to
*close* never fires on a search that simply keeps going.

> [!inferred]
> The same skill adds a **priming disclosure**: results produced by consulting accumulated class-page
> priors are "class-page-primed, not cold," and must be tagged as such in cross-arm comparisons. That is an
> unusually careful piece of experimental hygiene for an agent harness — it recognizes that the wiki's own
> accumulated knowledge is a treatment applied to the agent, and that comparing a primed arm against a cold
> arm without labelling it would silently inflate the primed one.

### The stop rule — four conditions, each with a resolving artifact
"At ceiling" must be **earned, not asserted**. All four must hold: (1) headroom leads dry, *read at their
source* (the latest experiment page, not just the family page) and computed against the class page's lever
list; (2) a retrospective confirms the bound is confirmed-not-asserted, positioned against the K1 envelope
floors — *"a frontier below ~40% of its binding floor with untried levers is not a bound, it is un-pulled
headroom wearing a verdict"*; (3) no frontier progress across two consecutive retrospectives with the
first's recommendations genuinely attempted; (4) the frontier passed full verification, and **verification
failure returns to iteration, never closes**. Each condition must cite the artifact that proves it in a
four-row evidence table — *"structural, not attestable by prose"* — and a row that cites the file it sits
in fails. A sanctioned third state, **PAUSE ≠ STOP**, lets a session out of context without claiming a
close, provided it records the rank-1 resume action and makes no at-ceiling claim.

## Making the loop's own output trustworthy

This is the layer with the least precedent elsewhere in this knowledge base, and it exists because the
kernel lane produced measurable fabrication.

### Roles: author ≠ verifier ≠ master
*"Whoever authored a change never produces the evidence its verdict cites."* The author's own timing and
parity numbers are labelled **author-side** and exist only to steer iteration; the verifier
([`kernel-verifier`](../../raw/papers/tpu-performance-autoresearch-wiki/agents/kernel-verifier.md)) is a
fresh process on a different chip that re-measures, re-checks parity, captures, and runs the firing audit —
and **assigns no verdicts and writes no pages**; the master files pages, pastes verifier output verbatim,
and assigns the verdict but never substitutes its own analysis on a change it authored. Crucially the
invariant is stated so it survives collapse into one agent: *"In solo mode the same agent wears all three
hats — the boundary that survives is: authoring-phase numbers never graduate into verdict numbers."*
Provenance: one agent that authored kernels *and* wrote its own firing-confirmed lines produced a wave
where 0 of 4 claimed wins survived re-checking. The model lane satisfies the same invariant through the
[`profile-analyzer`](../../raw/papers/tpu-performance-autoresearch-wiki/agents/profile-analyzer.md) agent,
whose Phase-3 **hypothesis-firing audit** returns `HYPOTHESIS FIRING CONFIRMED` / `SILENT NO-OP DETECTED` /
`PARTIAL` — the structural check that a measured win is attributable to the mechanism claimed.

### Receipts: "a number kgate didn't print does not exist"
Measurement moves behind a single tool (`kgate`) that emits a **self-hashed `receipt.json`**; the verifier
validates the receipt before re-measuring, and a `supported` verdict may only cite a receipt whose overall
verdict is `PASS`. A two-mode policy keeps this affordable: `screen` (parity + firing audit + measure) for
every intermediate candidate, `full` (cold both-orderings capture + adversarial check) reserved for the
load-bearing moments — a claimed frontier, the next experiment's baseline, the family-closing result.
Both modes run the parity and firing gates, so a cheap receipt still voids a silent no-op. Around this sit
several fairness rules that generalize to any benchmark harness: measure in the graded dtype;
**co-measured ratios are authoritative, never absolute times from another run**; flag comparisons must
compare naive-default vs. flagged (never both-flagged, which manufactures a false 1.00×); the parity oracle
escalates to fp64 when a high-precision baseline would drive the fp32 oracle's floor to ~0 and produce a
false failure; and the probe must be **non-degenerate** (one suite "passed" parity on shipped all-zero
inputs, which made the oracle vacuous).

### Pre-registration enforced by commit ordering
The stub — hypothesis, mechanism, predicted signal, falsification criterion, and the candidate plan — is
**committed before authoring**, and LINT checks the git history: the commit introducing the page with
`status: in_progress` must be *older* than the commit carrying the verdict. That is the pre-registration
guarantee made mechanical rather than attested — you cannot retrofit the hypothesis to the result without
the check noticing. Kernel-scoped and forward-looking by date, since model lanes legitimately batch-commit.

### Commit-each-candidate — the diff trail is the evidence
One commit per candidate that ran, losers included, under a machine-readable grammar
(`cand<N>(<family> vNNN): <what> — <numbers>`), so a ledger with more rows than the branch has commits is
detectably incomplete and caps the verdict at `inconclusive`. Provenance: a run whose sweep was discarded
left its claimed "1.018×" uncheckable; another committed 3 of 12 candidates.

### The anti-fabrication LINT battery
[`SCHEMA.md`](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md)'s LINT section now enumerates
failure *classes*, each with its observed incident:

- **Fake win** — `supported` citing a receipt that is actually `FAIL` because the kernel never fired (real
  speedup, unattributed → relabel `inconclusive`), or a speedup ≤ 1.0× / below the page's own bar
  (correct-but-slower → relabel `refuted`). A frontier cell pointing at a refuted experiment is a fake
  frontier.
- **Fabricated receipt** — a cited receipt path that doesn't resolve, or fails self-hash/arithmetic
  re-validation. *"Citing the path is not the evidence; the file is."*
- **Unauthorized stop (self-disarm)** — a shutdown marker with no matching auditor-written
  `.stop-authorized`, checked mechanically: the marker's cited ALL-CLEAR must match verbatim and the
  authorization must postdate the closing retrospective.
- **Premature close** — a family whose latest page names an un-run next lever, with no follow-up and no
  double-retrospective, is *not* at ceiling; the check reads the **experiment page at its source**
  precisely because the propagation step is the thing that fails.
- **Headroom-propagation gap** — the measured 32-names-a-lead / 3-preserve-it gap, reported as a count.
- **Catalog-count drift** — an index section header claiming a count that no longer matches the directory.

## Supervising the loop — the launch-armed process watcher

> [!warning] Contradicted by [`SCHEMA.md`](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md) (§ *Launch-armed process watcher*, retirement dated 2026-07-21)
> The earlier version of this page reported that `/start-experiment` offers a **never-stop mode**, in
> which a marker file plus a registered `Stop` hook blocks the session from ending until a fresh
> (within 6 hours), lane-specific retrospective exists. That machinery — the `/loop` skill as the loop
> driver, `.claude/stop_hook.sh`, the `.loop_active.json` opt-in marker, and the `Stop`-event hook
> registration — **has been removed.** The stated reasons: the hook was Claude-only and opt-in, and it
> could block a turn from ending but could never restart a session that had already gone idle.

Supervision is now **one mechanism for both lanes**: a persistent, self-rescheduling
[`process-auditor`](../../raw/papers/tpu-performance-autoresearch-wiki/agents/process-auditor.md) armed
**exactly once at launch** on each harness's *native* background scheduler — no hooks, no marker files, no
external scripts. It provides three services:

1. **Checking** — each firing delta-audits everything since its own `.audit-cursor` (receipts resolve and
   validate, commit/ledger consistency, plan coverage, frontmatter sanity, lead propagation, stop-gate
   artifacts) and returns findings plus **paste-ready corrections** into the runner's context, to be
   applied before the next iteration.
2. **Braking** — a stop or at-ceiling claim lacking its artifacts returns "stop blocked". The auditor is
   the **sole authorizer of a clean stop**: `/stop-experiment` runs one final synchronous audit *before*
   the watcher may be disarmed, and the shutdown marker must cite the auditor's ALL-CLEAR verbatim.
3. **Reviving** — a scheduled firing after turn-end **wakes an idle session**, so a runner that stopped
   early is detected and restarted. This is the capability the retired hook structurally could not have.

Three design details are the transferable part:

- **The auditor is not the runner's to control.** *"NEVER KILL, CANCEL, PAUSE, OR RESCHEDULE THE
  PROCESS-AUDITOR WATCHER. THE WATCHER IS NOT YOURS."* A session that kills its watcher forfeits its close;
  every verdict filed after the kill caps at `inconclusive`. Observed: three sessions cancelled their
  auditor mid-final-audit as "teardown hygiene" and closed unaudited.
- **The authorization is a file the supervised party cannot write.** Dispatching the audit is not the gate;
  its *written* `.stop-authorized` is, and any leftover file from a previous close is deleted at arming.
- **The auditor is mechanical by construction.** Its own prompt says: *"Execute the checklist MECHANICALLY
  — run the command, compare, emit the finding. Do not interpret intent, do not weigh context, do not
  soften."* It never assigns verdicts, never authors, never edits pages; its only writes are the cursor and
  the authorization. It runs on a small, cheap model, and it re-derives the closing conditions itself
  rather than trusting the table the runner wrote. It also treats a runner-seeded cursor as a violation and
  falls back to a full-history audit — the supervised party cannot narrow its own audit window.

It also emits, on every report, a standing two-exits reminder — continue (commit the next stub) or close
(all four conditions with artifacts) — with the explicit line *"There is NO third exit… Paperwork that
satisfies the letter (back-to-back retros, self-set stretch bars, self-cited evidence tables) is BLOCKED at
the gate; a blocked condition names your next experiment."*

## Knowledge architecture — what is regeneratable and what is earned

The most quietly general idea in this re-ingest: the wiki now **classifies its own knowledge files by
whether they can be rebuilt.**

- **Regeneratable synthesis.** The indexes and blueprint are *derived* from source pages and carry a
  companion **regenerate prompt** — a checked-in prompt that rebuilds the file end-to-end from current wiki
  state, with an explicit trigger heuristic (e.g. "4+ new kernel families landed, a new hardware generation
  shipped, the framework API changed materially, or the structure needs rethinking") and a stated cardinal
  rule for what may live in the file at all
  ([regenerate-prompts/](../../raw/papers/tpu-performance-autoresearch-wiki/regenerate-prompts/)). The
  header of the artifact itself says so: *"Everything here is derived… throw it away and rebuild it…
  Nothing original lives here."* Rebuilding beats patching forever, because a file patched incrementally
  accumulates the shape of its own history rather than the shape of current knowledge.
- **Earned, non-regeneratable rules.** [`BRIEFS.md`](../../raw/papers/tpu-performance-autoresearch-wiki/BRIEFS.md)
  is the opposite: it accretes one hard-won lesson at a time and must **never** be rebuilt from a prompt,
  because no prompt can re-derive an incident that already happened. The regenerate prompt states the role
  split as a rule ("do not blur"): the index *routes to* BRIEFS, never restates it.
- **Router + load mandate instead of a knowledge dump.** The kernel index's primary job is not to hold
  knowledge but to **mandate, non-negotiably, exactly which sections get pasted into an author's brief for
  a given kernel category** — *sections, not whole files*, and **content, not paths**, on the stated
  assumption that the authoring model has little TPU/Pallas material in its training set. Provenance: a
  benchmark scored 2/8 with path-only briefs versus 8/8 with pasted content. It also names what must
  *never* be pasted: per-kernel answers and prior worked examples are warm-tier only and would leak the
  answer in a cold run.
- **Strict index separation.** Hypothesis-generation material and analysis-reference material live in
  different files with mutually exclusive cardinal rules — `model-optimization-index.md` /
  `kernel-optimization-index.md` may hold *only* material that helps generate a falsifiable hypothesis;
  `profile-analyzer-index.md` may hold *only* analysis reference and "no hypothesis logic." Each index is
  read by exactly one role at exactly one step. This is sub-wiki scoping made structural: rather than
  trusting an agent to select relevant pages from the whole wiki, each role is handed a curated slice whose
  scope is enforced at authoring time.
- **Generation-scope labelling.** The kernel index separates what is *hardware-invariant* (the core
  thesis, the intervention-class decision, the ordering, the dispatch floor, the parity discipline — which
  it claims mostly transfer to GPU/Triton too) from what **must be re-derived per target** (tile edges,
  memory budgets, bandwidth ratios, every measured block size and speedup), and recommends *querying* the
  constants rather than hardcoding them. Treating measured numbers as calibration for the *shape* of an
  answer rather than as targets is a durable habit for any performance wiki.

Two more structural conventions round it out. **Logging is two-tier** — a global `wiki/log.md` for
cross-cutting ops and a per-lane log for loop iterations — because loop-rate entries (10s–100s per session)
would drown a single file and because one writer per lane makes merge conflicts vanish by construction;
routing between the tiers is a LINT contract, and only the loop-iteration op may use the one-line form.
And **the repo model is one infra wiki plus one private repo per model family**, with an explicit rule to
**promote** anything general (a concept, a reusable observation, a kernel pattern) up to the shared
template rather than re-deriving it per project.

## Reported results (context, not methodology)

The README reports two case studies, useful mainly as evidence that the methodology ports across agents:

- **Model lane** — Qwen3-8B on one v6e-8, four harnesses running the loop unattended end to end. Codex
  GPT-5.5 (47.3% MFU @2k, 40.5% @8k) and Claude Fable 5 (40.5% / 39.9%) both beat the hand-optimized
  MaxText reference (36.6% / 39.8%) autonomously; Claude Opus 4.8 (35.8% / 34.6%) and Antigravity Gemini
  3.1 Pro (33.0% / 30.6%) did not.
- **Kernel lane** — GQA attention on one v6e chip, scored against a hand-tuned reference's published 2.48×.
  All three agents beat it: Claude Opus 5 **6.77×** over 22 experiments, Codex GPT-5.6 3.73× over 9, Gemini
  Flash 3.6 3.51× over 12. These are one family's numbers from a live campaign as published in the README's
  interactive explorer at the time of this ingest, not a frozen benchmark — the ordering is the durable
  part, the per-arm decimals are not.

Both are described the same way, and the description is the interesting part: progress is *"not smooth but
a staircase of step-changes separated by long flat stretches of failed hypotheses, which is what an honest
search looks like."* Most experiments do not move the frontier — which is precisely why the stop rules
above are written to prevent stopping on the flat stretches.

## Gaps & caveats

- This summary omits the source repo's TPU-domain content: the ingested reference codebases, the ~3,580
  per-model and per-kernel pages, the technique concept pages, and the specific flag/kernel names inside
  the indexes and blueprint. The index/blueprint/class files *were* clipped because the *ordering
  discipline* and *lookup-before-hypothesizing* pattern they encode is methodology even though today's
  content instantiates it for TPU.
- The `profile-analyzer-index.md` body (an xprof/HLO tool reference) was not clipped as it is
  domain-technical throughout; its methodological role — the strict cardinal-rule separation from the
  hypothesis-generation indexes — is cited from `SCHEMA.md` instead.
- Most rules in the kernel lane are justified by a *single* named incident. That is honest provenance and
  makes the rules auditable, but it also means the evidence for each individual rule is one observation,
  not a controlled comparison. The two that do carry a measured comparison are the brief-pasting rule
  (2/8 vs 8/8) and the harness case studies above.
- The re-ingest is from the **private fork**; the public template lags it (the harness comparison in
  [§9](2026-08-06-harness-extensibility-comparison.md) notes concrete drift between the two, e.g. a Codex
  `Stop` hook still present publicly but retired privately).

## Connections
- [karpathy/autoresearch — overview](../code/autoresearch/overview.md) — the seed idea this wiki
  specializes and generalizes; side-by-side in
  [topics/wiki-driven-autoresearch-loop.md](../topics/wiki-driven-autoresearch-loop.md).
- [`concepts/llm-kernel-generation.md`](../concepts/llm-kernel-generation.md) — the new kernel lane placed
  against KernelEvolve and AlphaEvolve/openevolve on the **directed vs. selection-driven** axis; the
  auto-optimization-topic view is
  [here](../topics/auto-optimization.md#the-tpu-autoresearch-wikis-kernel-lane--the-directed-alternative).
- [`concepts/verification-independence.md`](../concepts/verification-independence.md) — the author ≠
  grader separation, and how each system in this wiki implements (or skips) it.
- [Harness Extensibility comparison](2026-08-06-harness-extensibility-comparison.md) — the same project's
  design reference for running one protocol across three agent harnesses.
- [Auto-optimization](../topics/auto-optimization.md) · [Autoresearch](../topics/autoresearch.md)

## Sources
- [`README.md`](../../raw/papers/tpu-performance-autoresearch-wiki/README.md) ·
  [`SCHEMA.md`](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md)
- Procedural specs:
  [`experiments-program.md`](../../raw/papers/tpu-performance-autoresearch-wiki/experiments-program.md)
  (model-lane root) ·
  [`kernel-experiments-program.md`](../../raw/papers/tpu-performance-autoresearch-wiki/kernel-experiments-program.md)
  (kernel-lane root, K0–K9) ·
  [`sample-program.md`](../../raw/papers/tpu-performance-autoresearch-wiki/sample-program.md)
  (the earlier template, retired upstream — kept for provenance)
- Knowledge files:
  [`model-optimization-index.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-index.md) ·
  [`model-optimization-blueprint.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-blueprint.md) ·
  [`kernel-optimization-index.md`](../../raw/papers/tpu-performance-autoresearch-wiki/kernel-optimization-index.md) ·
  [`BRIEFS.md`](../../raw/papers/tpu-performance-autoresearch-wiki/BRIEFS.md) ·
  [`design-class-catalog.md`](../../raw/papers/tpu-performance-autoresearch-wiki/design-class-catalog.md) ·
  [`classes-attention.md`](../../raw/papers/tpu-performance-autoresearch-wiki/classes-attention.md)
- [`regenerate-prompts/`](../../raw/papers/tpu-performance-autoresearch-wiki/regenerate-prompts/) — four
  checked-in prompts that rebuild the derived knowledge files
- [`skills/`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/) —
  `{create-experiment, formulate-hypothesis, start-experiment, stop-experiment, create-retrospective,
  ingest-source, edit-model-code, lint}` (updated) + `{author-kernel, formulate-kernel-hypothesis}` (new)
- [`agents/`](../../raw/papers/tpu-performance-autoresearch-wiki/agents/) —
  `{process-auditor, kernel-verifier, profile-analyzer, wikify-repo-navigator}`
- Original repos: https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki (public template;
  first ingest was commit `3344c6a`) and its private fork, re-ingested at `fa480a17` (2026-08-05)
