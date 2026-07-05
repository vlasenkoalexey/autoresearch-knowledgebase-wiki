---
title: Level 1.5 — search-config adjustment (freeze/unfreeze)
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# Level 1.5 — search-config adjustment (freeze/unfreeze)

## Definition
Level 1.5 is the tactical half of the outer loop: it changes *runtime search parameters* — freeze/unfreeze which hyperparameters are searched, shift strategy, and supply guidance text — without writing any new code. It handles adjustments like "stop searching WEIGHT_DECAY, focus on LR," leaving strategic mechanism invention to Level 2. This layer is the outer loop's control surface over the inner search.

## In bilevel-autoresearch (grounded)
- The control surface is [`SearchConfig`](../catalog/domains/train_opt/config.md#SearchConfig) in `domains/train_opt/config.py`. It exposes [`active_params`](../catalog/domains/train_opt/config.md#SearchConfig.active_params) (parameters currently available for search), [`frozen_params`](../catalog/domains/train_opt/config.md#SearchConfig.frozen_params) (removed from the search), [`strategy`](../catalog/domains/train_opt/config.md#SearchConfig.strategy), and [`guidance`](../catalog/domains/train_opt/config.md#SearchConfig.guidance) text.
- In the training domain, [`TrainOuterLoop`](../catalog/domains/train_opt/outer.md#TrainOuterLoop) analyzes the inner trace (`_analyze`) and writes config updates through [`_apply_analysis`](../catalog/domains/train_opt/outer.md#TrainOuterLoop._apply_analysis), which applies the outer-loop analysis to the inner loop's `SearchConfig`.
- In the article domain, the analogous tactical adjustment is prompt overrides rather than frozen params: [`OuterAnalyzer`](../catalog/domains/article_opt/outer.md#OuterAnalyzer) produces config changes and [`OuterLoopController`](../catalog/domains/article_opt/outer.md#OuterLoopController) applies them (`_apply_config_changes`).

## Why it matters / when it applies
The ablation is blunt about this layer: Group B (Level 1 + 1.5) scored −0.006 ± 0.006 versus Group A's −0.009 (0.7×) — parameter-only outer-loop adjustment gave **no reliable gain** on its own. Its value is separation of concerns: pulling tactical parameter management out of Level 2 lets mechanism discovery stay clean. The near-identical Group D (Level 1 + 2, mechanisms without config adjustment) reached 3.8×, confirming Level 2 carries the improvement while 1.5 is a supporting, not driving, layer.

## Connections
- Code concepts: [domains-train_opt-config](../concepts/domains-train_opt-config.md), [domains-train_opt-outer](../concepts/domains-train_opt-outer.md), [domains-article_opt-outer](../concepts/domains-article_opt-outer.md), [core-state](../concepts/core-state.md).
- Module catalogs: [domains/train_opt/config.md](../catalog/domains/train_opt/config.md), [domains/train_opt/outer.md](../catalog/domains/train_opt/outer.md), [domains/article_opt/outer.md](../catalog/domains/article_opt/outer.md).
- Related doc-concepts: [bilevel-architecture](bilevel-architecture.md), [level-2-mechanism-generation](level-2-mechanism-generation.md).

## Source
Extracted from `README.md` (kept in place).
