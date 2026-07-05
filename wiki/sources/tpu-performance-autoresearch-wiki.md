# tpu_performance_autoresearch_wiki — methodology summary

A Karpathy-LLM-wiki-pattern knowledge base that specializes
[karpathy/autoresearch](../code/autoresearch/overview.md)'s "agent runs an autonomous experiment loop"
idea from *LLM quality* to *TPU model performance* (step time, MFU, tokens/sec, memory), and generalizes
it into a full research-operations schema: a page-type taxonomy, a hierarchical procedural spec, and eight
callable skills that implement each stage of the loop. This summary covers **only the methodology** —
the loop, schema, and skills — not the ~26 ingested reference codebases, the 900+ per-model experiment
logs, or the TPU-domain technical content (concepts, sources, blueprint specifics) that fill out the rest
of that wiki. Full clips of the methodology files live in
[`raw/papers/tpu-performance-autoresearch-wiki/`](../../raw/papers/tpu-performance-autoresearch-wiki/).

## Overview

The source repo (`vlasenkoalexey/tpu_performance_autoresearch_wiki`) restates
[Karpathy's autoresearch loop](../code/autoresearch/overview.md) — hypothesize → experiment → observe →
revise — as a **domain-agnostic optimization loop** and then instantiates it fully for TPU performance
work: an LLM agent edits real model code on a git branch, runs it on real hardware, profiles it through an
MCP-wrapped profiler (XProf) instead of judging loss, and records every experiment — win or loss — into a
markdown wiki that becomes the prior for the next hypothesis
([README](../../raw/papers/tpu-performance-autoresearch-wiki/README.md)). The wiki is explicitly framed as
a low-cost alternative to RAG: `grep`-based retrieval over a schema-shaped, cross-linked set of markdown
pages instead of an embedding pipeline
([README](../../raw/papers/tpu-performance-autoresearch-wiki/README.md)).

## The methodology

### The loop and its substrate
[`SCHEMA.md`](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md) states the loop as: ingest
knowledge (papers, docs, codebases, profiles) → formulate ranked hypotheses → run experiments → record
observations → update priors → formulate next hypotheses. It draws a hard scope line — only step time,
MFU, tokens/sec, memory and what affects them are in scope; **any change that alters model semantics is
`invalid`, and its speedup is not reported** — the same "don't let the agent game the metric" discipline
`autoresearch`'s frozen `prepare.py` enforces via a fixed evaluation harness (see
[prepare.py — the frozen substrate](../code/autoresearch/concepts/prepare.md)), here generalized from "the
eval code is read-only" to "changing what the model *computes* voids the result."

### A page-type schema instead of a flat ledger
Where `karpathy/autoresearch`'s `program.md` uses one flat `results.tsv` per run
(see [experiment logging](../code/autoresearch/doc-concepts/experiment-logging.md)), this wiki
generalizes the ledger into eight page types, each with a mandatory frontmatter + section template
([SCHEMA.md](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md)): `source` (ingested
paper/doc), `codebase` (ingested repo), `concept` (a technique/flag/kernel), `model` (one
`(architecture, lane)` pair — the *lane* axis is treated as fundamental, since a different framework means
a different code path and debugging context, while *size* and *hardware* are "combinatorial accidents
over the same code"), `hypothesis` (a falsifiable candidate, ranked by
`expected_gain × confidence / effort`), `experiment` (one run against one hypothesis on one variant),
`observation` (a reusable finding extracted from a profile), and `analysis` (a synthesis). Contradictions
are never silently overwritten — a superseded claim is wrapped in a `> [!warning] Contradicted by …`
block with the new claim added below it, left for a human to adjudicate.

### The `program.md` hierarchy — generic spec, model overrides, lane overrides
`SCHEMA.md` is the **structural** spec (page types, layout, rules); the **procedural** spec — how to
actually execute the loop step by step — lives in a three-layer `program.md` hierarchy: a generic root
(`sample-program.md`), a model-family layer, and an optional lane layer, resolved *root → model → lane*
with **replace-per-section** semantics (the most specific file that defines an H2 section wins outright;
a child that doesn't define a section inherits it unchanged) — the same idea as CSS cascade specificity,
applied to procedure instead of style
([sample-program.md](../../raw/papers/tpu-performance-autoresearch-wiki/sample-program.md),
[SCHEMA.md](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md)).

### Falsifiability and pre-flight cost screening
Every hypothesis must state its expected metric delta and how it would be measured before it's ranked
(`SCHEMA.md` → `FORMULATE-HYPOTHESIS`). Two screening steps sit ahead of spending real hardware time: an
**HLO pre-filter** — before proposing to replace XLA-generated code with a hand-written kernel, AOT-compile
the baseline and check whether XLA already fused the target pattern into one kernel; if so, retire the
hypothesis immediately (`status: retired`, reason `xla-already-fuses`) rather than spend a run proving it
— and an optional **AOT cost-analysis screen** — compile the modified function and compare
`.cost_analysis()` FLOPs/bytes/optimal-seconds against baseline *before* committing to a full run
([SCHEMA.md](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md) → `FORMULATE-HYPOTHESIS` step
2b, `RUN-EXPERIMENT` step 1b). Both are cheap ways to refute a hypothesis on a CPU/compiler pass instead of
burning a real training run on it — the same instinct behind `autoresearch`'s fast-fail NaN/loss guard (see
[train.py — Edge cases](../code/autoresearch/concepts/train.md)), applied one step earlier in the pipeline.

