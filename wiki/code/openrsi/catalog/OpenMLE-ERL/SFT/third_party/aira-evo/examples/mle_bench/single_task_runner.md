---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.examples.mle_bench.single_task_runner`/
symbols:
  main.mirror_latest_node: main().mirror_latest_node().
  main: main().
  main.write_task_stat: main().write_task_stat().
  main.build_operator_config: main().build_operator_config().
  main.count_slime_message_tokens: main().count_slime_message_tokens().
  main.resolve_done_reason: main().resolve_done_reason().
  _load_yaml: _load_yaml().
  main.guard_operator_call: main().guard_operator_call().
  main.guard_operator_call.wrapped: main().guard_operator_call().wrapped().
  main.maybe_build_prompt_config: main().maybe_build_prompt_config().
  main.build_task_progress_state: main().build_task_progress_state().
  _strip_target: _strip_target().
  _safe_int: _safe_int().
  _extract_prompt_messages: _extract_prompt_messages().
  main.build_prompt_config: main().build_prompt_config().
  main.patched_log_journal: main().patched_log_journal().
  main.should_stop_search: main().should_stop_search().
  _merge_generation_kwargs: _merge_generation_kwargs().
  _select_best_available_node: _select_best_available_node().
  StopSearch: StopSearch#
  _prompt_content: _prompt_content().
  _safe_float: _safe_float().
  _extract_completion_artifacts: _extract_completion_artifacts().
  _sum_operator_usage: _sum_operator_usage().
  _safe_task_output_name: _safe_task_output_name().
  _sync_task_link: _sync_task_link().
  main.build_sft_assistant_content: main().build_sft_assistant_content().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py)

## Classes
### `StopSearch`  ·  implements/extends RuntimeError
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py:22`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L22)
- signature: `class StopSearch(RuntimeError):`
- used by: (2 test-only callers)

## Functions
- `_extract_completion_artifacts(operator_metric: dict[str, Any] | None, parse_thinking_tags_fn: Any)` — [`L74`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L74)
- `_extract_prompt_messages(operator_metric: dict[str, Any] | None)` — [`L56`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L56)
- `_load_yaml(path: Path)` — [`L26`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L26)
- `_merge_generation_kwargs(base_kwargs: dict[str, Any], override_kwargs: dict[str, Any])` — [`L34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L34)
- `_prompt_content(message: dict[str, Any])` — [`L49`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L49)
- `_safe_float(value: Any, default: float = 0)` — [`L140`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L140)
- `_safe_int(value: Any, default: int = 0)` — [`L147`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L147)
- `_safe_task_output_name(task_name: str, task_id: str)` — [`L123`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L123)
- `_select_best_available_node(solver: Any)` — [`L112`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L112)
- `_strip_target(payload: dict[str, Any])` — [`L30`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L30)
- `_sum_operator_usage(operator_metrics: list[dict[str, Any]])` — [`L94`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L94)
- `_sync_task_link(src: Path, dst: Path)` — [`L128`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L128)
- `build_operator_config(name: str, relative_path: str)` — [`L375`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L375)
- `build_prompt_config(prompt_payload: dict[str, Any])` — [`L367`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L367)
- `build_sft_assistant_content(*, reasoning_content: str, code: str, response_text: str)` — [`L288`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L288)
- `build_task_progress_state(*, final: bool = False)` — [`L703`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L703)
- `count_slime_message_tokens(*, system_prompt: str, user_prompt: str, response_text: str, reasoning_content: str, code: str)` — [`L306`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L306)
- `guard_operator_call(fn: Any)` — [`L1052`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1052)
- `main()` — [`L154`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L154) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `maybe_build_prompt_config(prompt_payload: dict[str, Any] | None)` — [`L370`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L370)
- `mirror_latest_node()` — [`L739`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L739) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- `patched_log_journal()` — [`L1039`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1039)
- `resolve_done_reason(*, final: bool = False)` — [`L680`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L680)
- `should_stop_search()` — [`L1045`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1045)
- `wrapped(*operator_args: Any, **operator_kwargs: Any)` — [`L1053`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L1053)
- `write_task_stat(*, best_node: Any | None = None, submit_result: dict[str, Any] | None = None, test_time: float = 0)` — [`L601`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/single_task_runner.py#L601)

