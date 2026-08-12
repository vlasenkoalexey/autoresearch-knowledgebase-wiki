---
title: Trainable atomic operators (Draft / Improve / Debug / Crossover)
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-06
status: fresh
---
# Trainable atomic operators (Draft / Improve / Debug / Crossover)

## Definition
The README's own framing: OpenMLE "aligns post-training and inference around a shared action space" built
from four operators — **Draft** (generate a program from scratch), **Improve** (refine a parent program using
execution feedback), **Debug** (repair a failing program), and **Crossover** (recombine two parent programs).
The same four are, per the README, "trained via execution-grounded SFT and RL... then composed into
long-horizon search" — one vocabulary meant to span post-training and inference-time search alike.

## In openrsi (grounded)
Every `Program` record across the three layers this ingest covers carries a `generation_mode` field typed to
exactly these four values: [`Program.generation_mode`](../catalog/OpenMLE-Evo/tts_search/program_database.md#Program.generation_mode)
in OpenMLE-Evo's storage layer and [`Program.generation_mode`](../catalog/OpenMLE-ERL/SFT/tts_search/program_database.md#Program.generation_mode)
in OpenMLE-ERL/SFT's are the same shape, and [`SearchEvent.generation_mode`](../catalog/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.md#SearchEvent.generation_mode)
persists it into the append-only lineage log. `build_prompt` in both
[`OpenMLE-ERL/RL`](../catalog/OpenMLE-ERL/RL/prompt_builder.md#build_prompt) and
[`OpenMLE-Evo`](../catalog/OpenMLE-Evo/tts_search/prompt_builder.md#build_prompt) dispatches per-operator to a
distinct prompt template — the "shared action space" the README describes.

**However, reading the wired code paths this ingest could ground shows the four-operator vocabulary is not
uniformly realized.** [`GreedySearch.select`](../catalog/OpenMLE-ERL/SFT/tts_search/greedy.md#GreedySearch.select) —
the only concrete `SearchAlgorithm` the SFT collection scheduler ships — only ever assigns `generation_mode`
`"draft"` or `"improve"`; "Debug" there is a parent-selection heuristic *inside* Improve (pick a program with
non-positive reward as the parent), not a distinct prompt template, and "Crossover" never appears in that path
at all. The RL rollout this packet cites has the same shape (see the concept pages linked below). The one
place `generation_mode` genuinely reads `"debug"`/`"crossover"` is the **vendored** AIRA-Dojo `Evolutionary`
solver's own operator methods, wrapped by `single_task_runner.py` — outside the primary code paths this
ingest grounded.

## Why it matters / when it applies
This is the README's headline design claim — "the same operators are trained via execution-grounded SFT and
RL... then composed into long-horizon search, coupling learning and evolution in a single loop" (paper
abstract) — and it is the central organizing idea of the whole repository: one small operator vocabulary
reused as SFT/RL training targets *and* as inference-time search moves, rather than a bespoke scheme per
stage. It matters to a reader precisely because the claim is stronger than what the wired-in code
demonstrates for Debug/Crossover — see the overview's dedicated comparison table for the full picture across
every layer.

## Connections
- Code concepts: [`OpenMLE-ERL-SFT-tts_search-services-tree_search_state`](../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md) —
  the durable event log this vocabulary is written into, and the page that first traced the Debug/Crossover
  gap to the vendored solver; [`OpenMLE-ERL-SFT-tts_search-services-scheduler`](../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md) —
  the SFT collection orchestrator whose wired `GreedySearch` only emits Draft/Improve;
  [`OpenMLE-ERL-SFT-tts_search-program_database`](../concepts/OpenMLE-ERL-SFT-tts_search-program_database.md) —
  independently confirms the same finding from the parent-database side;
  [`OpenMLE-Evo-tts_search-program_database`](../concepts/OpenMLE-Evo-tts_search-program_database.md) — the
  storage substrate that carries `generation_mode` at the inference-time-search layer, with no concrete
  selection policy implemented against it in this packet;
  [`OpenMLE-ERL-RL-airaevo_experience`](../concepts/OpenMLE-ERL-RL-airaevo_experience.md) — the RL harness's
  own adapter for the vendored AIRA-Evo baseline.
- Module catalogs: [`OpenMLE-ERL/SFT/tts_search/greedy.md`](../catalog/OpenMLE-ERL/SFT/tts_search/greedy.md),
  [`OpenMLE-ERL/RL/prompt_builder.md`](../catalog/OpenMLE-ERL/RL/prompt_builder.md),
  [`OpenMLE-Evo/tts_search/prompt_builder.md`](../catalog/OpenMLE-Evo/tts_search/prompt_builder.md).
- Related doc-concepts: [`shared-action-space`](shared-action-space.md) — the storage-shape side of the same
  claim.
- Cross-repo: [`program-evolution-operators`](../../../concepts/program-evolution-operators.md) — how this
  Draft/Improve/Debug/Crossover vocabulary compares against AIDE-style operators in this wiki's other silos.

## Source
Extracted from `README.md` (sections "🧩 OpenMLE: The Executable Stack" → "Trainable Atomic Operators", and
the paper abstract quoted in "🚀 Frontis-MA1"), kept in place.
