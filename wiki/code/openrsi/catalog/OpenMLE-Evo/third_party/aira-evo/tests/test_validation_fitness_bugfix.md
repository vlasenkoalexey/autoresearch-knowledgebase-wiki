---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.tests.test_validation_fitness_bugfix`/
symbols:
  test_evo_debug_cycle_logs_each_node_before_next_debug_attempt: test_evo_debug_cycle_logs_each_node_before_next_debug_attempt().
  test_evo_debug_cycle_defers_journal_logging_without_experience_mode: test_evo_debug_cycle_defers_journal_logging_without_experience_mode().
  test_sandbox_http_client_verifies_tls_by_default: test_sandbox_http_client_verifies_tls_by_default().
  colorama_stub: colorama_stub.
  build_solver: build_solver().
  module_name: module_name.
  build_sandbox_task: build_sandbox_task().
  test_evo_parent_selection_switches_between_original_and_experience_modes: test_evo_parent_selection_switches_between_original_and_experience_modes().
  dataclasses_json_stub: dataclasses_json_stub.
  igraph_stub: igraph_stub.
  EXAMPLES_MLE_BENCH_DIR: EXAMPLES_MLE_BENCH_DIR.
  test_validation_fitness_marks_node_as_non_buggy: test_validation_fitness_marks_node_as_non_buggy().
  test_evolutionary_experience_mode_skips_analyze_for_validation_fitness: test_evolutionary_experience_mode_skips_analyze_for_validation_fitness().
  test_evolutionary_validation_fitness_sanitizes_analysis_summary: test_evolutionary_validation_fitness_sanitizes_analysis_summary().
  test_sandbox_task_does_not_trust_model_reported_validation_score_by_default: test_sandbox_task_does_not_trust_model_reported_validation_score_by_default().
  test_sandbox_task_can_explicitly_enable_model_reported_validation_score: test_sandbox_task_can_explicitly_enable_model_reported_validation_score().
  test_sandbox_step_task_uses_self_validation_for_validation_fitness: test_sandbox_step_task_uses_self_validation_for_validation_fitness().
  test_sandbox_evaluate_fitness_reports_test_fitness: test_sandbox_evaluate_fitness_reports_test_fitness().
  test_evo_parent_selection_switches_between_original_and_experience_modes.Logger: test_evo_parent_selection_switches_between_original_and_experience_modes().Logger#
  test_evo_parent_selection_switches_between_original_and_experience_modes.make_search_node: test_evo_parent_selection_switches_between_original_and_experience_modes().make_search_node().
  build_solver.analyze: build_solver().analyze().
  test_sandbox_http_client_verifies_tls_by_default.FakeClient: test_sandbox_http_client_verifies_tls_by_default().FakeClient#
  test_sandbox_http_client_verifies_tls_by_default.fake_get_sandbox_result: test_sandbox_http_client_verifies_tls_by_default().fake_get_sandbox_result().
  test_evo_debug_cycle_logs_each_node_before_next_debug_attempt.log_journal: test_evo_debug_cycle_logs_each_node_before_next_debug_attempt().log_journal().
  test_evo_debug_cycle_logs_each_node_before_next_debug_attempt.debug: test_evo_debug_cycle_logs_each_node_before_next_debug_attempt().debug().
  test_evo_debug_cycle_logs_each_node_before_next_debug_attempt.parse_eval_result: test_evo_debug_cycle_logs_each_node_before_next_debug_attempt().parse_eval_result().
  test_evo_debug_cycle_logs_each_node_before_next_debug_attempt.Task: test_evo_debug_cycle_logs_each_node_before_next_debug_attempt().Task#
  test_evo_debug_cycle_defers_journal_logging_without_experience_mode.log_journal: test_evo_debug_cycle_defers_journal_logging_without_experience_mode().log_journal().
  test_evo_debug_cycle_defers_journal_logging_without_experience_mode.debug: test_evo_debug_cycle_defers_journal_logging_without_experience_mode().debug().
  test_evo_debug_cycle_defers_journal_logging_without_experience_mode.parse_eval_result: test_evo_debug_cycle_defers_journal_logging_without_experience_mode().parse_eval_result().
  test_evo_debug_cycle_defers_journal_logging_without_experience_mode.Task: test_evo_debug_cycle_defers_journal_logging_without_experience_mode().Task#
  test_sandbox_http_client_verifies_tls_by_default.FakeClient.__init__: test_sandbox_http_client_verifies_tls_by_default().FakeClient#__init__().
  test_sandbox_http_client_verifies_tls_by_default.FakeClient.__aenter__: test_sandbox_http_client_verifies_tls_by_default().FakeClient#__aenter__().
  test_sandbox_http_client_verifies_tls_by_default.FakeClient.__aexit__: test_sandbox_http_client_verifies_tls_by_default().FakeClient#__aexit__().
  test_evo_debug_cycle_logs_each_node_before_next_debug_attempt.Task.step_task: test_evo_debug_cycle_logs_each_node_before_next_debug_attempt().Task#step_task().
  test_evo_debug_cycle_defers_journal_logging_without_experience_mode.Task.step_task: test_evo_debug_cycle_defers_journal_logging_without_experience_mode().Task#step_task().
  test_evo_parent_selection_switches_between_original_and_experience_modes.Logger.info: test_evo_parent_selection_switches_between_original_and_experience_modes().Logger#info().
  test_evo_parent_selection_switches_between_original_and_experience_modes.Logger.debug: test_evo_parent_selection_switches_between_original_and_experience_modes().Logger#debug().
  test_evo_parent_selection_switches_between_original_and_experience_modes.Logger.warning: test_evo_parent_selection_switches_between_original_and_experience_modes().Logger#warning().
  test_evo_parent_selection_switches_between_original_and_experience_modes.Logger.error: test_evo_parent_selection_switches_between_original_and_experience_modes().Logger#error().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py)

## Classes
### `FakeClient`
- def: [`OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py:219`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L219)
- signature: `class FakeClient:`
- protocol/private: `__aenter__`[`L223`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L223), `__aexit__`[`L226`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L226), `__init__`[`L220`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L220)
- used by: (1 test-only callers)

### `Logger`
- def: [`OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py:425`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L425)
- signature: `class Logger:`
- members:
  - `debug(self, *args, **kwargs)` — [`L429`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L429)
  - `error(self, *args, **kwargs)` — [`L435`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L435)
  - `info(self, *args, **kwargs)` — [`L426`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L426)
  - `warning(self, *args, **kwargs)` — [`L432`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L432)
- used by: (1 test-only callers)

### `Task`
- def: [`OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py:408`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L408)
- signature: `class Task:`
- members:
  - `step_task(self, state, code)` — [`L342`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L342)
  - `step_task(self, state, code)` — [`L409`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L409)
- used by: (1 test-only callers)

## Functions
- `analyze(node)` — [`L68`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L68)
- `build_sandbox_task(*, use_clear_run_log_score=True, trust_model_validation_score=False)` — [`L149`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L149)
- `build_solver(solver_cls)` — [`L61`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L61)
- `debug(parent)` — [`L322`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L322)
- `debug(parent)` — [`L390`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L390)
- `fake_get_sandbox_result(**kwargs)` — [`L229`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L229)
- `log_journal()` — [`L306`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L306)
- `log_journal()` — [`L376`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L376)
- `make_search_node(score: float, official_score: float)` — [`L438`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L438)
- `parse_eval_result(node, eval_result)` — [`L333`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L333)
- `parse_eval_result(node, eval_result)` — [`L400`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L400)
- `test_evo_debug_cycle_defers_journal_logging_without_experience_mode()` — [`L359`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L359)
- `test_evo_debug_cycle_logs_each_node_before_next_debug_attempt()` — [`L289`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L289)
- `test_evo_parent_selection_switches_between_original_and_experience_modes()` — [`L424`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L424)
- `test_evolutionary_experience_mode_skips_analyze_for_validation_fitness()` — [`L96`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L96)
- `test_evolutionary_validation_fitness_sanitizes_analysis_summary()` — [`L114`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L114)
- `test_sandbox_evaluate_fitness_reports_test_fitness()` — [`L272`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L272)
- `test_sandbox_http_client_verifies_tls_by_default(monkeypatch)` — [`L215`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L215)
- `test_sandbox_step_task_uses_self_validation_for_validation_fitness()` — [`L251`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L251)
- `test_sandbox_task_can_explicitly_enable_model_reported_validation_score()` — [`L196`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L196)
- `test_sandbox_task_does_not_trust_model_reported_validation_score_by_default()` — [`L175`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L175)
- `test_validation_fitness_marks_node_as_non_buggy(solver_cls)` — [`L77`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L77)

## Module values
- `EXAMPLES_MLE_BENCH_DIR` — [`L54`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L54)
- `colorama_stub` — [`L22`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L22)
- `dataclasses_json_stub` — [`L13`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L13)
- `igraph_stub` — [`L36`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L36)
- `module_name` — [`L17`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_validation_fitness_bugfix.py#L17)

