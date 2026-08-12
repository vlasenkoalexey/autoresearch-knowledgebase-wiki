# Schema — Frontier Models with Our Harness Achieve ~99% on ARC-AGI-3 Public

Impossible Research (led by incoming PhD student Guanning Zeng, with Jiani Wang, Wenjie Ma, Shaofeng Yin,
Chenyang Wang, Shichen Liu, Angjoo Kanazawa, Wode Ni, Xiuyu Li, Andrea Zanette — UC Berkeley / Carnegie
Mellon affiliations among the team) — [schema-harness.github.io](https://schema-harness.github.io/), a
project announcement page rather than a paper. Ingested 2026-08-12 as the harness that crossed the
[ARC-AGI-3](arc-agi-3.md) human-expert baseline **before** [Prime Agent](prime-agent-launch.md)'s launch
post, and as the site of the sharpest public methodological dispute this batch touches.

## Overview

Schema frames ARC-AGI-3 explicitly as a reinforcement-learning-flavored world-modeling problem: can an
agent discover the hidden rules of an environment it has never seen, as efficiently as a human on first
exposure? Its answer is to make the model **behave like a physicist rather than a player** — ground
objects, relations, and goals from observation; propose and test hypotheses about how they change; and
encode both current state and discovered mechanism as an **editable, symbolic (Python) world model** rather
than a latent vector.

## Key claims

- **~99% RHAE on the ARC-AGI-3 public set** with an Opus 4.8 + Fable 5 pairing; **95.35%** with GPT-5.6 Sol
  — both self-reported by the team, not administered by ARC Prize.
- **The world model is a program, not a vector** — an append-only transition record, persistent notes, and
  editable Python hypotheses that can be backtested against the *full* interaction history so far, not just
  the most recent observation.
- **Certified-model search + discriminating probes**: the harness doesn't just fit a hypothesis to what
  it's seen — it searches for hypotheses that survive backtesting against the whole log, and can propose
  probing actions specifically chosen to discriminate between two hypotheses that currently agree on
  everything observed so far.
- **Guarded action queues**: planned action sequences are invalidated as soon as a prediction from the
  current world model mismatches what actually happens, rather than executing a stale plan to the end.

## Key data points

| Signal | Value |
|---|---|
| RHAE, Opus 4.8 + Fable 5 | ~99% (self-reported) |
| RHAE, GPT-5.6 Sol | 95.35% (self-reported) |
| Administered ARC Prize record at time of publication (for comparison) | 30.2% (Claude Opus 5, [arc-agi-3.md](arc-agi-3.md)) |

## Gaps & caveats
- **The public reaction split cleanly on the core methodological question this wiki also asks about
  [Retrodict](retrodict.md) and Prime Agent**: does a harness that builds and backtests an explicit
  simulator from the interaction log still measure what RHAE was designed to measure, or does it (as one
  critique put it) amount to running a specialized solver *alongside* the model rather than testing the
  model's own reasoning? Public commentary split between calling it genuine physicist-style program
  synthesis and calling it pre-baked, hard-to-audit engineering — reviewers who looked for the harness
  code itself reported it was difficult to determine from the outside how much problem-specific human
  engineering was baked into the world-model search versus general-purpose. See
  [`concepts/verification-independence.md`](../concepts/verification-independence.md).
- **A specific "moving the goal post" characterization is quoted in the source video** for this ingest
  batch, attributed to a commenter on the Schema announcement thread — I could not independently locate
  and verify that exact quote's source in this pass, so it is not repeated here as a confirmed citation.
- **No peer-reviewed paper accompanies this result** — it is a project page + social-media announcement.
  A related, later academic paper from an overlapping research thread — *Tycho: Active Abstraction with
  Programmatic World Models for ARC-AGI-3* — pursues a similar programmatic-world-model approach and is
  not ingested here; noted for a future pass.
- **All numbers here are self-reported**, same caveat as [Retrodict](retrodict.md) and
  [Prime Agent](prime-agent-launch.md) — none of the three harnesses that crossed the human baseline before
  Prime Agent's launch had an ARC-Prize-administered run at the time of this ingest.

## Connections
- [ARC-AGI-3 benchmark](arc-agi-3.md) — the benchmark and RHAE metric Schema is scored against.
- [Retrodict](retrodict.md) — the harness that surpassed Schema's own reported number (99.86% vs. ~99%) at
  roughly a tenth of the cost, and whose README's comparison table is the source for Schema's cost figure
  cited there (≥$6,447, fixed conditional reruns, higher result retained).
- [Prime Agent launch post](prime-agent-launch.md) — the harness the source video centers on; Schema and
  Retrodict both crossed the human-expert line before Prime Agent's own launch, a fact Prime Agent's launch
  post does not foreground.
- [`concepts/verification-independence.md`](../concepts/verification-independence.md) — the
  self-reported-vs-administered and "does the harness measure the model or replace it" questions this page
  raises without resolving.

## Sources
- [Frontier Models with Our Harness Achieve ~99% on ARC-AGI-3 Public](https://schema-harness.github.io/) —
  Schema project page, Impossible Research
- [Andrea Zanette announcement thread](https://x.com/Zanette_ai/status/2077793189608775728)
