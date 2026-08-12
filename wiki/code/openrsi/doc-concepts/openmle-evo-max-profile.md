---
title: OpenMLE-Evo-Max as a search profile, not a separate source tree
type: doc-concept
provenance: doc
source: README.md
updated: 2026-08-06
status: fresh
---
# OpenMLE-Evo-Max as a search profile, not a separate source tree

## Definition
The README states this explicitly, correcting a natural misreading of the paper's naming: "OpenMLE-Evo-Max
is the asynchronous multi-GPU search profile inside `OpenMLE-Evo`, not a separate source tree." Structurally
it is two additions layered on top of ordinary OpenMLE-Evo — benchmark-independent experience priors, and
asynchronous multi-GPU parallel search "at unchanged total sandbox compute" (paper §6.1) — configured, not a
separately shipped codebase.

## In openrsi (grounded)
The "asynchronous multi-GPU" half of Evo-Max is concretely
[`airaevo_async_resources.py`](../catalog/OpenMLE-Evo/tts_search/airaevo_async_resources.md), living in the
same `OpenMLE-Evo/tts_search/` directory as every other Evo module, not under a separate tree.
[`resolve_execution_mode`](../catalog/OpenMLE-Evo/tts_search/airaevo_async_resources.md#resolve_execution_mode)
switches between `"generation"` (the ordinary, single-worker path) and `"async_steady_state"` (Evo-Max) as a
config value; [`resolve_async_worker_count`](../catalog/OpenMLE-Evo/tts_search/airaevo_async_resources.md#resolve_async_worker_count)
resolves how many parallel workers that mode gets (one per detected GPU in `"auto"` mode), and
[`build_worker_specs`](../catalog/OpenMLE-Evo/tts_search/airaevo_async_resources.md#build_worker_specs)
produces one immutable [`WorkerSpec`](../catalog/OpenMLE-Evo/tts_search/airaevo_async_resources.md#WorkerSpec)
per worker (a GPU index and a sandbox-router URL). The "unchanged total sandbox compute" half of the claim is
`resolve_task_concurrency_per_epoch`, which shrinks the outer per-task concurrency budget in proportion to
the worker count `resolve_async_worker_count` returns — more per-task search parallelism, same aggregate
concurrency ceiling.

## Why it matters / when it applies
A reader who expects `OpenMLE-Evo-Max` to be its own directory or entry point (by analogy with how
`OpenMLE-Gym`/`OpenMLE-ERL`/`OpenMLE-Evo` are three separate top-level folders) would be looking in the wrong
place; the whole feature is a config flag (`execution_mode`) plus a resource resolver, applied at launch time
to the same `OpenMLE-Evo` runtime everything else uses. This matters for reproducing the paper's split between "OpenMLE-Evo" (60.61%) and "OpenMLE-Evo-Max" (71.21%)
Medal Average numbers for Frontis-MA1-35B (Table 1) — the difference is entirely in which config values were
set for that run, not a different codebase.

## Connections
- Code concepts: [`OpenMLE-Evo-tts_search-airaevo_async_resources`](../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md) —
  the full mechanism page this doc-concept summarizes; [`OpenMLE-Evo-tts_search-program_database`](../concepts/OpenMLE-Evo-tts_search-program_database.md) —
  the storage layer the async worker pool's `Evolutionary` solver reads/writes through (out of this packet's
  subgraph, but the same `ProgramDatabase`/`Program` shape).
- Module catalogs: [`OpenMLE-Evo/tts_search/airaevo_async_resources.md`](../catalog/OpenMLE-Evo/tts_search/airaevo_async_resources.md),
  [`OpenMLE-Evo/tts_search/airaevo_concurrency.md`](../catalog/OpenMLE-Evo/tts_search/airaevo_concurrency.md).
- Related doc-concepts: [`shared-action-space`](shared-action-space.md).

## Source
Extracted from `README.md` (section "🧩 OpenMLE: The Executable Stack", the note directly under the operator
table), kept in place.
