---
title: 'Module: domains/article_opt/pipeline/impact_assessment.py'
type: catalog
provenance: extracted
module: domains/article_opt/pipeline/impact_assessment.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.pipeline.impact_assessment`/
symbols:
  ImpactAssessmentStage.run: ImpactAssessmentStage#run().
  ImpactAssessmentStage: ImpactAssessmentStage#
  SYSTEM: SYSTEM.
  RUBRIC_BRIEF: RUBRIC_BRIEF.
  ImpactAssessmentStage.name: ImpactAssessmentStage#name.
---
# Module: [`domains/article_opt/pipeline/impact_assessment.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/impact_assessment.py)

## Classes
### `ImpactAssessmentStage`  ·  implements/extends BaseStage
- def: [`domains/article_opt/pipeline/impact_assessment.py:27`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/impact_assessment.py#L27) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
- signature: `class ImpactAssessmentStage(BaseStage):`
- members:
  - `run(self, context: dict)` — [`L30`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/impact_assessment.py#L30) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
  - `name` — [`L28`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/impact_assessment.py#L28)
- uses (calls/refs, reference-scoped): [`parse_json_response`](../../../core/llm_client.md#parse_json_response), [`call_llm`](../../../core/llm_client.md#call_llm), [`BaseStage`](base.md#BaseStage), [`_save_artifact`](base.md#BaseStage._save_artifact), [`model`](base.md#BaseStage.model), [`RUBRIC_BRIEF`](impact_assessment.md#RUBRIC_BRIEF), [`SYSTEM`](impact_assessment.md#SYSTEM)
- used by: [`BaseStage`](base.md#BaseStage), [`stages`](../runner.md#InnerRunner.stages), [`run`](base.md#BaseStage.run)  (2 test-only)

## Module values
- `RUBRIC_BRIEF` — [`L19`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/impact_assessment.py#L19)
- `SYSTEM` — [`L12`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/impact_assessment.py#L12)

