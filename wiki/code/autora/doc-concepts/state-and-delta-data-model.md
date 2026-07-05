---
title: The State/Delta data model
type: doc-concept
provenance: doc
source: docs/terminology.md, README.md
updated: 2026-07-05
status: fresh
---
# The State/Delta data model

## Definition
`docs/terminology.md` defines the abstraction that threads through every stage of the
[closed-loop research cycle](closed-loop-research-cycle.md): a **State** is "an object representing
data from an experiment, like the conditions, observed experiment data and models," and it "includes
rules on how to update those data if new data are provided using the 'Delta mechanism'." A **Delta** is
"an object with new data that can be added to a State, returning a new State which includes the new
data" — i.e. state updates are immutable/functional, not in-place mutation. **StandardState** is "an
optional default State" with four named fields: `variables`, `conditions`, `experiment_data`, `models`.
Around this, a **Wrapper** is a "special function that makes the components of AutoRA able to operate
on State objects," and a **Workflow** is "a collection of tools that enable closed-loop empirical
research."

## In autora (grounded)
Nothing in this repo's own 16-symbol SCIP graph implements `State`/`Delta`/`StandardState` — per
[`test_core_imports`](../catalog/tests/test_core_imports.md#test_core_imports), those live in the
sibling `autora-core` package (imported here only as `autora.variable`, `autora.utils`,
`autora.workflow`, none of which resolve to local symbols since the package isn't vendored in this
repo). What *is* visible is how the terminology table scopes each field's readers: `variables`,
`conditions` are read/written by all three components (Experimentalists, Experiment Runners,
Theorists); `experiment_data` is written by the Experiment Runner and read by the Theorist; `models` is
written by the Theorist and read back by the Experimentalist on the next cycle — which is the whole
mechanism by which "each result feeds into the next decision" (the wiki's cross-cutting
[`closed-loop-experiment-design`](../../../concepts/closed-loop-experiment-design.md) axis). The
README's worked example shows the pattern concretely: `experimentalist = on_state(random_pool,
output=["conditions"])` and `theorist = estimator_on_state(BMSRegressor(epochs=100))` are **Wrappers**
— they adapt a plain function/estimator to read named fields off a `StandardState` and write back a
`Delta` — and the loop body `s = experimentalist(s, ...)`; `s = experiment_runner(s, ...)`; `s =
theorist(s)` is exactly "a new State returned, including the new data" repeated once per role, per
cycle.

> [!inferred]
> The exact implementation of `on_state`/`estimator_on_state` (decorator-style adapters vs. wrapper
> classes) is not groundable here — it lives in `autora-core`, outside this repo's indexed surface.

## Why it matters / when it applies
This is the piece that lets AutoRA's three roles be **independently pluggable** — the terminology
table's "Relevant Modules" column lists Experimentalists, Experiment Runners, and Theorists as all
consuming the same `Variables`/`Conditions`/`Experiment Data`/`Model` vocabulary, which is precisely
what lets any experimentalist implementation in
[experimentalist-component-family](experimentalist-component-family.md) compose with any theorist in
[theorist-component-family](theorist-component-family.md) and any runner in
[experiment-runner-component-family](experiment-runner-component-family.md) without those packages
depending on each other directly — they only need to agree on the shape of the `State`.

## Connections
- Code concepts: _none — this silo has zero synthesized code concept pages (see the Overview for why)._
- Module catalogs: [tests/test_core_imports](../catalog/tests/test_core_imports.md).
- Related doc-concepts: [closed-loop-research-cycle](closed-loop-research-cycle.md),
  [experimentalist-component-family](experimentalist-component-family.md),
  [experiment-runner-component-family](experiment-runner-component-family.md),
  [theorist-component-family](theorist-component-family.md).

## Source
Extracted from `docs/terminology.md` and `README.md` (kept in place).
