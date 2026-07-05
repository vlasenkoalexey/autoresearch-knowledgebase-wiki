---
title: 'Module: domains/article_opt/pipeline/edit_planning.py'
type: catalog
provenance: extracted
module: domains/article_opt/pipeline/edit_planning.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.pipeline.edit_planning`/
symbols:
  EditPlanningStage.run: EditPlanningStage#run().
  EditPlanningStage: EditPlanningStage#
  TRIAGE_SYSTEM: TRIAGE_SYSTEM.
  PLAN_SYSTEM: PLAN_SYSTEM.
  EditPlanningStage.name: EditPlanningStage#name.
  EditPlanningStage.max_retries: EditPlanningStage#max_retries.
---
# Module: [`domains/article_opt/pipeline/edit_planning.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/edit_planning.py)

## Classes
### `EditPlanningStage`  ·  implements/extends BaseStage
- def: [`domains/article_opt/pipeline/edit_planning.py:30`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/edit_planning.py#L30) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
- signature: `class EditPlanningStage(BaseStage):`
- members:
  - `run(self, context: dict)` — [`L34`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/edit_planning.py#L34) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
  - `max_retries` — [`L32`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/edit_planning.py#L32)
  - `name` — [`L31`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/edit_planning.py#L31)
- uses (calls/refs, reference-scoped): [`call_llm`](../../../core/llm_client.md#call_llm), [`BaseStage`](base.md#BaseStage), [`_save_artifact`](base.md#BaseStage._save_artifact), [`model`](base.md#BaseStage.model), [`_outer_guidance`](base.md#BaseStage._outer_guidance), [`PLAN_SYSTEM`](edit_planning.md#PLAN_SYSTEM), [`TRIAGE_SYSTEM`](edit_planning.md#TRIAGE_SYSTEM)
- used by: [`BaseStage`](base.md#BaseStage), [`stages`](../runner.md#InnerRunner.stages), [`run`](base.md#BaseStage.run)  (2 test-only)

## Module values
- `PLAN_SYSTEM` — [`L19`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/edit_planning.py#L19)
- `TRIAGE_SYSTEM` — [`L14`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/edit_planning.py#L14)

