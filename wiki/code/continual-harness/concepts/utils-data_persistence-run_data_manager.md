---
title: RunDataManager — the per-run cache directory
type: concept
provenance: mixed
concept: utils-data_persistence-run_data_manager
updated: 2026-08-12
status: fresh
---
# RunDataManager — the per-run cache directory

## Overview

[`get_run_data_manager`](../catalog/utils/data_persistence/run_data_manager.md#get_run_data_manager) —
*"Get the global run data manager instance"* — and
[`get_cache_path`](../catalog/utils/data_persistence/run_data_manager.md#get_cache_path) — *"Get a path
within the run-specific cache directory"* — give every other module in this silo a shared, run-scoped
place to persist state (evolution logs, map data, metrics), the filesystem counterpart to
[`utils-stores-subagents`](utils-stores-subagents.md)'s JSON stores.

## See also
- [`agents-utils-harness_evolver`](agents-utils-harness_evolver.md) — a consumer via `_save_evolution_log`.
