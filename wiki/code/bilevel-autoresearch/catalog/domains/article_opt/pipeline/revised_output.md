---
title: 'Module: domains/article_opt/pipeline/revised_output.py'
type: catalog
provenance: extracted
module: domains/article_opt/pipeline/revised_output.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.pipeline.revised_output`/
symbols:
  RevisedOutputStage._revise_by_section: RevisedOutputStage#_revise_by_section().
  RevisedOutputStage: RevisedOutputStage#
  RevisedOutputStage._revise_whole: RevisedOutputStage#_revise_whole().
  RevisedOutputStage.run: RevisedOutputStage#run().
  SYSTEM: SYSTEM.
  SECTION_SYSTEM: SECTION_SYSTEM.
  _extract_sections: _extract_sections().
  RevisedOutputStage.name: RevisedOutputStage#name.
---
# Module: [`domains/article_opt/pipeline/revised_output.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py)

## Classes
### `RevisedOutputStage`  ·  implements/extends BaseStage
- def: [`domains/article_opt/pipeline/revised_output.py:56`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py#L56) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
- signature: `class RevisedOutputStage(BaseStage):`
- members:
  - `run(self, context: dict)` — [`L59`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py#L59) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
  - `name` — [`L57`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py#L57)
- protocol/private: `_revise_by_section`[`L97`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py#L97), `_revise_whole`[`L79`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py#L79)
- uses (calls/refs, reference-scoped): [`call_llm`](../../../core/llm_client.md#call_llm), [`BaseStage`](base.md#BaseStage), [`_save_artifact`](base.md#BaseStage._save_artifact), [`model`](base.md#BaseStage.model), [`SECTION_SYSTEM`](revised_output.md#SECTION_SYSTEM), [`SYSTEM`](revised_output.md#SYSTEM), [`_extract_sections`](revised_output.md#_extract_sections)
- used by: [`BaseStage`](base.md#BaseStage), [`stages`](../runner.md#InnerRunner.stages), [`run`](base.md#BaseStage.run)  (3 test-only)

## Functions
- `_extract_sections(article: str)` — [`L31`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py#L31) — Split article into (header, body) pairs. Returns [(header, body), ...]. — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)

## Module values
- `SECTION_SYSTEM` — [`L25`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py#L25)
- `SYSTEM` — [`L15`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/revised_output.py#L15)

