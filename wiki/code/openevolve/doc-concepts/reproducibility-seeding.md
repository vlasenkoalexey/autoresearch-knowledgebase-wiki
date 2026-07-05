---
title: Reproducibility via hash-derived component seeding
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# Reproducibility via hash-derived component seeding

## Definition

The README advertises "Scientific Reproducibility" as a headline feature: "every component (LLM,
database, evaluation) is seeded," with a default seed of 42 giving "immediate reproducible results out
of the box," plus "Component Isolation: Hash-based isolation prevents cross-contamination." The claim
worth grounding is specifically the *hash-based isolation* part — a single top-level seed doesn't just
get broadcast identically to every random-number source; the pieces need decorrelated seeds even though
they derive from the same root, or two components sampling in lockstep could produce artificially
correlated behavior.

## In openevolve (grounded)

A single [`Config.random_seed`](../catalog/openevolve/config.md#Config.random_seed) (defaulting to
`42`) is the only user-facing knob. It fans out from
[`OpenEvolve.__init__`](../catalog/openevolve/controller.md#OpenEvolve.__init__) (see
[`openevolve-controller.md`](../concepts/openevolve-controller.md)): when `random_seed is not None`, the
constructor seeds the *global* `random` and `numpy.random` modules directly with it, then derives a
second, **different** seed for the LLM subsystem by hashing the root seed together with a literal
`b"llm"` tag (`hashlib.md5(base_seed + b"llm").hexdigest()[:8]`, taken mod `2**31`) and propagating that
derived `llm_seed` onto every model config that doesn't already carry its own explicit `random_seed`.
Separately, [`Config.database.random_seed`](../catalog/openevolve/config.md#DatabaseConfig) is set
directly from the same root `random_seed` (not hash-derived) in
[`__init__`](../catalog/openevolve/controller.md#OpenEvolve.__init__), and
[`ProgramDatabase`](../catalog/openevolve/database.md#ProgramDatabase) seeds Python's global `random`
module again with it — while [`LLMEnsemble`](../catalog/openevolve/llm/ensemble.md#LLMEnsemble) instead
seeds its own **private**
[`random_state`](../catalog/openevolve/llm/ensemble.md#LLMEnsemble.random_state) (a dedicated
`random.Random()` instance, not the global module) with whatever `random_seed` ends up on
`models_cfg[0]` — the hash-derived `llm_seed` in the common case.

## Why it matters / when it applies

The instinct to give every component the literal same seed would be simpler, but two subsystems drawing
from identically-seeded generators in the same order can end up correlated in ways that aren't obvious
from the outside (e.g. an island-selection draw and a model-selection draw moving in lockstep across
runs). Deriving the LLM seed via a hash of the root seed plus a component-specific tag string is a cheap
way to decorrelate the two draw sequences while still keeping the whole run reproducible from one number
— rerun with the same `random_seed` and every derived seed is recomputed identically, but the database's
draws and the ensemble's draws no longer track each other by construction. This is also why
`LLMEnsemble` owns a private `random.Random()` rather than calling module-level `random` functions (see
[`openevolve-llm-ensemble.md`](../concepts/openevolve-llm-ensemble.md)): a private generator per
ensemble instance is what makes per-worker-process determinism actually hold, since two worker processes
constructing their own ensembles won't perturb a shared global generator's state.

## Connections

- Code concepts: [OpenEvolve's main evolution loop](../concepts/openevolve-controller.md) — where the
  hash-derived seed fan-out happens; [Config — the knobs behind mutation, evaluation, and the population
  database](../concepts/openevolve-config.md) — the single `random_seed` field this all derives from;
  [The program database](../concepts/openevolve-database.md) and
  [LLM Ensemble](../concepts/openevolve-llm-ensemble.md) — the two components that actually consume a
  derived seed.
- Module catalogs: [openevolve/controller.py](../catalog/openevolve/controller.md),
  [openevolve/config.py](../catalog/openevolve/config.md), [openevolve/database.py](../catalog/openevolve/database.md),
  [openevolve/llm/ensemble.py](../catalog/openevolve/llm/ensemble.md).
- Related doc-concepts: none yet.

## Source

Extracted from `README.md` (kept in place), "Scientific Reproducibility" section under Advanced
Features.
