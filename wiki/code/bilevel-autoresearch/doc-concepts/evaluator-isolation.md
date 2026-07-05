---
title: Evaluator isolation — lessons never reach judgments
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-05
status: fresh
---
# Evaluator isolation — lessons never reach judgments

## Definition
The framework's key invariant: **the evaluator must NEVER receive lesson memory. Lessons influence proposals, never judgments.** Accumulated lessons steer what the system tries next, but the module that scores an attempt must stay blind to that memory so the objective signal is not contaminated by what the system "expects" or "hopes" to see.

## In bilevel-autoresearch (grounded)
- Lessons are the memory types in `core/state.py`: [`InnerLesson`](../catalog/core/state.md#InnerLesson) and [`OuterLesson`](../catalog/core/state.md#OuterLesson), carried on [`InnerLoopState`](../catalog/core/state.md#InnerLoopState) / [`OuterLoopState`](../catalog/core/state.md#OuterLoopState).
- In article_opt these lessons feed *proposal-side* code: [`InnerRunner`](../catalog/domains/article_opt/runner.md#InnerRunner) formats them via `_build_lessons_text` and injects them into the generative stages, while scoring is done separately by [`ArticleEvaluator.evaluate`](../catalog/domains/article_opt/evaluator/article_evaluator.md#ArticleEvaluator.evaluate), which receives only the article and its id — not the lesson memory. The evaluator and the proposer are distinct modules precisely so the boundary can be enforced.
- The isolation boundary is a first-class concern of the state layer (`core/state.py` is described in the architecture as "state management with isolation boundaries"), and [`OuterLoopState.extract_from_inner`](../catalog/core/state.md#OuterLoopState.extract_from_inner) pulls process-level signals up to the outer loop without routing lesson text into the scoring path.

## Why it matters / when it applies
If lessons leaked into the evaluator, the system could learn to *report* success rather than *achieve* it — the measured objective (`val_bpb`, the article rubric) would drift from ground truth and the whole bilevel gain would be an artifact. Keeping judgment blind to memory is what lets the outer loop trust the inner loop's trace when deciding whether to freeze a param or activate a generated mechanism. The constraint applies to every domain and is called out in the README as a hard rule for anyone adding a new domain or provider.

## Connections
- Code concepts: [core-state](../concepts/core-state.md), [domains-article_opt-runner](../concepts/domains-article_opt-runner.md), [core-inner_loop](../concepts/core-inner_loop.md).
- Module catalogs: [core/state.md](../catalog/core/state.md), [domains/article_opt/evaluator/article_evaluator.md](../catalog/domains/article_opt/evaluator/article_evaluator.md).
- Related doc-concepts: [bilevel-architecture](bilevel-architecture.md), [two-demo-domains](two-demo-domains.md).

## Source
Extracted from `README.md` (kept in place).
