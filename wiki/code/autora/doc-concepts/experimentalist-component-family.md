---
title: The experimentalist component family
type: doc-concept
provenance: doc
source: docs/experimentalist/index.md
updated: 2026-07-05
status: fresh
---
# The experimentalist component family

## Definition
`docs/experimentalist/index.md`: "The primary goal of an experimentalist is to identify experiments
that yield scientific merit." Concretely, an experimentalist is a function that takes some combination
of the current candidate models $M$ (from the theorist), the conditions already probed $X'$, and their
observations $Y'$, and returns new **conditions** — a vector of independent-variable values — that are
"intended to yield novel observations." The doc's table enumerates nine experimentalist
implementations, each shipped as its own separately-published, separately-versioned PyPI/GitHub package
— mostly under the `autora-experimentalist-*` naming convention, except **Mixture**, which ships as the
independently-named `mixture-experimentalist`: **Random** (pool + uniform sample, in
`autora-core` itself), **Novelty** (pairwise-distance novelty vs. existing conditions), **Uncertainty**
(model uncertainty, three variants), **Model Disagreement** (disagreement between theorist models),
**Falsification** (samples where the current best model's predicted loss is highest — i.e. actively
seeks conditions that could disprove the leading model), **Mixture** (weighted combination of other
strategies' scores), **Nearest Value**, **Leverage** (iterative leave-one-out refit), and
**Inequality** (pairwise-distance-threshold scoring).

> [!inferred]
> `pyproject.toml` declares an additional `experimentalist-bandit-random` extra
> (`autora-experimentalist-bandit-random`) not yet listed in this doc's table — the packaging manifest
> is slightly ahead of the documentation.

## In autora (grounded)
None of these nine cataloged packages (nor the undocumented `bandit-random` extra) are vendored in
`AutoResearch/autora` itself — the metapackage only
*declares* the dependency edges (`pyproject.toml`'s `autora[experimentalist-*]` extras, one per row of
this table), each pointing at a distinct GitHub repo. This repo's own indexed surface has no
`autora.experimentalist.*` symbols at all — [`test_core_imports`](../catalog/tests/test_core_imports.md#test_core_imports)
imports the bare `autora.experimentalist` namespace (giving you Random, the only one bundled with
`autora-core`) but none of the nine opt-in extras.

## Why it matters / when it applies
The **Falsification** strategy is the closest this catalog comes to a self-critical loop within a
single cycle — it explicitly samples conditions expected to be *worst* for the current best model,
rather than merely novel or uncertain ones, which is a different exploration principle than the
tree-search/evolutionary silos elsewhere in this wiki use (see
[agentic-tree-search](../../../concepts/agentic-tree-search.md),
[evolutionary-algorithm-discovery](../../../concepts/evolutionary-algorithm-discovery.md)): those
search over *code* or *experiment trajectories* directly; an AutoRA experimentalist searches over the
next physical/behavioral *experimental condition* to run, keeping the model-fitting (theorist) and
condition-selection (experimentalist) concerns strictly separated via the shared
[State/Delta](state-and-delta-data-model.md) object.

## Connections
- Code concepts: _none — this silo has zero synthesized code concept pages (see the Overview for why)._
- Module catalogs: none locally (no `autora.experimentalist.*` symbols are present in this repo's SCIP
  index; see [tests/test_core_imports](../catalog/tests/test_core_imports.md) for the one that is).
- Related doc-concepts: [closed-loop-research-cycle](closed-loop-research-cycle.md),
  [state-and-delta-data-model](state-and-delta-data-model.md),
  [theorist-component-family](theorist-component-family.md),
  [experiment-runner-component-family](experiment-runner-component-family.md).

## Source
Extracted from `docs/experimentalist/index.md` (kept in place).
