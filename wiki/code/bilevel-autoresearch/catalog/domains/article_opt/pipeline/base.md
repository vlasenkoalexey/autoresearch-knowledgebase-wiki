---
title: 'Module: domains/article_opt/pipeline/base.py'
type: catalog
provenance: extracted
module: domains/article_opt/pipeline/base.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.pipeline.base`/BaseStage#
symbols:
  BaseStage: ''
  BaseStage.run: run().
  BaseStage._save_artifact: _save_artifact().
  BaseStage.model: model.
  BaseStage.name: name.
  BaseStage._outer_guidance: _outer_guidance().
  BaseStage.max_retries: max_retries.
  BaseStage.__init__: __init__().
---
# Module: [`domains/article_opt/pipeline/base.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py)

## Classes
### `BaseStage`  ·  implements/extends ABC
- def: [`domains/article_opt/pipeline/base.py:6`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py#L6) — documented in [domains-article_opt-mechanism_research](../../../../concepts/domains-article_opt-mechanism_research.md)
- doc: Base class for all article optimizer stages.
- signature: `class BaseStage(ABC):`
- members:
  - `_outer_guidance(self, context: dict)` — [`L33`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py#L33) — Return outer loop guidance for this stage, or empty string. — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
  - `run(self, context: dict)` — [`L31`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py#L31) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
  - `max_retries` — [`L25`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py#L25)
  - `model` — [`L28`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py#L28) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
  - `name` — [`L24`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py#L24) — documented in [domains-article_opt-pipeline-base](../../../../concepts/domains-article_opt-pipeline-base.md)
- protocol/private: `__init__`[`L27`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py#L27), `_save_artifact`[`L41`](../../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/pipeline/base.py#L41)
- uses (calls/refs, reference-scoped): [`run`](article_analysis.md#ArticleAnalysisStage.run), [`run`](edit_planning.md#EditPlanningStage.run), [`run`](impact_assessment.md#ImpactAssessmentStage.run), [`run`](improvement_hypotheses.md#ImprovementHypothesesStage.run), [`ArticleAnalysisStage`](article_analysis.md#ArticleAnalysisStage), [`RevisedOutputStage`](revised_output.md#RevisedOutputStage), [`EditPlanningStage`](edit_planning.md#EditPlanningStage), [`ImpactAssessmentStage`](impact_assessment.md#ImpactAssessmentStage), [`ImprovementHypothesesStage`](improvement_hypotheses.md#ImprovementHypothesesStage), [`run`](revised_output.md#RevisedOutputStage.run)  (2 test-only)
- used by: [`inject_stage`](../runner.md#InnerRunner.inject_stage), [`run`](article_analysis.md#ArticleAnalysisStage.run), [`run`](edit_planning.md#EditPlanningStage.run), [`run`](impact_assessment.md#ImpactAssessmentStage.run), [`run`](improvement_hypotheses.md#ImprovementHypothesesStage.run), [`_revise_by_section`](revised_output.md#RevisedOutputStage._revise_by_section), [`ArticleAnalysisStage`](article_analysis.md#ArticleAnalysisStage), [`RevisedOutputStage`](revised_output.md#RevisedOutputStage), [`_revise_whole`](revised_output.md#RevisedOutputStage._revise_whole), [`EditPlanningStage`](edit_planning.md#EditPlanningStage), [`ImpactAssessmentStage`](impact_assessment.md#ImpactAssessmentStage), [`ImprovementHypothesesStage`](improvement_hypotheses.md#ImprovementHypothesesStage), [`run`](revised_output.md#RevisedOutputStage.run), [`_load_stage`](../mechanism_research.md#MechanismResearcher._load_stage)  (7 test-only)

