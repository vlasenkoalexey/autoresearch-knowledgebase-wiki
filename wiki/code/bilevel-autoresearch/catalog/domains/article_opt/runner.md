---
title: 'Module: domains/article_opt/runner.py'
type: catalog
provenance: extracted
module: domains/article_opt/runner.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.article_opt.runner`/
symbols:
  InnerRunner.run_once: InnerRunner#run_once().
  InnerRunner._extract_lessons: InnerRunner#_extract_lessons().
  InnerRunner.stages: InnerRunner#stages.
  InnerRunner._build_lessons_text: InnerRunner#_build_lessons_text().
  InnerRunner.inject_stage: InnerRunner#inject_stage().
  InnerRunner: InnerRunner#
  logger: logger.
  InnerRunner._run_stage_with_gate: InnerRunner#_run_stage_with_gate().
  InnerRunner.outer_cycle: InnerRunner#outer_cycle.
  InnerRunner.evaluator: InnerRunner#evaluator.
  InnerRunner.model: InnerRunner#model.
  InnerRunner.artifacts_base: InnerRunner#artifacts_base.
  InnerRunner.prompt_overrides: InnerRunner#prompt_overrides.
  LESSON_SYSTEM: LESSON_SYSTEM.
  InnerRunner.max_retries: InnerRunner#max_retries.
  InnerRunner.__init__: InnerRunner#__init__().
  InnerRunner.eval_model: InnerRunner#eval_model.
  InnerRunner.min_score: InnerRunner#min_score.
---
# Module: [`domains/article_opt/runner.py`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py)

## Classes
### `InnerRunner`
- def: [`domains/article_opt/runner.py:33`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L33) — documented in [domains-article_opt-cli](../../../concepts/domains-article_opt-cli.md)
- doc: Executes one inner run and updates InnerLoopState.
- signature: `class InnerRunner:`
- members:
  - `_build_lessons_text(self, inner_state: InnerLoopState)` — [`L209`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L209) — Format lessons for injection into stages. — documented in [domains-article_opt-runner](../../../concepts/domains-article_opt-runner.md)
  - `_extract_lessons(self, context: dict, eval_result: dict, run_num: int)` — [`L252`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L252) — Extract structured lessons from this run's outputs and evaluation. — documented in [core-llm_client](../../../concepts/core-llm_client.md)
  - `_run_stage_with_gate(self, stage, context: dict, run_num: int)` — [`L177`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L177) — Run a stage, apply quality gate, retry if needed. Returns (output, score_info, retried). — documented in [domains-article_opt-runner](../../../concepts/domains-article_opt-runner.md)
  - `inject_stage(self, stage: BaseStage, inject_after: str)` — [`L73`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L73) — Insert a generated stage into the pipeline after the named stage. — documented in [domains-article_opt-mechanism_research](../../../concepts/domains-article_opt-mechanism_research.md)
  - `run_once(self, inner_state: InnerLoopState)` — [`L97`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L97) — Execute one full pipeline pass. Updates inner_state and returns RunResult. — documented in [core-state](../../../concepts/core-state.md)
  - `artifacts_base` — [`L57`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L57)
  - `eval_model` — [`L54`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L54)
  - `evaluator` — [`L67`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L67)
  - `max_retries` — [`L56`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L56)
  - `min_score` — [`L55`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L55)
  - `model` — [`L53`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L53)
  - `outer_cycle` — [`L71`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L71) — documented in [domains-article_opt-runner](../../../concepts/domains-article_opt-runner.md)
  - `prompt_overrides` — [`L69`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L69)
  - `stages` — [`L60`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L60) — documented in [domains-article_opt-runner](../../../concepts/domains-article_opt-runner.md)
- protocol/private: `__init__`[`L45`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L45)
- uses (calls/refs, reference-scoped): [`parse_json_response`](../../core/llm_client.md#parse_json_response), [`call_llm`](../../core/llm_client.md#call_llm), [`BaseStage`](pipeline/base.md#BaseStage), [`run_trace`](../../core/state.md#InnerLoopState.run_trace), [`inner_lessons`](../../core/state.md#InnerLoopState.inner_lessons), [`InnerLoopState`](../../core/state.md#InnerLoopState), [`overall`](../../core/state.md#RunResult.overall), [`add_lesson`](../../core/state.md#InnerLoopState.add_lesson), [`evaluate`](evaluator/article_evaluator.md#ArticleEvaluator.evaluate), [`record_run`](../../core/state.md#InnerLoopState.record_run), [`scores`](../../core/state.md#RunResult.scores), [`RunResult`](../../core/state.md#RunResult), [`stage`](../../core/state.md#StageScore.stage), [`StageScore`](../../core/state.md#StageScore), [`ArticleAnalysisStage`](pipeline/article_analysis.md#ArticleAnalysisStage), [`confidence`](../../core/state.md#InnerLesson.confidence), [`inner_skills`](../../core/state.md#InnerLoopState.inner_skills), [`run_number`](../../core/state.md#RunResult.run_number), [`InnerLesson`](../../core/state.md#InnerLesson), [`article_version`](../../core/state.md#RunResult.article_version), [`score`](../../core/state.md#StageScore.score), [`RevisedOutputStage`](pipeline/revised_output.md#RevisedOutputStage), [`article_id`](../../core/state.md#InnerLoopState.article_id), [`name`](pipeline/base.md#BaseStage.name), [`EditPlanningStage`](pipeline/edit_planning.md#EditPlanningStage), [`ImpactAssessmentStage`](pipeline/impact_assessment.md#ImpactAssessmentStage), [`ImprovementHypothesesStage`](pipeline/improvement_hypotheses.md#ImprovementHypothesesStage), [`feedback`](../../core/state.md#StageScore.feedback), [`logger`](runner.md#logger), [`article_working_copy`](../../core/state.md#InnerLoopState.article_working_copy), [`run_number`](../../core/state.md#InnerLesson.run_number), [`stage`](../../core/state.md#InnerLesson.stage), [`reuse_rule`](../../core/state.md#InnerLesson.reuse_rule), [`summary`](../../core/state.md#InnerLesson.summary), [`lesson_type`](../../core/state.md#InnerLesson.lesson_type), [`ArticleEvaluator`](evaluator/article_evaluator.md#ArticleEvaluator), [`retried`](../../core/state.md#StageScore.retried), [`LESSON_SYSTEM`](runner.md#LESSON_SYSTEM)
- used by: [`cmd_mechresearch`](cli.md#cmd_mechresearch), [`validate`](mechanism_research.md#MechanismResearcher.validate), [`cmd_once`](cli.md#cmd_once), [`v`](cli.md#v), [`make_runner`](cli.md#make_runner)  (7 test-only)

## Module values
- `LESSON_SYSTEM` — [`L28`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L28)
- `logger` — [`L26`](../../../../../../raw/code/bilevel-autoresearch/domains/article_opt/runner.py#L26)

