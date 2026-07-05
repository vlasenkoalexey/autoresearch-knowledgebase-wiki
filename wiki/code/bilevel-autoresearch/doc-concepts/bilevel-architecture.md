---
title: Bilevel architecture and the three-layer split
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# Bilevel architecture and the three-layer split

## Definition
"Autoresearch that researches itself." An **inner loop** optimizes the task output (propose → execute → evaluate → keep/discard), and an **outer loop** optimizes *how the inner loop works* (analyze trace → modify mechanisms → re-run). Both levels use the same pattern — propose × evaluate × iterate — but the outer loop improves the inner loop not by tuning prompts but by structurally changing how it searches. In the experiment the outer loop is split into two responsibilities for cleaner separation of concerns, yielding three layers.

## In bilevel-autoresearch (grounded)
- **Level 1 — inner loop.** One task cycle is driven by [`InnerLoopController.run_cycle`](../catalog/core/inner_loop.md#InnerLoopController.run_cycle) in module `core/inner_loop.py`; per-cycle process signals accumulate in [`InnerLoopState`](../catalog/core/state.md#InnerLoopState).
- **Level 1.5 — outer loop, config.** Adjusts runtime search *parameters* (freeze/unfreeze, strategy shift) via [`SearchConfig`](../catalog/domains/train_opt/config.md#SearchConfig) in `domains/train_opt/config.py`. See sibling [level-1.5-config-adjustment](level-1.5-config-adjustment.md).
- **Level 2 — outer loop, mechanism.** Generates new Python mechanism code and injects it, through [`BaseMechanismResearcher`](../catalog/core/base_mechanism_research.md#BaseMechanismResearcher) and its domain subclasses. See sibling [level-2-mechanism-generation](level-2-mechanism-generation.md).
- The outer loop reads the inner trace into [`OuterLoopState`](../catalog/core/state.md#OuterLoopState) via [`OuterLoopState.extract_from_inner`](../catalog/core/state.md#OuterLoopState.extract_from_inner), then drives re-runs — in train_opt via [`TrainOuterLoop.run`](../catalog/domains/train_opt/outer.md#TrainOuterLoop.run), in article_opt via [`OuterLoopController.run`](../catalog/domains/article_opt/outer.md#OuterLoopController.run).

## Why it matters / when it applies
Separating tactical parameter tuning (Level 1.5, "stop searching WEIGHT_DECAY, focus on LR") from strategic innovation (Level 2, "invent a Tabu Search mechanism") lets Level 2 focus purely on mechanism discovery without being distracted by parameter tuning. The controlled ablation (4 groups × 3 repeats × 30 iterations) found Level 2 is the load-bearing layer — Group C (1 + 1.5 + 2) reached ~5× the baseline gain, while parameter-only Level 1.5 (Group B) gave no reliable gain. Applies to anything with a measurable objective: project management, multi-agent coordination, experiment scheduling, the research process itself.

## Connections
- Code concepts: [core-inner_loop](../concepts/core-inner_loop.md), [core-state](../concepts/core-state.md), [core-base_mechanism_research](../concepts/core-base_mechanism_research.md), [domains-train_opt-outer](../concepts/domains-train_opt-outer.md), [domains-article_opt-outer](../concepts/domains-article_opt-outer.md).
- Module catalogs: [core/inner_loop.md](../catalog/core/inner_loop.md), [core/state.md](../catalog/core/state.md).
- Related doc-concepts: [level-1.5-config-adjustment](level-1.5-config-adjustment.md), [level-2-mechanism-generation](level-2-mechanism-generation.md), [recursive-bootstrapping](recursive-bootstrapping.md), [evaluator-isolation](evaluator-isolation.md).

## Source
Extracted from `README.md` (kept in place).
