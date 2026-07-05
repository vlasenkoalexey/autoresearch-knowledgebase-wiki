---
title: The theorist component family
type: doc-concept
provenance: doc
source: docs/theorist/index.md
updated: 2026-07-05
status: fresh
---
# The theorist component family

## Definition
`docs/theorist/index.md`: "AutoRA consists of a set of techniques designed to automate the construction
of interpretable models from data," framed as discovering small **computation graphs** that map
experimental conditions (e.g. stimulus brightness) to observed dependent measures (e.g. detection
probability). A theorist consumes the conditions already probed $X'$ and their observations $Y'$ — the
`experiment_data` field of the [shared State](state-and-delta-data-model.md), populated by the
[experiment runner](experiment-runner-component-family.md) — and returns a fitted **model**, which is
written back to `state.models` for the next
[experimentalist](experimentalist-component-family.md) call to read. The doc lists three implemented
theorists: **BMS** (Bayesian Machine Scientist — algorithmic Bayesian symbolic regression), **BSR**
(Bayesian Symbolic Regression — a second, distinct algorithmic approach to the same problem), and
**DARTS** (Differentiable Architecture Search — makes architecture search amenable to gradient
descent). All three target the same goal (interpretable expressions/architectures that fit $X',Y'$)
via different search strategies.

## In autora (grounded)
As with the other two component families, none of `autora-theorist-bms`, `autora-theorist-bsr`, or
`autora-theorist-darts` is vendored in this repo — each is declared only as a `pyproject.toml` extra
(`autora[theorist-bms]`, etc.) pointing at its own package/repo, and none of their symbols appear in
this repo's 16-symbol SCIP index. The README's worked example names one of them directly —
`from autora.theorist.bms import BMSRegressor` — as the theorist used in the `sin(x)` discovery
walkthrough, wrapped via `estimator_on_state(BMSRegressor(epochs=100))` to read/write the
[shared State](state-and-delta-data-model.md).

## Why it matters / when it applies
DARTS is the notable outlier of the three: it is itself a **neural-architecture-search** method
(gradient-based, differentiable) repurposed here as a *theorist* — i.e. the same auto-optimization
technique this wiki catalogs elsewhere under NAS is being applied to discover a scientific model's
functional form rather than a classifier's architecture. BMS and BSR instead do symbolic regression —
searching directly over interpretable closed-form expressions rather than over network topologies —
which is the more central case for AutoRA's "interpretable model" framing, since a DARTS-discovered
computation graph still needs a separate interpretation step to read off as a scientific claim.

## Connections
- Code concepts: _none — this silo has zero synthesized code concept pages (see the Overview for why)._
- Module catalogs: none locally (no `autora.theorist.*` symbols are present in this repo's SCIP index).
- Related doc-concepts: [closed-loop-research-cycle](closed-loop-research-cycle.md),
  [state-and-delta-data-model](state-and-delta-data-model.md),
  [experimentalist-component-family](experimentalist-component-family.md),
  [experiment-runner-component-family](experiment-runner-component-family.md).

## Source
Extracted from `docs/theorist/index.md` (kept in place).
