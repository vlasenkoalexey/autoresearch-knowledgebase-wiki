---
title: 'Module: tests/test_train_opt.py'
type: catalog
provenance: extracted
module: tests/test_train_opt.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `tests.test_train_opt`/Test
symbols:
  TestTrainTrace._make_result: TrainTrace#_make_result().
  TestTrainResult.test_basic_creation: TrainResult#test_basic_creation().
  TestTrainTrace.test_add_keep_updates_best: TrainTrace#test_add_keep_updates_best().
  TestTrainTrace.test_add_better_keep_updates_best: TrainTrace#test_add_better_keep_updates_best().
  TestTrainTrace.test_add_worse_keep_does_not_update_best: TrainTrace#test_add_worse_keep_does_not_update_best().
  TestTrainTrace.test_add_discard_does_not_update_best: TrainTrace#test_add_discard_does_not_update_best().
  TestSearchConfig.test_active_params_excludes_frozen: SearchConfig#test_active_params_excludes_frozen().
  TestSearchConfig.test_freeze_all_params: SearchConfig#test_freeze_all_params().
  TestTrainTrace.test_empty_trace_initial_state: TrainTrace#test_empty_trace_initial_state().
  TestTrainTrace.test_add_crash_does_not_update_best: TrainTrace#test_add_crash_does_not_update_best().
  TestTrainTrace.test_results_list_grows: TrainTrace#test_results_list_grows().
  TestTrainTrace.test_summary_contains_best_line: TrainTrace#test_summary_contains_best_line().
  TestTrainTrace.test_summary_last_n_limits_output: TrainTrace#test_summary_last_n_limits_output().
  TestTrainResult._make_result: TrainResult#_make_result().
  TestSearchConfig.test_active_params_full_when_nothing_frozen: SearchConfig#test_active_params_full_when_nothing_frozen().
  TestSearchConfig.test_freeze_a_param: SearchConfig#test_freeze_a_param().
  TestSearchConfig.test_default_strategy_and_guidance: SearchConfig#test_default_strategy_and_guidance().
  TestSearchConfig.test_custom_strategy: SearchConfig#test_custom_strategy().
  TestSearchConfig.test_default_budgets: SearchConfig#test_default_budgets().
  TestTrainResult.test_crash_status: TrainResult#test_crash_status().
  TestSearchConfig.test_default_editable_params_contains_expected: SearchConfig#test_default_editable_params_contains_expected().
  TestTrainResult.test_default_depth_is_zero: TrainResult#test_default_depth_is_zero().
  TestTrainResult.test_custom_depth: TrainResult#test_custom_depth().
  TestTrainResult.test_discard_status: TrainResult#test_discard_status().
  TestTrainResult.test_empty_changes: TrainResult#test_empty_changes().
  TestTrainTrace.test_summary_empty_trace: TrainTrace#test_summary_empty_trace().
  TestSearchConfig: SearchConfig#
  TestTrainResult: TrainResult#
  TestTrainTrace: TrainTrace#
---
# Module: [`tests/test_train_opt.py`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py)

## Classes
### `TestSearchConfig`
- def: [`tests/test_train_opt.py:8`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L8)
- signature: `class TestSearchConfig:`
- members:
  - `test_active_params_excludes_frozen(self)` — [`L21`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L21)
  - `test_active_params_full_when_nothing_frozen(self)` — [`L30`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L30)
  - `test_custom_strategy(self)` — [`L50`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L50)
  - `test_default_budgets(self)` — [`L55`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L55)
  - `test_default_editable_params_contains_expected(self)` — [`L9`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L9)
  - `test_default_strategy_and_guidance(self)` — [`L45`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L45)
  - `test_freeze_a_param(self)` — [`L34`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L34)
  - `test_freeze_all_params(self)` — [`L40`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L40)
