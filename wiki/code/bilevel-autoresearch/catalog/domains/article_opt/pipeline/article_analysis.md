---
title: 'Module: domains/article_opt/pipeline/article_analysis.py'
type: catalog
provenance: extracted
module: domains/article_opt/pipeline/article_analysis.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.pipeline.article_analysis`/
symbols:
  ArticleAnalysisStage.run: ArticleAnalysisStage#run().
  ArticleAnalysisStage: ArticleAnalysisStage#
  SYSTEM: SYSTEM.
  RUBRIC: RUBRIC.
  ArticleAnalysisStage.name: ArticleAnalysisStage#name.
---
# Module: [`domains/article_opt/pipeline/article_analysis.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/article_analysis.py)

## Classes
### `ArticleAnalysisStage`  ·  implements/extends BaseStage
- def: [`domains/article_opt/pipeline/article_analysis.py:53`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/article_analysis.py#L53) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
- signature: `class ArticleAnalysisStage(BaseStage):`
- members:
  - `run(self, context: dict)` — [`L56`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/article_analysis.py#L56) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
  - `name` — [`L54`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/article_analysis.py#L54)
- uses (calls/refs, reference-scoped): [`parse_json_response`](../../../core/llm_client.md#parse_json_response), [`call_llm`](../../../core/llm_client.md#call_llm), [`BaseStage`](base.md#BaseStage), [`_save_artifact`](base.md#BaseStage._save_artifact), [`model`](base.md#BaseStage.model), [`RUBRIC`](article_analysis.md#RUBRIC), [`SYSTEM`](article_analysis.md#SYSTEM)
- used by: [`BaseStage`](base.md#BaseStage), [`stages`](../runner.md#InnerRunner.stages), [`run`](base.md#BaseStage.run)  (5 test-only)

## Module values
- `RUBRIC` — [`L23`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/article_analysis.py#L23)
- `SYSTEM` — [`L13`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/article_analysis.py#L13)

