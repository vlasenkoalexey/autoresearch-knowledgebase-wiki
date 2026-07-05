---
title: Two demo domains — train_opt vs article_opt
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# Two demo domains — train_opt vs article_opt

## Definition
The bilevel principle is domain-agnostic, so the repo ships two self-contained instantiations under `domains/`. **Training optimization** (`train_opt`) is the headline experiment: the LLM proposes hyperparameter changes to Karpathy's `train.py`, trains for ~5 minutes, and measures `val_bpb` — it needs a GPU and a cloned `karpathy/autoresearch`. **Article optimization** (`article_opt`) is a lightweight no-GPU demo: a 5-stage article-revision pipeline scored against a rubric. Domains share `core/` but implement their own runner, outer loop, and mechanism research.

## In bilevel-autoresearch (grounded)
- **train_opt** — inner search runs in [`TrainRunner`](../catalog/domains/train_opt/runner.md#TrainRunner), the outer loop is [`TrainOuterLoop`](../catalog/domains/train_opt/outer.md#TrainOuterLoop) (freezes ineffective params, shifts strategy via [`SearchConfig`](../catalog/domains/train_opt/config.md#SearchConfig)), and Level 2 is [`TrainMechanismResearcher`](../catalog/domains/train_opt/mechanism_research.md#TrainMechanismResearcher) (generates Tabu Search / Multi-Scale Bandit / Orthogonal Exploration and injects them via `importlib`). Validated with the 3×3 ablation on RTX 5090 — 5× over baseline.
- **article_opt** — 5-stage pipeline (Analysis → Hypotheses → Planning → Assessment → Revision), each stage a [`BaseStage`](../catalog/domains/article_opt/pipeline/base.md#BaseStage) subclass, driven by [`InnerRunner`](../catalog/domains/article_opt/runner.md#InnerRunner) and scored by [`ArticleEvaluator.evaluate`](../catalog/domains/article_opt/evaluator/article_evaluator.md#ArticleEvaluator.evaluate) against a rubric. The outer loop [`OuterLoopController`](../catalog/domains/article_opt/outer.md#OuterLoopController) injects prompt overrides; Level 2 [`MechanismResearcher`](../catalog/domains/article_opt/mechanism_research.md#MechanismResearcher) generates new pipeline stages and inserts them with [`InnerRunner.inject_stage`](../catalog/domains/article_opt/runner.md#InnerRunner.inject_stage).
- Both call the shared multi-provider [`LLMClient`](../catalog/core/llm_client.md#LLMClient) and share the state types [`InnerLoopState`](../catalog/core/state.md#InnerLoopState) / [`OuterLoopState`](../catalog/core/state.md#OuterLoopState).

## Why it matters / when it applies
Two domains with different objectives (a continuous training metric vs a discrete rubric) and different Level-2 targets (rewrite the runner vs inject a pipeline stage) demonstrate the architecture is not bolted to one task. article_opt exists so the full bilevel flow (including Level 2 code generation) can be run offline without a GPU — the README uses it for the smoke test — while train_opt reproduces the paper's headline 5× result. Adding a domain means creating `runner.py`, `outer.py`, `config.py`, `cli.py`; only `core.llm_client` is imported from shared code.

## Connections
- Code concepts: [domains-train_opt-runner](../concepts/domains-train_opt-runner.md), [domains-train_opt-outer](../concepts/domains-train_opt-outer.md), [domains-train_opt-config](../concepts/domains-train_opt-config.md), [domains-train_opt-mechanism_research](../concepts/domains-train_opt-mechanism_research.md), [domains-article_opt-runner](../concepts/domains-article_opt-runner.md), [domains-article_opt-outer](../concepts/domains-article_opt-outer.md), [domains-article_opt-mechanism_research](../concepts/domains-article_opt-mechanism_research.md), [domains-article_opt-pipeline-base](../concepts/domains-article_opt-pipeline-base.md), [domains-article_opt-cli](../concepts/domains-article_opt-cli.md), [core-llm_client](../concepts/core-llm_client.md).
- Module catalogs: [domains/train_opt/runner.md](../catalog/domains/train_opt/runner.md), [domains/article_opt/runner.md](../catalog/domains/article_opt/runner.md), [domains/article_opt/evaluator/article_evaluator.md](../catalog/domains/article_opt/evaluator/article_evaluator.md).
- Related doc-concepts: [bilevel-architecture](bilevel-architecture.md), [level-2-mechanism-generation](level-2-mechanism-generation.md), [evaluator-isolation](evaluator-isolation.md).

## Source
Extracted from `README.md` (kept in place).
