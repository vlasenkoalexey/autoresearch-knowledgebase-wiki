---
title: AIDE lineage (tree-search provenance)
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# AIDE lineage (tree-search provenance)

## Definition
The README's Acknowledgement states that the tree-search component under the `ai_scientist` directory is
**built on top of the [AIDE](https://github.com/WecoAI/aideml) project**. AIDE (from WecoAI) is a
solution-space tree search over agent-generated code: it maintains a journal of nodes, drafts candidate
solutions, executes them, and improves or debugs from the best node so far. AI Scientist-v2 inherits that
core and extends it into a parallel, experiment-manager-guided search that generalizes across ML domains.

## In ai-scientist-v2 (grounded)
The AIDE heritage is visible in the shape of the treesearch subsystem's core abstractions rather than in
any single symbol the README names — this is a provenance note, so the grounding is structural:
- The **journal / node** model AIDE popularized is carried by
  [`Journal`](../catalog/ai_scientist/treesearch/journal.md#Journal) and
  [`Node`](../catalog/ai_scientist/treesearch/journal.md#Node), with the classic AIDE distinction between
  draft roots ([`Journal.draft_nodes`](../catalog/ai_scientist/treesearch/journal.md#Journal.draft_nodes))
  and best-so-far selection
  ([`Journal.get_best_node`](../catalog/ai_scientist/treesearch/journal.md#Journal.get_best_node)) (owning
  module: [`ai_scientist/treesearch/journal.py`](../catalog/ai_scientist/treesearch/journal.md)).
- AIDE's draft → improve → debug operators map onto
  [`MinimalAgent._draft`](../catalog/ai_scientist/treesearch/parallel_agent.md#MinimalAgent._draft),
  [`MinimalAgent._improve`](../catalog/ai_scientist/treesearch/parallel_agent.md#MinimalAgent._improve),
  and [`MinimalAgent._debug`](../catalog/ai_scientist/treesearch/parallel_agent.md#MinimalAgent._debug).
- The v2 extension beyond stock AIDE is the *parallelization*:
  [`ParallelAgent`](../catalog/ai_scientist/treesearch/parallel_agent.md#ParallelAgent) expands multiple
  nodes concurrently per
  [`ParallelAgent.step`](../catalog/ai_scientist/treesearch/parallel_agent.md#ParallelAgent.step) (owning
  module: [`ai_scientist/treesearch/parallel_agent.py`](../catalog/ai_scientist/treesearch/parallel_agent.md)) —
  the `num_workers` concurrency the README documents. AI Scientist-v2's own contribution on top is the
  experiment-manager guidance and the multi-stage discovery-to-manuscript pipeline that AIDE alone does not
  provide.

## Why it matters / when it applies
The lineage explains *why* the code is organized the way it is: readers familiar with AIDE will recognize
the journal/node/draft-improve-debug vocabulary immediately, and the acknowledgement is also a licensing
and credit obligation. It matters when reasoning about which behaviors are inherited (the search core) versus
v2-specific (parallel workers, the experiment manager agent, the full paper-generation pipeline).

## Connections
- Code concepts:
  [ai_scientist-treesearch-parallel_agent](../concepts/ai_scientist-treesearch-parallel_agent.md) — the
  parallel search runtime;
  [ai_scientist-treesearch-journal](../concepts/ai_scientist-treesearch-journal.md) — the journal/node
  bookkeeping AIDE contributes.
- Module catalogs:
  [ai_scientist/treesearch/parallel_agent](../catalog/ai_scientist/treesearch/parallel_agent.md),
  [ai_scientist/treesearch/journal](../catalog/ai_scientist/treesearch/journal.md).
- Related doc-concepts: [bfts-tree-search-configuration](bfts-tree-search-configuration.md),
  [executing-llm-written-code](executing-llm-written-code.md).

## Source
Extracted from `README.md` (kept in place).
