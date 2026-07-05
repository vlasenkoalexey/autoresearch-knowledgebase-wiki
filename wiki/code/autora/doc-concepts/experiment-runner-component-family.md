---
title: The experiment-runner component family
type: doc-concept
provenance: doc
source: docs/experiment-runner/index.md
updated: 2026-07-05
status: fresh
---
# The experiment-runner component family

## Definition
`docs/experiment-runner/index.md`: "`autora` includes tools for running synthetic and real-world
experiments." An experiment runner takes conditions (produced by an
[experimentalist](experimentalist-component-family.md)) and returns observations. The doc splits this
into two very different kinds of "running an experiment":
- **Synthetic** — "a compendium of ground-truth models across psychology, psychophysics, behavioral
  economics, and other disciplines" (`autora-synthetic`): given a condition, evaluate a known equation
  and return a (possibly noised) observation. No human is involved; this is what the README's `sin(x)`
  walkthrough uses.
- **Real-world** — composed from two separable roles: an **experimentation manager** ("facilitate
  communication of conditions and observations between `autora` and environments in which experiments
  are hosted," e.g. Firebase) and a **recruitment manager** ("facilitate recruitment and coordination of
  study participants," e.g. Prolific). The doc's one shipped real-world runner,
  **Firebase-Prolific**, is literally the composition of those two: "combines the Firebase
  experimentation manager and the Prolific recruitment manager to automatically run human behavioral
  experiments."

## In autora (grounded)
As with the [experimentalist family](experimentalist-component-family.md), none of these are vendored
here — `autora-synthetic`, `autora-experiment-runner-experimentation-manager-firebase`,
`autora-experiment-runner-recruitment-manager-prolific`, and
`autora-experiment-runner-firebase-prolific` are each a separate package/repo, declared only as extras
in this metapackage's `pyproject.toml`.
[`test_core_imports`](../catalog/tests/test_core_imports.md#test_core_imports) does import
`autora.experiment_runner.synthetic` as part of the *default* install — i.e. the synthetic runner is
the one part of "running an experiment" that ships out of the box; every real-world (human-in-the-loop)
runner is opt-in.

## Why it matters / when it applies
This is the step where AutoRA's closed loop actually leaves the computer: for a real-world run, an
experiment-runner hands a generated condition to an **actual human participant** (via Prolific
recruitment + Firebase-hosted trial delivery) and waits for a genuine behavioral response before the
[theorist](theorist-component-family.md) ever sees new data — the concrete mechanism behind this wiki's
framing of AutoRA as closing the loop over *physical/behavioral* experiments rather than the in-silico
training runs, code edits, or simulated benchmarks the other autoresearch silos iterate on (see
[closed-loop-experiment-design](../../../concepts/closed-loop-experiment-design.md)). The
synthetic/real-world split also means a workflow can be developed and debugged entirely against the
synthetic runner (fast, free, reproducible) before being pointed at the real-world one for actual data
collection — the same condition-selection and model-fitting code runs unchanged either way, because
both runner kinds only need to satisfy the shared [State/Delta](state-and-delta-data-model.md)
interface.

## Connections
- Code concepts: _none — this silo has zero synthesized code concept pages (see the Overview for why)._
- Module catalogs: none locally for the runner packages themselves; see
  [tests/test_core_imports](../catalog/tests/test_core_imports.md) for the one grounded import
  (`autora.experiment_runner.synthetic`).
- Related doc-concepts: [closed-loop-research-cycle](closed-loop-research-cycle.md),
  [state-and-delta-data-model](state-and-delta-data-model.md),
  [experimentalist-component-family](experimentalist-component-family.md),
  [theorist-component-family](theorist-component-family.md).

## Source
Extracted from `docs/experiment-runner/index.md` (kept in place).
