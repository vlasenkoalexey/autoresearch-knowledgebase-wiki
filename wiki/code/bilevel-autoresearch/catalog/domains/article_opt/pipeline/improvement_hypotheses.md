---
title: 'Module: domains/article_opt/pipeline/improvement_hypotheses.py'
type: catalog
provenance: extracted
module: domains/article_opt/pipeline/improvement_hypotheses.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.pipeline.improvement_hypotheses`/
symbols:
  ImprovementHypothesesStage.run: ImprovementHypothesesStage#run().
  ImprovementHypothesesStage: ImprovementHypothesesStage#
  SYSTEM: SYSTEM.
  ImprovementHypothesesStage.name: ImprovementHypothesesStage#name.
---
# Module: [`domains/article_opt/pipeline/improvement_hypotheses.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/improvement_hypotheses.py)

## Classes
### `ImprovementHypothesesStage`  ·  implements/extends BaseStage
- def: [`domains/article_opt/pipeline/improvement_hypotheses.py:24`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/improvement_hypotheses.py#L24) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
- signature: `class ImprovementHypothesesStage(BaseStage):`
- members:
  - `run(self, context: dict)` — [`L27`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/improvement_hypotheses.py#L27) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
  - `name` — [`L25`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/improvement_hypotheses.py#L25)
- uses (calls/refs, reference-scoped): [`parse_json_response`](../../../core/llm_client.md#parse_json_response), [`call_llm`](../../../core/llm_client.md#call_llm), [`BaseStage`](base.md#BaseStage), [`_save_artifact`](base.md#BaseStage._save_artifact), [`model`](base.md#BaseStage.model), [`_outer_guidance`](base.md#BaseStage._outer_guidance), [`SYSTEM`](improvement_hypotheses.md#SYSTEM)
- used by: [`BaseStage`](base.md#BaseStage), [`stages`](../runner.md#InnerRunner.stages), [`run`](base.md#BaseStage.run)  (2 test-only)

## Module values
- `SYSTEM` — [`L12`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/improvement_hypotheses.py#L12)

