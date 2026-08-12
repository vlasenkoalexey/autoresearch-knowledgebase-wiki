---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.tests.test_async_steady_state`/
symbols:
  path: path.
  test_async_worker_retries_same_attempt_after_transient_failure: test_async_worker_retries_same_attempt_after_transient_failure().
  test_async_sampling_honors_fresh_draft_probability: test_async_sampling_honors_fresh_draft_probability().
  test_async_attempts_map_to_virtual_generations_and_budget: test_async_attempts_map_to_virtual_generations_and_budget().
  test_async_node_keeps_its_work_item_metadata: test_async_node_keeps_its_work_item_metadata().
  test_worker_specs_validate_assignment: test_worker_specs_validate_assignment().
  _make_async_solver: _make_async_solver().
  test_async_sandbox_urls_and_round_robin_assignment: test_async_sandbox_urls_and_round_robin_assignment().
  test_async_sandbox_slot_wait_does_not_block_event_loop.probe: test_async_sandbox_slot_wait_does_not_block_event_loop().probe().
  colorama_stub: colorama_stub.
  module_name: module_name.
  make_node: make_node().
  test_gpu_detection_treats_missing_nvidia_smi_as_cpu_only: test_gpu_detection_treats_missing_nvidia_smi_as_cpu_only().
  test_async_mode_with_one_worker_does_not_fall_back_to_generation: test_async_mode_with_one_worker_does_not_fall_back_to_generation().
  test_solution_database_returns_parent_selection_trace_for_async_sampling: test_solution_database_returns_parent_selection_trace_for_async_sampling().
  test_sandbox_task_async_eval_uses_router_url_override: test_sandbox_task_async_eval_uses_router_url_override().
  dataclasses_json_stub: dataclasses_json_stub.
  igraph_stub: igraph_stub.
  AIRA_EVO_DIR: AIRA_EVO_DIR.
  SRC_DIR: SRC_DIR.
  EXAMPLES_MLE_BENCH_DIR: EXAMPLES_MLE_BENCH_DIR.
  test_async_worker_retries_same_attempt_after_transient_failure.flaky_create: test_async_worker_retries_same_attempt_after_transient_failure().flaky_create().
  test_async_sandbox_slot_wait_does_not_block_event_loop.holder: test_async_sandbox_slot_wait_does_not_block_event_loop().holder().
  test_async_sandbox_slot_wait_does_not_block_event_loop.waiter: test_async_sandbox_slot_wait_does_not_block_event_loop().waiter().
  Logger: Logger#
  test_async_worker_count_auto_uses_visible_gpu_count: test_async_worker_count_auto_uses_visible_gpu_count().
  test_execution_mode_is_explicit_and_validated: test_execution_mode_is_explicit_and_validated().
  test_async_time_budget_excludes_task_reported_scheduler_wait: test_async_time_budget_excludes_task_reported_scheduler_wait().
  test_solution_database_restore_is_shared_by_sync_and_async_paths: test_solution_database_restore_is_shared_by_sync_and_async_paths().
  test_generation_mode_rejects_multiple_workers: test_generation_mode_rejects_multiple_workers().
  test_task_concurrency_default_accounts_for_async_workers: test_task_concurrency_default_accounts_for_async_workers().
  test_async_sandbox_slot_wait_does_not_block_event_loop: test_async_sandbox_slot_wait_does_not_block_event_loop().
  REPO_DIR: REPO_DIR.
  EmptySolutionDatabase: EmptySolutionDatabase#
  test_gpu_detection_treats_missing_nvidia_smi_as_cpu_only.missing_binary: test_gpu_detection_treats_missing_nvidia_smi_as_cpu_only().missing_binary().
  test_async_worker_retries_same_attempt_after_transient_failure.tracked_next: test_async_worker_retries_same_attempt_after_transient_failure().tracked_next().
  test_async_worker_retries_same_attempt_after_transient_failure.fake_step_task_async: test_async_worker_retries_same_attempt_after_transient_failure().fake_step_task_async().
  test_async_worker_retries_same_attempt_after_transient_failure.fake_commit_async_node: test_async_worker_retries_same_attempt_after_transient_failure().fake_commit_async_node().
  test_async_worker_retries_same_attempt_after_transient_failure.no_sleep: test_async_worker_retries_same_attempt_after_transient_failure().no_sleep().
  test_async_mode_with_one_worker_does_not_fall_back_to_generation.fake_async_search: test_async_mode_with_one_worker_does_not_fall_back_to_generation().fake_async_search().
  test_sandbox_task_async_eval_uses_router_url_override.fake_run_eval_async: test_sandbox_task_async_eval_uses_router_url_override().fake_run_eval_async().
  test_sandbox_task_async_eval_uses_router_url_override.run_step: test_sandbox_task_async_eval_uses_router_url_override().run_step().
  Logger.info: Logger#info().
  Logger.debug: Logger#debug().
  Logger.warning: Logger#warning().
  Logger.error: Logger#error().
  EmptySolutionDatabase.num_islands: EmptySolutionDatabase#num_islands.
  EmptySolutionDatabase.has_nodes: EmptySolutionDatabase#has_nodes.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py)

## Classes
### `EmptySolutionDatabase`
- def: [`OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py:173`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L173)
- signature: `class EmptySolutionDatabase:`
- members:
  - `has_nodes` — [`L175`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L175)
  - `num_islands` — [`L174`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L174)
- used by: (2 test-only callers)

### `Logger`
- def: [`OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py:70`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L70)
- signature: `class Logger:`
- members:
  - `debug(self, *args, **kwargs)` — [`L74`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L74)
  - `error(self, *args, **kwargs)` — [`L80`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L80)
  - `info(self, *args, **kwargs)` — [`L71`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L71)
  - `warning(self, *args, **kwargs)` — [`L77`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L77)
- used by: (3 test-only callers)

## Functions
- `_make_async_solver(*, execution_mode: str, workers: int = 1)` — [`L178`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L178)
- `fake_async_search(task, state, *, worker_count)` — [`L374`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L374)
- `fake_commit_async_node(**kwargs)` — [`L306`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L306)
- `fake_run_eval_async(code, *, data_dir, sandbox_base_url=None, eval_split=None, job_timeout=None, wait_timeout=None)` — [`L507`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L507)
- `fake_step_task_async(task, state, code, sandbox_url)` — [`L303`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L303)
- `flaky_create(work_item)` — [`L297`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L297)
- `holder(release: asyncio.Event)` — [`L425`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L425)
- `make_node(score: float)` — [`L84`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L84)
- `missing_binary(*args, **kwargs)` — [`L146`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L146)
- `no_sleep(delay)` — [`L310`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L310)
- `probe()` — [`L434`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L434)
- `run_step()` — [`L542`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L542)
- `test_async_attempts_map_to_virtual_generations_and_budget(monkeypatch)` — [`L197`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L197) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `test_async_mode_with_one_worker_does_not_fall_back_to_generation()` — [`L368`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L368)
- `test_async_node_keeps_its_work_item_metadata()` — [`L337`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L337)
- `test_async_sampling_honors_fresh_draft_probability()` — [`L248`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L248) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `test_async_sandbox_slot_wait_does_not_block_event_loop(monkeypatch)` — [`L417`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L417)
- `test_async_sandbox_urls_and_round_robin_assignment()` — [`L157`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L157)
- `test_async_time_budget_excludes_task_reported_scheduler_wait(monkeypatch)` — [`L217`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L217)
- `test_async_worker_count_auto_uses_visible_gpu_count()` — [`L107`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L107) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `test_async_worker_retries_same_attempt_after_transient_failure(monkeypatch)` — [`L275`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L275) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `test_execution_mode_is_explicit_and_validated()` — [`L113`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L113) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `test_generation_mode_rejects_multiple_workers()` — [`L386`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L386)
- `test_gpu_detection_treats_missing_nvidia_smi_as_cpu_only(monkeypatch)` — [`L145`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L145)
- `test_sandbox_task_async_eval_uses_router_url_override(monkeypatch)` — [`L484`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L484)
- `test_solution_database_restore_is_shared_by_sync_and_async_paths()` — [`L234`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L234)
- `test_solution_database_returns_parent_selection_trace_for_async_sampling()` — [`L453`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L453)
- `test_task_concurrency_default_accounts_for_async_workers()` — [`L393`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L393)
- `test_worker_specs_validate_assignment(monkeypatch)` — [`L121`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L121) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `tracked_next(**kwargs)` — [`L292`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L292)
- `waiter(started: asyncio.Event)` — [`L429`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L429)

## Module values
- `AIRA_EVO_DIR` — [`L43`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L43)
- `EXAMPLES_MLE_BENCH_DIR` — [`L45`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L45)
- `REPO_DIR` — [`L42`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L42)
- `SRC_DIR` — [`L44`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L44)
- `colorama_stub` — [`L24`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L24)
- `dataclasses_json_stub` — [`L15`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L15)
- `igraph_stub` — [`L38`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L38)
- `module_name` — [`L19`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L19)
- `path` — [`L46`](../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/tests/test_async_steady_state.py#L46)

