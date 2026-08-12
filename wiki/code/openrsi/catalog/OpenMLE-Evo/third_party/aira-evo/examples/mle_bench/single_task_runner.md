---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.examples.mle_bench.single_task_runner`/
symbols:
  main.write_task_stat: main().write_task_stat().
  main: main().
  main.build_operator_config: main().build_operator_config().
  _select_best_available_node: _select_best_available_node().
  main.mirror_latest_node: main().mirror_latest_node().
  _coerce_float_value: _coerce_float_value().
  _reconcile_resume_steps_with_checkpoint: _reconcile_resume_steps_with_checkpoint().
  main.submit_score_from_result: main().submit_score_from_result().
  _naturebench_valid_score_from_node: _naturebench_valid_score_from_node().
  main.coerce_float: main().coerce_float().
  _load_yaml: _load_yaml().
  _naturebench_score_from_node: _naturebench_score_from_node().
  main.guard_operator_call: main().guard_operator_call().
  _is_naturebench_successful_node: _is_naturebench_successful_node().
  _should_run_final_submit: _should_run_final_submit().
  _naturebench_leaderboard_flags: _naturebench_leaderboard_flags().
  _select_method2_oracle_score: _select_method2_oracle_score().
  main.select_best_submit_result: main().select_best_submit_result().
  main.build_submit_attempt_payload: main().build_submit_attempt_payload().
  main.guard_operator_call.wrapped: main().guard_operator_call().wrapped().
  _naturebench_successful_aux_info: _naturebench_successful_aux_info().
  _naturebench_score_from_aux_info: _naturebench_score_from_aux_info().
  main.maybe_build_prompt_config: main().maybe_build_prompt_config().
  _node_selection_score: _node_selection_score().
  _score_is_better_value: _score_is_better_value().
  main.score_is_better: main().score_is_better().
  _strip_target: _strip_target().
  _node_aux_info: _node_aux_info().
  _solver_defaults_relative_path: _solver_defaults_relative_path().
  _extract_prompt_messages: _extract_prompt_messages().
  _effective_submit_score: _effective_submit_score().
  _submit_score_from_result: _submit_score_from_result().
  _archive_orphan_step_dirs: _archive_orphan_step_dirs().
  main.build_prompt_config: main().build_prompt_config().
  main.patched_log_journal: main().patched_log_journal().
  main.should_stop_search: main().should_stop_search().
  _merge_generation_kwargs: _merge_generation_kwargs().
  _step_index_from_payload: _step_index_from_payload().
  StopSearch: StopSearch#
  _benchmark_name: _benchmark_name().
  _prompt_content: _prompt_content().
  _node_sort_key: _node_sort_key().
  _final_score_source: _final_score_source().
  main.mean_or_none: main().mean_or_none().
  _operator_paths_for_benchmark: _operator_paths_for_benchmark().
  _load_naturebench_task_class: _load_naturebench_task_class().
  _sum_operator_usage: _sum_operator_usage().
  _coerce_bool: _coerce_bool().
  _nested_cfg_get: _nested_cfg_get().
  NATUREBENCH_SURPASS_SOTA_THRESHOLD: NATUREBENCH_SURPASS_SOTA_THRESHOLD.
  _step_index_from_experience_card: _step_index_from_experience_card().
  _resolve_step_schedule_metadata: _resolve_step_schedule_metadata().
  _load_checkpoint_current_step: _load_checkpoint_current_step().
  _step_validation_time: _step_validation_time().
  _next_archive_path: _next_archive_path().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py)

## Classes
### `StopSearch`  ·  implements/extends RuntimeError
- def: [`OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py:23`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L23)
- signature: `class StopSearch(RuntimeError):`
- used by: (2 test-only callers)

## Functions
- `_archive_orphan_step_dirs(output_dir: Path, orphan_step_indices: set[int])` — [`L493`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L493)
- `_benchmark_name(task_cfg: dict[str, Any])` — [`L31`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L31)
- `_coerce_bool(value: Any, *, default: bool = False)` — [`L216`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L216)
- `_coerce_float_value(value: Any)` — [`L280`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L280)
- `_effective_submit_score(*, benchmark: str, submit_score: Any, final_selection_score: Any, final_submit_enabled: bool)` — [`L257`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L257)
- `_extract_prompt_messages(operator_metric: dict[str, Any] | None)` — [`L118`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L118)
- `_final_score_source(selected_source: str | None, aux_source: Any | None)` — [`L274`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L274)
- `_is_naturebench_successful_node(node: Any)` — [`L212`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L212)
- `_load_checkpoint_current_step(checkpoint_dir: Path)` — [`L451`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L451)
- `_load_naturebench_task_class(example_dir: Path)` — [`L79`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L79)
- `_load_yaml(path: Path)` — [`L27`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L27)
- `_merge_generation_kwargs(base_kwargs: dict[str, Any], override_kwargs: dict[str, Any])` — [`L96`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L96)
- `_naturebench_leaderboard_flags(score: Any)` — [`L293`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L293) — Return the official Lite/leaderboard threshold flags for a valid g score.
- `_naturebench_score_from_aux_info(aux_info: dict[str, Any])` — [`L186`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L186)
- `_naturebench_score_from_node(node: Any)` — [`L201`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L201)
- `_naturebench_successful_aux_info(aux_info: dict[str, Any])` — [`L178`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L178)
- `_naturebench_valid_score_from_node(node: Any)` — [`L205`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L205)
- `_nested_cfg_get(payload: dict[str, Any], keys: tuple[str, ...], default: Any)` — [`L226`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L226)
- `_next_archive_path(archive_root: Path, step_dir_name: str)` — [`L484`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L484)
- `_node_aux_info(node: Any)` — [`L163`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L163)
- `_node_selection_score(node: Any)` — [`L169`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L169)
- `_node_sort_key(node: Any)` — [`L154`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L154)
- `_operator_paths_for_benchmark(benchmark: str, *, experience_enabled: bool)` — [`L44`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L44)
- `_prompt_content(message: dict[str, Any])` — [`L111`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L111)
- `_reconcile_resume_steps_with_checkpoint(output_dir: Path, checkpoint_dir: Path, existing_task_stat: dict[str, Any])` — [`L509`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L509)
- `_resolve_step_schedule_metadata(node: Any, solver: Any)` — [`L428`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L428)
- `_score_is_better_value(candidate: Any, incumbent: Any, *, higher_is_better: bool)` — [`L305`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L305)
- `_select_best_available_node(solver: Any, *, seed: int, task_name: str, sample_index: int, benchmark: str = "mlebench")` — [`L367`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L367)
- `_select_method2_oracle_score(*, final_test_score: Any, submit_test_score: Any, higher_is_better: bool)` — [`L341`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L341)
- `_should_run_final_submit(*, benchmark: str, submit_repeats: int, task_cfg: dict[str, Any], runner_cfg: dict[str, Any])` — [`L237`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L237)
- `_solver_defaults_relative_path(task_cfg: dict[str, Any])` — [`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L35)
- `_step_index_from_experience_card(card: dict[str, Any])` — [`L421`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L421)
- `_step_index_from_payload(step_payload: dict[str, Any])` — [`L414`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L414)
- `_step_validation_time(step_payload: dict[str, Any])` — [`L465`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L465)
- `_strip_target(payload: dict[str, Any])` — [`L92`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L92)
- `_submit_score_from_result(result: dict[str, Any] | None, *, evaluation_protocol: str)` — [`L322`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L322)
- `_sum_operator_usage(operator_metrics: list[dict[str, Any]])` — [`L136`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L136)
- `build_operator_config(name: str, relative_path: str)` — [`L758`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L758)
- `build_prompt_config(prompt_payload: dict[str, Any])` — [`L750`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L750)
- `build_submit_attempt_payload(result: dict[str, Any], *, attempt_index: int, leaderboard: Any | None)` — [`L672`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L672)
- `coerce_float(value: Any)` — [`L644`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L644)
- `guard_operator_call(fn: Any)` — [`L1615`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1615)
- `main()` — [`L559`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L559)
- `maybe_build_prompt_config(prompt_payload: dict[str, Any] | None)` — [`L753`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L753)
- `mean_or_none(values: list[float])` — [`L701`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L701)
- `mirror_latest_node()` — [`L1385`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1385)
- `patched_log_journal()` — [`L1592`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1592)
- `score_is_better(candidate: Any, incumbent: Any)` — [`L647`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L647)
- `select_best_submit_result(submit_results: list[dict[str, Any]])` — [`L660`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L660)
- `should_stop_search()` — [`L1598`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1598)
- `submit_score_from_result(result: dict[str, Any] | None)` — [`L654`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L654)
- `wrapped(*operator_args: Any, **operator_kwargs: Any)` — [`L1616`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1616)
- `write_task_stat(*, best_node: Any | None = None, submit_result: dict[str, Any] | None = None, submit_results: list[dict[str, Any]] | None = None, test_time: float = 0)` — [`L1050`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1050) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)

## Module values
- `NATUREBENCH_SURPASS_SOTA_THRESHOLD` — [`L290`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L290)