### Mandatory "next hypotheses" — keeping the queue non-empty
Every experiment page must end with a `## Next hypotheses` section enumerating concrete follow-up
candidates, each filed as a real (stub) hypothesis page in the same change — an empty or missing section
fails lint. The rationale stated directly: *"the experiment that just landed is the cheapest moment to
capture the next move while the context is fresh"*
([SCHEMA.md](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md) → `experiment` page format).
This is a durable, generalizable discipline for any autoresearch-style loop: don't let idea generation
depend on someone remembering to come back to it later.

### The `formulate-hypothesis` skill — three-layer prior lookup
[`formulate-hypothesis`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/formulate-hypothesis.md)
is the skill that turns "propose the next experiment" into a disciplined lookup rather than a guess. It
reads three layers in full before proposing anything: (1) a **generic topic index** mapping observed
profile signatures to likely mechanisms and cross-model refuted-pattern principles, (2) a **generic
optimization blueprint** giving phase ordering, compounding rules, and trap awareness, and (3) a
**per-model refuted-patterns layer** plus the model page and recent experiments for variant-specific prior
refutations. It runs in four modes — `frontier` (full ceremony, a measured best exists and regression is
costly), `exploration` (lighter ceremony for stalled variants or hunches), `bootstrap` (brand-new model,
thin state, first-principles reasoning from the generic layers), and `user-override` (validate a
human-specified candidate rather than generate one) — and its output is a structured proposal recording
which index/blueprint sections were consulted, which refuted patterns were checked against, the
falsification criterion, expected gain, effort, and a duplicate-track check against in-flight experiments.
A hard rule up front: **never skip this skill before proposing a hypothesis** — the stated justification is
a real incident where skipping the precedent check let a 200× regression class recur.

