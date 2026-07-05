---
title: 'Module: domains/article_opt/evaluator/article_evaluator.py'
type: catalog
provenance: extracted
module: domains/article_opt/evaluator/article_evaluator.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.evaluator.article_evaluator`/
symbols:
  ArticleEvaluator.evaluate: ArticleEvaluator#evaluate().
  ArticleEvaluator: ArticleEvaluator#
  EVALUATOR_SYSTEM: EVALUATOR_SYSTEM.
  RUBRIC: RUBRIC.
  ArticleEvaluator.model: ArticleEvaluator#model.
  ArticleEvaluator._fallback: ArticleEvaluator#_fallback().
  ArticleEvaluator.__init__: ArticleEvaluator#__init__().
---
# Module: [`domains/article_opt/evaluator/article_evaluator.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/evaluator/article_evaluator.py)

## Classes
### `ArticleEvaluator`
- def: [`domains/article_opt/evaluator/article_evaluator.py:53`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/evaluator/article_evaluator.py#L53)
- doc: Evaluates a complete revised article against the 5-dimension rubric.
- signature: `class ArticleEvaluator:`
- members:
  - `evaluate(self, article: str, article_id: str)` — [`L62`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/evaluator/article_evaluator.py#L62) — Score the article on dimensions A–E. — documented in [domains-article_opt-runner](../../../../concepts/domains-article_opt-runner.md)
  - `model` — [`L60`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/evaluator/article_evaluator.py#L60)
- protocol/private: `__init__`[`L59`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/evaluator/article_evaluator.py#L59), `_fallback`[`L121`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/evaluator/article_evaluator.py#L121)
- uses (calls/refs, reference-scoped): [`parse_json_response`](../../../core/llm_client.md#parse_json_response), [`call_llm`](../../../core/llm_client.md#call_llm), [`EVALUATOR_SYSTEM`](article_evaluator.md#EVALUATOR_SYSTEM), [`RUBRIC`](article_evaluator.md#RUBRIC)
- used by: [`run_once`](../runner.md#InnerRunner.run_once), [`evaluator`](../runner.md#InnerRunner.evaluator)

## Module values
- `EVALUATOR_SYSTEM` — [`L10`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/evaluator/article_evaluator.py#L10)
- `RUBRIC` — [`L14`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/evaluator/article_evaluator.py#L14)

