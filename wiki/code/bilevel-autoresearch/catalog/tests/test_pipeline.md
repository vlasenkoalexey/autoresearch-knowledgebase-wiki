---
title: 'Module: tests/test_pipeline.py'
type: catalog
provenance: extracted
module: tests/test_pipeline.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `tests.test_pipeline`/Test
symbols:
  TestStageNames.test_expected_names: StageNames#test_expected_names().
  TestStageNames.test_all_stage_names_unique: StageNames#test_all_stage_names_unique().
  TestBaseStage.test_max_retries_default_none: BaseStage#test_max_retries_default_none().
  TestBaseStage.test_model_default_empty: BaseStage#test_model_default_empty().
  TestBaseStage.test_model_can_be_set: BaseStage#test_model_can_be_set().
  TestSaveArtifact.test_save_artifact_creates_file: SaveArtifact#test_save_artifact_creates_file().
  TestSaveArtifact.test_save_artifact_creates_parent_dirs: SaveArtifact#test_save_artifact_creates_parent_dirs().
  TestBaseStage: BaseStage#
  TestStageNames: StageNames#
  TestSaveArtifact: SaveArtifact#
---
# Module: [`tests/test_pipeline.py`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py)

## Classes
### `TestBaseStage`
- def: [`tests/test_pipeline.py:12`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L12)
- signature: `class TestBaseStage:`
- members:
  - `test_max_retries_default_none(self)` — [`L13`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L13)
  - `test_model_can_be_set(self)` — [`L20`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L20)
  - `test_model_default_empty(self)` — [`L16`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L16)
- uses (calls/refs, reference-scoped): [`BaseStage`](../domains/article_opt/pipeline/base.md#BaseStage), [`model`](../domains/article_opt/pipeline/base.md#BaseStage.model), [`ArticleAnalysisStage`](../domains/article_opt/pipeline/article_analysis.md#ArticleAnalysisStage), [`max_retries`](../domains/article_opt/pipeline/base.md#BaseStage.max_retries)

### `TestSaveArtifact`
- def: [`tests/test_pipeline.py:45`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L45)
- signature: `class TestSaveArtifact:`
- members:
  - `test_save_artifact_creates_file(self, tmp_path)` — [`L46`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L46)
  - `test_save_artifact_creates_parent_dirs(self, tmp_path)` — [`L53`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L53)
- uses (calls/refs, reference-scoped): [`_save_artifact`](../domains/article_opt/pipeline/base.md#BaseStage._save_artifact), [`ArticleAnalysisStage`](../domains/article_opt/pipeline/article_analysis.md#ArticleAnalysisStage), [`RevisedOutputStage`](../domains/article_opt/pipeline/revised_output.md#RevisedOutputStage)

### `TestStageNames`
- def: [`tests/test_pipeline.py:25`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L25)
- signature: `class TestStageNames:`
- members:
  - `test_all_stage_names_unique(self)` — [`L26`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L26)
  - `test_expected_names(self)` — [`L37`](../../../../../raw/code/bilevel-autoresearch/tests/test_pipeline.py#L37)
- uses (calls/refs, reference-scoped): [`ArticleAnalysisStage`](../domains/article_opt/pipeline/article_analysis.md#ArticleAnalysisStage), [`RevisedOutputStage`](../domains/article_opt/pipeline/revised_output.md#RevisedOutputStage), [`name`](../domains/article_opt/pipeline/base.md#BaseStage.name), [`EditPlanningStage`](../domains/article_opt/pipeline/edit_planning.md#EditPlanningStage), [`ImpactAssessmentStage`](../domains/article_opt/pipeline/impact_assessment.md#ImpactAssessmentStage), [`ImprovementHypothesesStage`](../domains/article_opt/pipeline/improvement_hypotheses.md#ImprovementHypothesesStage)

