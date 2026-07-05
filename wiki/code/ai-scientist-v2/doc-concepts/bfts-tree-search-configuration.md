---
title: BFTS tree-search configuration knobs
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# BFTS tree-search configuration knobs

## Definition
The best-first tree search (BFTS) that runs Stage-2 experiments is tuned entirely through
`bfts_config.yaml`, not command-line flags. The README documents two config blocks: an `agent` block
(how many exploration paths run and how far the search goes) and a `search` block (how failing nodes are
debugged and how many independent trees are grown). The headline worked example: with `num_workers=3` and
`steps=21`, the search explores up to 21 nodes total while expanding 3 nodes concurrently at each step.

## In ai-scientist-v2 (grounded)
The YAML keys map onto the dataclass fields loaded by
[`load_cfg`](../catalog/ai_scientist/treesearch/utils/config.md#load_cfg) into the top-level
[`Config`](../catalog/ai_scientist/treesearch/utils/config.md#Config) (owning module:
[`ai_scientist/treesearch/utils/config.py`](../catalog/ai_scientist/treesearch/utils/config.md)):

**`agent` block**
- `num_workers` → [`AgentConfig.num_workers`](../catalog/ai_scientist/treesearch/utils/config.md#AgentConfig.num_workers)
  — number of parallel exploration paths (concurrent node expansions).
- `steps` → [`AgentConfig.steps`](../catalog/ai_scientist/treesearch/utils/config.md#AgentConfig.steps)
  — the maximum number of nodes to explore (the "21" in the worked example).
- `num_seeds` — the README's rule of thumb (match `num_workers` when it is below 3, else set to 3) has no
  dedicated field under that exact name in the config catalog; the related switch that *is* present is
  [`AgentConfig.multi_seed_eval`](../catalog/ai_scientist/treesearch/utils/config.md#AgentConfig.multi_seed_eval).
  Treat `num_seeds` as a YAML-level knob and cross-check the parallel-agent concept page for how seeding
  feeds evaluation.
- The README explicitly notes
  [`AgentConfig.k_fold_validation`](../catalog/ai_scientist/treesearch/utils/config.md#AgentConfig.k_fold_validation),
  [`AgentConfig.expose_prediction`](../catalog/ai_scientist/treesearch/utils/config.md#AgentConfig.expose_prediction),
  and [`AgentConfig.data_preview`](../catalog/ai_scientist/treesearch/utils/config.md#AgentConfig.data_preview)
  are **not used in the current version** — they exist as fields but are inert.

**`search` block**
- `max_debug_depth` → [`SearchConfig.max_debug_depth`](../catalog/ai_scientist/treesearch/utils/config.md#SearchConfig.max_debug_depth)
  — how many times the agent will try to debug a failing node before abandoning that path.
- `debug_prob` → [`SearchConfig.debug_prob`](../catalog/ai_scientist/treesearch/utils/config.md#SearchConfig.debug_prob)
  — the probability of attempting to debug a failing node at all.
- `num_drafts` → [`SearchConfig.num_drafts`](../catalog/ai_scientist/treesearch/utils/config.md#SearchConfig.num_drafts)
  — the number of initial root nodes, i.e. how many independent trees are grown during Stage 1.

The runtime that consumes `num_workers`/`steps` is
[`ParallelAgent`](../catalog/ai_scientist/treesearch/parallel_agent.md#ParallelAgent): it reads its own
[`ParallelAgent.num_workers`](../catalog/ai_scientist/treesearch/parallel_agent.md#ParallelAgent.num_workers)
and drives each expansion through
[`ParallelAgent.step`](../catalog/ai_scientist/treesearch/parallel_agent.md#ParallelAgent.step); the
debug behavior gated by `max_debug_depth`/`debug_prob` surfaces in
[`MinimalAgent._debug`](../catalog/ai_scientist/treesearch/parallel_agent.md#MinimalAgent._debug), and the
`num_drafts` root nodes are seeded via
[`MinimalAgent._draft`](../catalog/ai_scientist/treesearch/parallel_agent.md#MinimalAgent._draft).

## Why it matters / when it applies
These knobs are the primary throughput/cost/thoroughness levers for an experiment run. `num_workers × step
budget` bounds the compute and dollar cost; `num_drafts` widens the initial search (more independent
attempts at the idea) at the cost of more roots to grow; `max_debug_depth` and `debug_prob` trade off
persistence on flaky nodes against wasting budget on dead ends. Because the defaults ship
`claude-3-5-sonnet` for experiments and a run costs ~$15–20, the README's guidance is to review this file
before launching rather than accept defaults blindly.

## Connections
- Code concepts:
  [ai_scientist-treesearch-utils-config](../concepts/ai_scientist-treesearch-utils-config.md) — the config
  dataclasses and loading; [ai_scientist-treesearch-parallel_agent](../concepts/ai_scientist-treesearch-parallel_agent.md)
  — the parallel search runtime that consumes these knobs.
- Module catalogs:
  [ai_scientist/treesearch/utils/config](../catalog/ai_scientist/treesearch/utils/config.md),
  [ai_scientist/treesearch/parallel_agent](../catalog/ai_scientist/treesearch/parallel_agent.md).
- Related doc-concepts: [two-stage-operator-workflow](two-stage-operator-workflow.md),
  [aide-lineage](aide-lineage.md).

## Source
Extracted from `README.md` (kept in place).