- uses (calls/refs, reference-scoped): [`active_params`](../domains/train_opt/config.md#SearchConfig.active_params), [`SearchConfig`](../domains/train_opt/config.md#SearchConfig), [`frozen_params`](../domains/train_opt/config.md#SearchConfig.frozen_params), [`strategy`](../domains/train_opt/config.md#SearchConfig.strategy), [`time_budget`](../domains/train_opt/config.md#SearchConfig.time_budget), [`guidance`](../domains/train_opt/config.md#SearchConfig.guidance), [`editable_params`](../domains/train_opt/config.md#SearchConfig.editable_params), [`inner_budget`](../domains/train_opt/config.md#SearchConfig.inner_budget)

### `TestTrainResult`
- def: [`tests/test_train_opt.py:61`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L61)
- signature: `class TestTrainResult:`
- members:
  - `test_basic_creation(self)` — [`L76`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L76)
  - `test_crash_status(self)` — [`L95`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L95)
  - `test_custom_depth(self)` — [`L87`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L87)
  - `test_default_depth_is_zero(self)` — [`L83`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L83)
  - `test_discard_status(self)` — [`L91`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L91)
  - `test_empty_changes(self)` — [`L100`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L100)
- protocol/private: `_make_result`[`L62`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L62)
- uses (calls/refs, reference-scoped): [`val_bpb`](../domains/train_opt/runner.md#TrainResult.val_bpb), [`status`](../domains/train_opt/runner.md#TrainResult.status), [`iteration`](../domains/train_opt/runner.md#TrainResult.iteration), [`TrainResult`](../domains/train_opt/runner.md#TrainResult), [`changes`](../domains/train_opt/runner.md#TrainResult.changes), [`depth`](../domains/train_opt/runner.md#TrainResult.depth)

### `TestTrainTrace`
- def: [`tests/test_train_opt.py:105`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L105)
- signature: `class TestTrainTrace:`
- members:
  - `test_add_better_keep_updates_best(self)` — [`L130`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L130)
  - `test_add_crash_does_not_update_best(self)` — [`L151`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L151)
  - `test_add_discard_does_not_update_best(self)` — [`L144`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L144)
  - `test_add_keep_updates_best(self)` — [`L124`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L124)
  - `test_add_worse_keep_does_not_update_best(self)` — [`L137`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L137)
  - `test_empty_trace_initial_state(self)` — [`L118`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L118)
  - `test_results_list_grows(self)` — [`L157`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L157)
  - `test_summary_contains_best_line(self)` — [`L163`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L163)
  - `test_summary_empty_trace(self)` — [`L179`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L179)
  - `test_summary_last_n_limits_output(self)` — [`L170`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L170)
- protocol/private: `_make_result`[`L106`](../../../../../raw/code/bilevel-autoresearch/tests/test_train_opt.py#L106)
- uses (calls/refs, reference-scoped): [`add`](../domains/train_opt/runner.md#TrainTrace.add), [`val_bpb`](../domains/train_opt/runner.md#TrainResult.val_bpb), [`status`](../domains/train_opt/runner.md#TrainResult.status), [`best_bpb`](../domains/train_opt/runner.md#TrainTrace.best_bpb), [`results`](../domains/train_opt/runner.md#TrainTrace.results), [`summary`](../domains/train_opt/runner.md#TrainTrace.summary), [`description`](../domains/train_opt/runner.md#TrainResult.description), [`iteration`](../domains/train_opt/runner.md#TrainResult.iteration), [`TrainResult`](../domains/train_opt/runner.md#TrainResult), [`TrainTrace`](../domains/train_opt/runner.md#TrainTrace), [`best_iteration`](../domains/train_opt/runner.md#TrainTrace.best_iteration), [`changes`](../domains/train_opt/runner.md#TrainResult.changes), [`num_params_m`](../domains/train_opt/runner.md#TrainResult.num_params_m), [`peak_vram_mb`](../domains/train_opt/runner.md#TrainResult.peak_vram_mb), [`training_seconds`](../domains/train_opt/runner.md#TrainResult.training_seconds)

