---
title: 'Module: tests/test_state.py'
type: catalog
provenance: extracted
module: tests/test_state.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `tests.test_state`/Test
symbols:
  TestInnerLoopState.test_record_run: InnerLoopState#test_record_run().
  TestRunResult.test_stage_map: RunResult#test_stage_map().
  TestInnerLoopState.test_add_lesson: InnerLoopState#test_add_lesson().
  TestInnerLoopState.test_peak_score: InnerLoopState#test_peak_score().
  TestInnerLoopState.test_runs_to_threshold: InnerLoopState#test_runs_to_threshold().
  TestInnerLoopState.test_runs_to_threshold_never: InnerLoopState#test_runs_to_threshold_never().
  TestInnerLoopState.test_initial_state: InnerLoopState#test_initial_state().
  TestInnerLoopState._make_state: InnerLoopState#_make_state().
  TestInnerLoopState.test_peak_score_empty: InnerLoopState#test_peak_score_empty().
  TestRunResult: RunResult#
  TestInnerLoopState: InnerLoopState#
---
# Module: [`tests/test_state.py`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py)

## Classes
### `TestInnerLoopState`
- def: [`tests/test_state.py:15`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L15)
- signature: `class TestInnerLoopState:`
- members:
  - `test_add_lesson(self)` — [`L64`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L64)
  - `test_initial_state(self)` — [`L19`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L19) — documented in [core-state](../../concepts/core-state.md)
  - `test_peak_score(self)` — [`L37`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L37)
  - `test_peak_score_empty(self)` — [`L45`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L45)
  - `test_record_run(self)` — [`L25`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L25) — documented in [core-state](../../concepts/core-state.md)
  - `test_runs_to_threshold(self)` — [`L49`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L49)
  - `test_runs_to_threshold_never(self)` — [`L57`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L57)
- protocol/private: `_make_state`[`L16`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L16)
- uses (calls/refs, reference-scoped): [`run_trace`](../core/state.md#InnerLoopState.run_trace), [`inner_lessons`](../core/state.md#InnerLoopState.inner_lessons), [`InnerLoopState`](../core/state.md#InnerLoopState), [`overall`](../core/state.md#RunResult.overall), [`add_lesson`](../core/state.md#InnerLoopState.add_lesson), [`record_run`](../core/state.md#InnerLoopState.record_run), [`peak_score`](../core/state.md#InnerLoopState.peak_score), [`scores`](../core/state.md#RunResult.scores), [`RunResult`](../core/state.md#RunResult), [`runs_to_threshold`](../core/state.md#InnerLoopState.runs_to_threshold), [`stage`](../core/state.md#StageScore.stage), [`StageScore`](../core/state.md#StageScore), [`confidence`](../core/state.md#InnerLesson.confidence), [`run_number`](../core/state.md#RunResult.run_number), [`InnerLesson`](../core/state.md#InnerLesson), [`article_version`](../core/state.md#RunResult.article_version), [`score`](../core/state.md#StageScore.score), [`article_id`](../core/state.md#InnerLoopState.article_id), [`feedback`](../core/state.md#StageScore.feedback), [`article_working_copy`](../core/state.md#InnerLoopState.article_working_copy), [`run_number`](../core/state.md#InnerLesson.run_number), [`stage`](../core/state.md#InnerLesson.stage), [`reuse_rule`](../core/state.md#InnerLesson.reuse_rule), [`summary`](../core/state.md#InnerLesson.summary), [`lesson_type`](../core/state.md#InnerLesson.lesson_type)

### `TestRunResult`
- def: [`tests/test_state.py:5`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L5)
- signature: `class TestRunResult:`
- members:
  - `test_stage_map(self)` — [`L6`](../../../../../raw/code/bilevel-autoresearch/tests/test_state.py#L6)
- uses (calls/refs, reference-scoped): [`overall`](../core/state.md#RunResult.overall), [`scores`](../core/state.md#RunResult.scores), [`RunResult`](../core/state.md#RunResult), [`stage_map`](../core/state.md#RunResult.stage_map), [`stage`](../core/state.md#StageScore.stage), [`StageScore`](../core/state.md#StageScore), [`run_number`](../core/state.md#RunResult.run_number), [`article_version`](../core/state.md#RunResult.article_version), [`score`](../core/state.md#StageScore.score), [`feedback`](../core/state.md#StageScore.feedback)