### The optimization blueprint — a generic ordering discipline
[`model-optimization-blueprint.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-blueprint.md)
distills a **generic ladder** (its word) from hundreds of experiments across multiple model families: work
cheap-to-expensive, phase by phase — substrate sanity checks (things that cost ~nothing but invalidate every
downstream measurement if skipped, e.g. profiler-off, loss-trajectory sanity, "did the change actually take
effect") → cheap memory/precision levers → known-good flag bundles → kernel/structural code work (the
biggest but most expensive wins) → batch/sequence amortization → cross-variant/cross-generation transfer →
**exploratory flag sweeps last, as a last resort** — because in the data, undirected flag-sweeping is the
lowest-yield activity in the ledger, while the highest-yield flag work is applying already-known-good
bundles. The generalizable claim: exploration should be ordered by (yield ÷ cost), applied only after
cheaper, higher-confidence levers are exhausted, and a "verify the change actually happened" check belongs
at the very front of *every* phase, not just as an afterthought when a result looks surprising.

### Retrospectives — a coverage-gap audit before declaring a search exhausted
[`create-retrospective`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/create-retrospective.md)
exists specifically to counter premature exhaustion: it re-reads **every** experiment page in a lane (not a
sample — "coverage is the whole point"), builds a categorized ledger against the generic topic taxonomy,
detects imbalance signatures (e.g. many single-flag probes but no kernel-level work tried) and
stuck-frontier duration, and ranks unexplored directions — explicitly triggered by the agent saying "I'm
out of ideas," and justified by a named incident: a lane was declared exhausted, and a kernel port that
landed +4.18 pp MFU shipped one week later. It is read-only over its own recommendations — a separate step
(`/formulate-hypothesis`) decides what to actually run next. This generalizes past TPU work directly: any
long-running autonomous search needs a periodic "did I actually cover the space, or did I just get tired"
audit distinct from the moment-to-moment hypothesis proposer.

### Coding discipline for the agent's edits — `edit-model-code`
[`edit-model-code`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/edit-model-code.md) adapts
Karpathy's general LLM-coding guidelines (think before coding, simplicity first, surgical changes,
goal-driven execution) to an autonomous loop that can't pause to ask clarifying questions: state
assumptions in the experiment page rather than interrupting; test exactly one mechanism per experiment (if
a five-line idea needs 200 lines of plumbing, the hypothesis is probably wrong); touch only what the
hypothesis requires — the fork is throwaway, the trunk is not; and treat the training run itself as the
test ("refuted" is a valid, successful outcome — don't tune the test to avoid it). Two invariants are called
out as non-negotiable: **no semantics drift** (bf16 stays bf16, output distribution must match baseline
within numeric noise, or the verdict is `invalid` — never fix this by loosening the comparison), and **no
silent fallback paths in kernel code** (a kernel that fails should crash loudly, not silently degrade to a
slower path, because a silent fallback destroys the loop's ability to distinguish "kernel didn't fire" from
"kernel fired and lost").

### Bootstrap, launch, and shutdown skills
[`create-experiment`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/create-experiment.md)
scaffolds a brand-new model family (asks for lanes/sizes/hardware/sequence length, then writes the
folder structure, a model-level `program.md`, and model-page stubs) — explicitly interactive
("do NOT silently write files without confirming"). [`start-experiment`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/start-experiment.md)
resolves the three-layer `program.md`, does hardware/cluster discovery and an occupancy check, then starts
the loop — optionally in a **never-stop mode**, where a marker file plus a registered Stop hook blocks the
session from ending until a fresh (within 6 hours), lane-specific retrospective exists; this is a concrete
accountability mechanism for autonomous "run until interrupted" loops, an idea the plain
[`autoresearch` program.md](../code/autoresearch/doc-concepts/autonomous-experiment-loop.md) states only as
a policy ("NEVER STOP") rather than as an enforced gate.
[`stop-experiment`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/stop-experiment.md) is the
reverse: cancel scheduled continuations, reap orphaned cluster workloads (with a human-in-the-loop
disposition for each: let it finish / kill as inconclusive / kill as killed-by-master), resolve any
in-progress experiment stubs, run lint, and append a clean-shutdown marker — so a later session can tell a
clean stop from a crash by reading the log.

### `ingest-source` and `lint` — keeping the substrate coherent
[`ingest-source`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/ingest-source.md) encodes a
**discuss-before-write** discipline: draft the key claims and proposed connections, surface them to the
human, and only write the source page and update cross-links after explicit confirmation — "getting
emphasis wrong propagates downstream into bad hypothesis proposals." It never silently overwrites an
existing source page on re-ingest, and it uses the same `[!warning]` contradiction convention as the rest
of the schema. [`lint`](../../raw/papers/tpu-performance-autoresearch-wiki/skills/lint.md) implements
SCHEMA's `LINT` operation as ~23 structural invariant checks (orphan pages, broken links, missing
experiment sections, stuck in-progress stubs, stale codebase pins, log-routing violations, and a
"hook-health" check on the never-stop loop's own Stop-hook wiring — treated as the loop's *control plane*,
whose silent failure would defeat the discipline invisibly). It auto-fixes mechanical issues and surfaces
judgment calls as a punch list; it never auto-commits and never adjudicates a contradiction itself.

## Gaps & caveats
This summary deliberately omits the TPU-domain-specific content of the source repo: the ~26 ingested
reference codebases (JAX, MaxText, tokamax, torchax, etc.), the 900+ per-model experiment logs, the
TPU-technique concept pages (flash attention, HBM, ICI, …), and the specific flag/kernel names inside the
optimization blueprint and index — those are implementation detail for TPU performance work specifically,
not general autoresearch methodology, and were excluded on request. The blueprint/index files *were*
pulled in because the *ordering discipline* and *lookup-before-hypothesizing* pattern they encode is
methodology, even though today's content instantiates it for TPU flags and kernels.

## Connections
- [karpathy/autoresearch — overview](../code/autoresearch/overview.md) — the seed idea this wiki
  specializes and generalizes; see the new synthesis at
  [topics/wiki-driven-autoresearch-loop.md](../topics/wiki-driven-autoresearch-loop.md) for a side-by-side.

## Sources
- [`raw/papers/tpu-performance-autoresearch-wiki/README.md`](../../raw/papers/tpu-performance-autoresearch-wiki/README.md)
- [`raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md`](../../raw/papers/tpu-performance-autoresearch-wiki/SCHEMA.md)
- [`raw/papers/tpu-performance-autoresearch-wiki/sample-program.md`](../../raw/papers/tpu-performance-autoresearch-wiki/sample-program.md)
- [`raw/papers/tpu-performance-autoresearch-wiki/model-optimization-blueprint.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-blueprint.md)
- [`raw/papers/tpu-performance-autoresearch-wiki/model-optimization-index.md`](../../raw/papers/tpu-performance-autoresearch-wiki/model-optimization-index.md)
- `raw/papers/tpu-performance-autoresearch-wiki/skills/{create-experiment,formulate-hypothesis,start-experiment,stop-experiment,create-retrospective,ingest-source,edit-model-code,lint}.md`
- Original repo: https://github.com/vlasenkoalexey/tpu_performance_autoresearch_wiki (commit `3344c6a`)
