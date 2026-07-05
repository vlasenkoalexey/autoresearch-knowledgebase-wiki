---
title: 'Module: tests/test_inner_loop.py'
type: catalog
provenance: extracted
module: tests/test_inner_loop.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `tests.test_inner_loop`/
symbols:
  _MockRunner.run_once: _MockRunner#run_once().
  TestRunCycleCallCount.test_converges_early_stops_calling_runner: TestRunCycleCallCount#test_converges_early_stops_calling_runner().
  TestRunCycleCallCount.test_budget_exhausted_when_never_converges: TestRunCycleCallCount#test_budget_exhausted_when_never_converges().
  TestInnerLoopControllerInstantiation.test_can_instantiate_with_mock_runner: TestInnerLoopControllerInstantiation#test_can_instantiate_with_mock_runner().
  TestInnerLoopControllerInstantiation.test_custom_parameters_stored: TestInnerLoopControllerInstantiation#test_custom_parameters_stored().
  TestRunCycleCallCount.test_run_once_called_expected_times_with_consecutive_2: TestRunCycleCallCount#test_run_once_called_expected_times_with_consecutive_2().
  _make_outer_state: _make_outer_state().
  _MockRunner: _MockRunner#
  _MockRunner.call_count: _MockRunner#call_count.
  _MockRunner._score: _MockRunner#_score.
  _MockRunner.__init__: _MockRunner#__init__().
  _MockRunner.prompt_overrides: _MockRunner#prompt_overrides.
  _MockRunner.outer_cycle: _MockRunner#outer_cycle.
  _MockRunner.model: _MockRunner#model.
  TestInnerLoopControllerInstantiation: TestInnerLoopControllerInstantiation#
  TestRunCycleCallCount: TestRunCycleCallCount#
---
# Module: [`tests/test_inner_loop.py`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py)

## Classes
### `TestInnerLoopControllerInstantiation`
- def: [`tests/test_inner_loop.py:39`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L39)
- signature: `class TestInnerLoopControllerInstantiation:`
- members:
  - `test_can_instantiate_with_mock_runner(self)` — [`L40`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L40) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `test_custom_parameters_stored(self)` — [`L47`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L47) — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
- uses (calls/refs, reference-scoped): [`InnerLoopController`](../core/inner_loop.md#InnerLoopController), [`convergence_threshold`](../core/inner_loop.md#InnerLoopController.convergence_threshold), [`max_iterations`](../core/inner_loop.md#InnerLoopController.max_iterations), [`runner`](../core/inner_loop.md#InnerLoopController.runner), [`convergence_consecutive`](../core/inner_loop.md#InnerLoopController.convergence_consecutive)  (1 test-only)

### `TestRunCycleCallCount`
- def: [`tests/test_inner_loop.py:60`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L60)
- signature: `class TestRunCycleCallCount:`
- members:
  - `test_budget_exhausted_when_never_converges(self)` — [`L77`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L77) — Runner returns score=5 every time; never converges, should hit max_iterations. — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `test_converges_early_stops_calling_runner(self)` — [`L61`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L61) — Runner returns score=9 every time; convergence_consecutive=3 so it stops at run 3. — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
  - `test_run_once_called_expected_times_with_consecutive_2(self)` — [`L92`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L92) — With convergence_consecutive=2, runner should stop after 2 high-score runs. — documented in [core-inner_loop](../../concepts/core-inner_loop.md)
- uses (calls/refs, reference-scoped): [`run_cycle`](../core/inner_loop.md#InnerLoopController.run_cycle), [`peak_score`](../core/state.md#InnerLoopState.peak_score), [`InnerLoopController`](../core/inner_loop.md#InnerLoopController), [`is_converged`](../core/state.md#InnerLoopState.is_converged)  (3 test-only)

### `_MockRunner`
- def: [`tests/test_inner_loop.py:6`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L6)
- doc: A minimal runner that returns a fixed score without any LLM calls.
- signature: `class _MockRunner:`
- members:
  - `run_once(self, inner: InnerLoopState)` — [`L16`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L16)
  - `call_count` — [`L11`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L11)
  - `model` — [`L14`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L14)
  - `outer_cycle` — [`L13`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L13)
  - `prompt_overrides` — [`L12`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L12)
- protocol/private: `__init__`[`L9`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L9), `_score`[`L10`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L10)
- uses (calls/refs, reference-scoped): [`run_trace`](../core/state.md#InnerLoopState.run_trace), [`InnerLoopState`](../core/state.md#InnerLoopState), [`overall`](../core/state.md#RunResult.overall), [`record_run`](../core/state.md#InnerLoopState.record_run), [`scores`](../core/state.md#RunResult.scores), [`RunResult`](../core/state.md#RunResult), [`stage`](../core/state.md#StageScore.stage), [`StageScore`](../core/state.md#StageScore), [`run_number`](../core/state.md#RunResult.run_number), [`article_version`](../core/state.md#RunResult.article_version), [`score`](../core/state.md#StageScore.score), [`feedback`](../core/state.md#StageScore.feedback), [`article_working_copy`](../core/state.md#InnerLoopState.article_working_copy)
- used by: (5 test-only callers)

## Functions
- `_make_outer_state(article_id: str = "article1", text: str = "hello")` — [`L33`](../../../../../raw/code/bilevel-autoresearch/tests/test_inner_loop.py#L33)

