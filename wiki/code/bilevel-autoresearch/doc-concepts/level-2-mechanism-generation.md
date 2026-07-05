---
title: Level 2 — mechanism generation via importlib
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# Level 2 — mechanism generation via importlib

## Definition
Level 2 is the strategic layer of the outer loop: an autonomous agent reads the inner loop's code, identifies bottlenecks, and *writes new Python code* to fix them — inventing structural changes to the search process rather than tuning prompts or parameters. The outer loop generates Python for new search mechanisms, dynamically loads them via `importlib`, and injects them into the running inner loop. This is the load-bearing layer of the architecture (Group C reached ~5× the baseline in the ablation).

## In bilevel-autoresearch (grounded)
- The shared protocol is [`BaseMechanismResearcher`](../catalog/core/base_mechanism_research.md#BaseMechanismResearcher) in `core/base_mechanism_research.py`, whose [`_run_session`](../catalog/core/base_mechanism_research.md#BaseMechanismResearcher._run_session) executes a fixed 4-round research session (Explore → Critique → Specify → Generate).
- **Training domain:** [`TrainMechanismResearcher`](../catalog/domains/train_opt/mechanism_research.md#TrainMechanismResearcher) — [`research`](../catalog/domains/train_opt/mechanism_research.md#TrainMechanismResearcher.research) runs a session and rewrites `runner.py`; [`validate`](../catalog/domains/train_opt/mechanism_research.md#TrainMechanismResearcher.validate) verifies the modified runner can be imported without errors (the activate-or-revert gate). Generated mechanisms (Tabu Search, Multi-Scale Bandit, Orthogonal Exploration) are injected into [`TrainRunner`](../catalog/domains/train_opt/runner.md#TrainRunner).
- **Article domain:** [`MechanismResearcher`](../catalog/domains/article_opt/mechanism_research.md#MechanismResearcher) generates a new pipeline stage; [`_load_stage`](../catalog/domains/article_opt/mechanism_research.md#MechanismResearcher._load_stage) dynamically imports the generated file and returns the class, [`validate`](../catalog/domains/article_opt/mechanism_research.md#MechanismResearcher.validate) checks it, and [`InnerRunner.inject_stage`](../catalog/domains/article_opt/runner.md#InnerRunner.inject_stage) inserts the new [`BaseStage`](../catalog/domains/article_opt/pipeline/base.md#BaseStage) subclass into the pipeline.
- All rounds call the LLM through [`call_llm`](../catalog/core/llm_client.md#call_llm) / [`LLMClient`](../catalog/core/llm_client.md#LLMClient).

## Why it matters / when it applies
Baseline autoresearch (Group A) follows a deterministic search path — it tries a few params then gets stuck repeating the same proposals for 20+ iterations. Level 2's generated mechanisms (Tabu Search, Orthogonal Exploration) break that loop and steer the LLM toward directions it never explored (e.g. reducing TOTAL_BATCH_SIZE). Each repeat independently discovered mechanisms from different domains — combinatorial optimization, online learning/MAB, design of experiments — with no human specifying which to explore. A GP Regressor mechanism was auto-generated but reverted when `sklearn` was not installed, demonstrating the validate-or-revert safety gate.

## Connections
- Code concepts: [core-base_mechanism_research](../concepts/core-base_mechanism_research.md), [domains-train_opt-mechanism_research](../concepts/domains-train_opt-mechanism_research.md), [domains-article_opt-mechanism_research](../concepts/domains-article_opt-mechanism_research.md), [domains-train_opt-runner](../concepts/domains-train_opt-runner.md), [domains-article_opt-runner](../concepts/domains-article_opt-runner.md), [domains-article_opt-pipeline-base](../concepts/domains-article_opt-pipeline-base.md), [core-llm_client](../concepts/core-llm_client.md).
- Module catalogs: [core/base_mechanism_research.md](../catalog/core/base_mechanism_research.md), [domains/train_opt/mechanism_research.md](../catalog/domains/train_opt/mechanism_research.md), [domains/article_opt/mechanism_research.md](../catalog/domains/article_opt/mechanism_research.md).
- Related doc-concepts: [bilevel-architecture](bilevel-architecture.md), [level-1.5-config-adjustment](level-1.5-config-adjustment.md), [two-demo-domains](two-demo-domains.md), [recursive-bootstrapping](recursive-bootstrapping.md).

## Source
Extracted from `README.md` (kept in place).
