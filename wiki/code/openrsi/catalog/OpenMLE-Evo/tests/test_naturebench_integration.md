---
title: 'Module: OpenMLE-Evo/tests/test_naturebench_integration.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tests/test_naturebench_integration.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tests.test_naturebench_integration`/
symbols:
  REPO_ROOT: REPO_ROOT.
  _load_module: _load_module().
  Node.metric: Node#metric.
  test_naturebench_concurrent_attempts_keep_distinct_workspaces: test_naturebench_concurrent_attempts_keep_distinct_workspaces().
  test_naturebench_build_tasks_writes_airaevo_config: test_naturebench_build_tasks_writes_airaevo_config().
  test_naturebench_build_tasks_extracts_empirical_eda_addendum: test_naturebench_build_tasks_extracts_empirical_eda_addendum().
  test_naturebench_build_tasks_uses_task_set_resource_labels: test_naturebench_build_tasks_uses_task_set_resource_labels().
  test_naturebench_build_tasks_uses_official_scm_resource_lines: test_naturebench_build_tasks_uses_official_scm_resource_lines().
  test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable: test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable().
  test_naturebench_build_tasks_allows_zero_submit_repeats: test_naturebench_build_tasks_allows_zero_submit_repeats().
  test_naturebench_task_uses_current_aggregate_improvement_as_fitness: test_naturebench_task_uses_current_aggregate_improvement_as_fitness().
  test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate: test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate().
  test_naturebench_preflight_blocks_package_install_without_evaluation: test_naturebench_preflight_blocks_package_install_without_evaluation().
  test_naturebench_scm_gpu_wait_is_reported_separately: test_naturebench_scm_gpu_wait_is_reported_separately().
  test_naturebench_task_registers_eval_service_once_before_evaluation: test_naturebench_task_registers_eval_service_once_before_evaluation().
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().
  test_naturebench_scm_ssh_retries_transient_connection_close: test_naturebench_scm_ssh_retries_transient_connection_close().
  test_naturebench_docker_timeout_forcibly_removes_named_container: test_naturebench_docker_timeout_forcibly_removes_named_container().
  _write_fake_naturebench_task: _write_fake_naturebench_task().
  test_naturebench_runner_uses_naturebench_task_and_prompt_paths: test_naturebench_runner_uses_naturebench_task_and_prompt_paths().
  test_naturebench_final_submit_is_disabled_by_default_and_uses_search_score: test_naturebench_final_submit_is_disabled_by_default_and_uses_search_score().
  test_naturebench_final_selection_ignores_failed_high_score_nodes: test_naturebench_final_selection_ignores_failed_high_score_nodes().
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Node: test_naturebench_final_selection_ignores_failed_high_score_nodes().Node#
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Solver.__init__: test_naturebench_final_selection_ignores_failed_high_score_nodes().Solver#__init__().
  Solver.journal: Solver#journal.
  test_naturebench_leaderboard_flags_use_official_thresholds: test_naturebench_leaderboard_flags_use_official_thresholds().
  test_naturebench_valid_final_score_requires_successful_node: test_naturebench_valid_final_score_requires_successful_node().
  test_naturebench_skipped_submit_outputs_count_as_completed: test_naturebench_skipped_submit_outputs_count_as_completed().
  test_evaluate_naturebench_payloads_point_to_naturebench_builder_and_runner: test_evaluate_naturebench_payloads_point_to_naturebench_builder_and_runner().
  test_naturebench_remote_tar_command_quotes_workspace_component: test_naturebench_remote_tar_command_quotes_workspace_component().
  test_naturebench_local_candidate_env_does_not_inherit_secrets: test_naturebench_local_candidate_env_does_not_inherit_secrets().
  test_runner_config_redaction_removes_nested_api_keys: test_runner_config_redaction_removes_nested_api_keys().
  test_naturebench_scm_ssh_retries_transient_connection_close.fake_run: test_naturebench_scm_ssh_retries_transient_connection_close().fake_run().
  test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable.FailedProcess.stderr: test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable().FailedProcess#stderr.
  test_naturebench_scm_gpu_wait_is_reported_separately.CapturingTask._ssh: test_naturebench_scm_gpu_wait_is_reported_separately().CapturingTask#_ssh().
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag.CapturingTask._ssh: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().CapturingTask#_ssh().
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool.CapturingTask._ssh: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().CapturingTask#_ssh().
  test_naturebench_operator_templates_accept_verified_visible_data_analysis: test_naturebench_operator_templates_accept_verified_visible_data_analysis().
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Journal.__init__: test_naturebench_final_selection_ignores_failed_high_score_nodes().Journal#__init__().
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Journal.is_root_node: test_naturebench_final_selection_ignores_failed_high_score_nodes().Journal#is_root_node().
  test_naturebench_valid_final_score_requires_successful_node.Node.__init__: test_naturebench_valid_final_score_requires_successful_node().Node#__init__().
  test_naturebench_operator_prompts_use_output_dir_not_submission_csv: test_naturebench_operator_prompts_use_output_dir_not_submission_csv().
  test_naturebench_default_configs_skip_submit_and_reduce_search_artifacts: test_naturebench_default_configs_skip_submit_and_reduce_search_artifacts().
  test_naturebench_summary_does_not_require_mle_leaderboard: test_naturebench_summary_does_not_require_mle_leaderboard().
  test_generic_llm_converts_generation_kwargs_to_plain_containers: test_generic_llm_converts_generation_kwargs_to_plain_containers().
  test_naturebench_scm_ssh_retries_transient_connection_close.FakeCompletedProcess: test_naturebench_scm_ssh_retries_transient_connection_close().FakeCompletedProcess#
  test_naturebench_valid_final_score_requires_successful_node.Node: test_naturebench_valid_final_score_requires_successful_node().Node#
  test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable.FailedProcess: test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable().FailedProcess#
  test_naturebench_task_uses_current_aggregate_improvement_as_fitness.FakeNatureBenchTask: test_naturebench_task_uses_current_aggregate_improvement_as_fitness().FakeNatureBenchTask#
  test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate.FakeNatureBenchTask: test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate().FakeNatureBenchTask#
  test_naturebench_preflight_blocks_package_install_without_evaluation.CountingTask: test_naturebench_preflight_blocks_package_install_without_evaluation().CountingTask#
  test_naturebench_scm_gpu_wait_is_reported_separately.FakeCompletedProcess: test_naturebench_scm_gpu_wait_is_reported_separately().FakeCompletedProcess#
  test_naturebench_scm_gpu_wait_is_reported_separately.CapturingTask: test_naturebench_scm_gpu_wait_is_reported_separately().CapturingTask#
  test_naturebench_task_registers_eval_service_once_before_evaluation.RegisteringFakeNatureBenchTask: test_naturebench_task_registers_eval_service_once_before_evaluation().RegisteringFakeNatureBenchTask#
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag.FakeCompletedProcess: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().FakeCompletedProcess#
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag.CapturingTask: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().CapturingTask#
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool.FakeCompletedProcess: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().FakeCompletedProcess#
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool.CapturingTask: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().CapturingTask#
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Metric: test_naturebench_final_selection_ignores_failed_high_score_nodes().Metric#
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Journal: test_naturebench_final_selection_ignores_failed_high_score_nodes().Journal#
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Solver: test_naturebench_final_selection_ignores_failed_high_score_nodes().Solver#
  test_solutions_database_can_force_a_fresh_draft_after_repeated_error.Logger: test_solutions_database_can_force_a_fresh_draft_after_repeated_error().Logger#
  test_solutions_database_can_force_a_fresh_draft_after_repeated_error.Node: test_solutions_database_can_force_a_fresh_draft_after_repeated_error().Node#
  test_naturebench_valid_final_score_requires_successful_node.Metric: test_naturebench_valid_final_score_requires_successful_node().Metric#
  test_generic_llm_converts_generation_kwargs_to_plain_containers.FakeClient: test_generic_llm_converts_generation_kwargs_to_plain_containers().FakeClient#
  test_naturebench_concurrent_attempts_keep_distinct_workspaces.ConcurrentTask: test_naturebench_concurrent_attempts_keep_distinct_workspaces().ConcurrentTask#
  test_naturebench_concurrent_attempts_keep_distinct_workspaces.run_candidate: test_naturebench_concurrent_attempts_keep_distinct_workspaces().run_candidate().
  test_naturebench_docker_timeout_forcibly_removes_named_container.fake_run: test_naturebench_docker_timeout_forcibly_removes_named_container().fake_run().
  test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable.FailedProcess.returncode: test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable().FailedProcess#returncode.
  test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable.FailedProcess.stdout: test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable().FailedProcess#stdout.
  test_naturebench_task_uses_current_aggregate_improvement_as_fitness.FakeNatureBenchTask._run_solution: test_naturebench_task_uses_current_aggregate_improvement_as_fitness().FakeNatureBenchTask#_run_solution().
  test_naturebench_task_uses_current_aggregate_improvement_as_fitness.FakeNatureBenchTask._post_evaluate: test_naturebench_task_uses_current_aggregate_improvement_as_fitness().FakeNatureBenchTask#_post_evaluate().
  test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate.FakeNatureBenchTask._run_solution: test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate().FakeNatureBenchTask#_run_solution().
  test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate.FakeNatureBenchTask._post_evaluate: test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate().FakeNatureBenchTask#_post_evaluate().
  test_naturebench_preflight_blocks_package_install_without_evaluation.CountingTask._run_solution: test_naturebench_preflight_blocks_package_install_without_evaluation().CountingTask#_run_solution().
  test_naturebench_preflight_blocks_package_install_without_evaluation.CountingTask._post_evaluate: test_naturebench_preflight_blocks_package_install_without_evaluation().CountingTask#_post_evaluate().
  test_naturebench_scm_gpu_wait_is_reported_separately.FakeCompletedProcess.returncode: test_naturebench_scm_gpu_wait_is_reported_separately().FakeCompletedProcess#returncode.
  test_naturebench_scm_gpu_wait_is_reported_separately.FakeCompletedProcess.stdout: test_naturebench_scm_gpu_wait_is_reported_separately().FakeCompletedProcess#stdout.
  test_naturebench_scm_gpu_wait_is_reported_separately.FakeCompletedProcess.stderr: test_naturebench_scm_gpu_wait_is_reported_separately().FakeCompletedProcess#stderr.
  test_naturebench_scm_gpu_wait_is_reported_separately.CapturingTask._sync_workspace_to_scm: test_naturebench_scm_gpu_wait_is_reported_separately().CapturingTask#_sync_workspace_to_scm().
  test_naturebench_scm_gpu_wait_is_reported_separately.CapturingTask._resolve_scm_task_root: test_naturebench_scm_gpu_wait_is_reported_separately().CapturingTask#_resolve_scm_task_root().
  test_naturebench_task_registers_eval_service_once_before_evaluation.RegisteringFakeNatureBenchTask._run_solution: test_naturebench_task_registers_eval_service_once_before_evaluation().RegisteringFakeNatureBenchTask#_run_solution().
  test_naturebench_task_registers_eval_service_once_before_evaluation.RegisteringFakeNatureBenchTask._post_json: test_naturebench_task_registers_eval_service_once_before_evaluation().RegisteringFakeNatureBenchTask#_post_json().
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag.FakeCompletedProcess.returncode: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().FakeCompletedProcess#returncode.
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag.FakeCompletedProcess.stdout: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().FakeCompletedProcess#stdout.
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag.FakeCompletedProcess.stderr: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().FakeCompletedProcess#stderr.
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag.CapturingTask._sync_workspace_to_scm: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().CapturingTask#_sync_workspace_to_scm().
  test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag.CapturingTask._resolve_scm_task_root: test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag().CapturingTask#_resolve_scm_task_root().
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool.FakeCompletedProcess.returncode: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().FakeCompletedProcess#returncode.
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool.FakeCompletedProcess.stdout: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().FakeCompletedProcess#stdout.
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool.FakeCompletedProcess.stderr: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().FakeCompletedProcess#stderr.
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool.CapturingTask._sync_workspace_to_scm: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().CapturingTask#_sync_workspace_to_scm().
  test_naturebench_scm_docker_uses_shared_gpu_slot_pool.CapturingTask._resolve_scm_task_root: test_naturebench_scm_docker_uses_shared_gpu_slot_pool().CapturingTask#_resolve_scm_task_root().
  test_naturebench_scm_ssh_retries_transient_connection_close.FakeCompletedProcess.__init__: test_naturebench_scm_ssh_retries_transient_connection_close().FakeCompletedProcess#__init__().
  FakeCompletedProcess.returncode: FakeCompletedProcess#returncode.
  FakeCompletedProcess.stdout: FakeCompletedProcess#stdout.
  FakeCompletedProcess.stderr: FakeCompletedProcess#stderr.
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Metric.__init__: test_naturebench_final_selection_ignores_failed_high_score_nodes().Metric#__init__().
  Metric.value: Metric#value.
  Metric.info: Metric#info.
  test_naturebench_final_selection_ignores_failed_high_score_nodes.Node.__init__: test_naturebench_final_selection_ignores_failed_high_score_nodes().Node#__init__().
  Node.id: Node#id.
  Node.step: Node#step.
  Node.code: Node#code.
  Journal.nodes: Journal#nodes.
  test_solutions_database_can_force_a_fresh_draft_after_repeated_error: test_solutions_database_can_force_a_fresh_draft_after_repeated_error().
  test_solutions_database_can_force_a_fresh_draft_after_repeated_error.Logger.info: test_solutions_database_can_force_a_fresh_draft_after_repeated_error().Logger#info().
  test_solutions_database_can_force_a_fresh_draft_after_repeated_error.Logger.warning: test_solutions_database_can_force_a_fresh_draft_after_repeated_error().Logger#warning().
  test_solutions_database_can_force_a_fresh_draft_after_repeated_error.Logger.debug: test_solutions_database_can_force_a_fresh_draft_after_repeated_error().Logger#debug().
  test_solutions_database_can_force_a_fresh_draft_after_repeated_error.Node.__init__: test_solutions_database_can_force_a_fresh_draft_after_repeated_error().Node#__init__().
  test_naturebench_valid_final_score_requires_successful_node.Metric.__init__: test_naturebench_valid_final_score_requires_successful_node().Metric#__init__().
  test_generic_llm_converts_generation_kwargs_to_plain_containers.FakeClient.client_content_key: test_generic_llm_converts_generation_kwargs_to_plain_containers().FakeClient#client_content_key.
  test_generic_llm_converts_generation_kwargs_to_plain_containers.FakeClient.query: test_generic_llm_converts_generation_kwargs_to_plain_containers().FakeClient#query().
  test_naturebench_concurrent_attempts_keep_distinct_workspaces.ConcurrentTask._run_solution: test_naturebench_concurrent_attempts_keep_distinct_workspaces().ConcurrentTask#_run_solution().
  test_naturebench_concurrent_attempts_keep_distinct_workspaces.ConcurrentTask._post_evaluate: test_naturebench_concurrent_attempts_keep_distinct_workspaces().ConcurrentTask#_post_evaluate().
---
# Module: [`OpenMLE-Evo/tests/test_naturebench_integration.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py)

## Classes
### `CapturingTask`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:862`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L862)
- signature: `class CapturingTask(base_task.NatureBenchTask):`
- protocol/private: `_resolve_scm_task_root`[`L633`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L633), `_resolve_scm_task_root`[`L792`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L792), `_resolve_scm_task_root`[`L870`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L870), `_ssh`[`L636`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L636), `_ssh`[`L795`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L795), `_ssh`[`L873`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L873), `_sync_workspace_to_scm`[`L626`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L626), `_sync_workspace_to_scm`[`L785`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L785), `_sync_workspace_to_scm`[`L863`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L863)
- uses (calls/refs, reference-scoped): (3 test-only callers)
- used by: (1 test-only callers)

### `ConcurrentTask`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:1608`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1608)
- signature: `class ConcurrentTask(base_task.NatureBenchTask):`
- protocol/private: `_post_evaluate`[`L1626`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1626), `_run_solution`[`L1609`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1609)
- used by: (1 test-only callers)

### `CountingTask`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:563`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L563)
- signature: `class CountingTask(base_task.NatureBenchTask):`
- protocol/private: `_post_evaluate`[`L575`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L575), `_run_solution`[`L564`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L564)
- used by: (1 test-only callers)

### `FailedProcess`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:369`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L369)
- signature: `class FailedProcess:`
- members:
  - `returncode` — [`L370`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L370)
  - `stderr` — [`L372`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L372)
  - `stdout` — [`L371`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L371)

### `FakeClient`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:1528`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1528)
- signature: `class FakeClient:`
- members:
  - `query(self, messages, **kwargs)` — [`L1531`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1531) — python\nprint(1)\n
  - `client_content_key` — [`L1529`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1529)
- used by: (1 test-only callers)

### `FakeCompletedProcess`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:937`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L937)
- signature: `class FakeCompletedProcess:`
- members:
  - `returncode` — [`L621`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L621)
  - `returncode` — [`L780`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L780)
  - `returncode` — [`L858`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L858)
  - `returncode` — [`L939`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L939)
  - `stderr` — [`L623`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L623)
  - `stderr` — [`L782`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L782)
  - `stderr` — [`L860`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L860)
  - `stderr` — [`L941`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L941)
  - `stdout` — [`L622`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L622)
  - `stdout` — [`L781`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L781)
  - `stdout` — [`L859`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L859)
  - `stdout` — [`L940`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L940)
- protocol/private: `__init__`[`L938`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L938)
- used by: (1 test-only callers)

### `FakeNatureBenchTask`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:500`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L500)
- signature: `class FakeNatureBenchTask(base_task.NatureBenchTask):`
- protocol/private: `_post_evaluate`[`L444`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L444), `_post_evaluate`[`L511`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L511), `_run_solution`[`L433`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L433), `_run_solution`[`L501`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L501)
- used by: (1 test-only callers)

### `Journal`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:1136`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1136)
- signature: `class Journal:`
- members:
  - `is_root_node(self, node: Node)` — [`L1140`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1140)
  - `nodes` — [`L1138`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1138)
- protocol/private: `__init__`[`L1137`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1137)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `Logger`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:1202`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1202)
- signature: `class Logger:`
- members:
  - `debug(self, *args, **kwargs)` — [`L1209`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1209)
  - `info(self, *args, **kwargs)` — [`L1203`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1203)
  - `warning(self, *args, **kwargs)` — [`L1206`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1206)
- used by: (1 test-only callers)

### `Metric`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:1264`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1264)
- signature: `class Metric:`
- members:
  - `info` — [`L1127`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1127)
  - `value` — [`L1126`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1126)
- protocol/private: `__init__`[`L1125`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1125), `__init__`[`L1265`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1265)
- used by: (1 test-only callers)

### `Node`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:1268`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1268)
- signature: `class Node:`
- members:
  - `code` — [`L1133`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1133)
  - `id` — [`L1131`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1131)
  - `metric` — [`L1134`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1134)
  - `step` — [`L1132`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1132)
- protocol/private: `__init__`[`L1130`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1130), `__init__`[`L1213`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1213), `__init__`[`L1269`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1269)
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `RegisteringFakeNatureBenchTask`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:691`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L691)
- signature: `class RegisteringFakeNatureBenchTask(base_task.NatureBenchTask):`
- protocol/private: `_post_json`[`L702`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L702), `_run_solution`[`L692`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L692)
- used by: (1 test-only callers)

### `Solver`
- def: [`OpenMLE-Evo/tests/test_naturebench_integration.py:1143`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1143)
- signature: `class Solver:`
- members:
  - `journal` — [`L1145`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1145)
- protocol/private: `__init__`[`L1144`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1144)
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `_load_module(name: str, path: Path)` — [`L22`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L22)
- `_write_fake_naturebench_task(root: Path, task_name: str = "fake-nature-task")` — [`L31`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L31)
- `fake_run(command, **kwargs)` — [`L943`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L943)
- `fake_run(command, **kwargs)` — [`L1682`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1682)
- `run_candidate(index: int)` — [`L1652`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1652)
- `test_evaluate_naturebench_payloads_point_to_naturebench_builder_and_runner(tmp_path)` — [`L1368`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1368)
- `test_generic_llm_converts_generation_kwargs_to_plain_containers(monkeypatch, tmp_path)` — [`L1518`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1518)
- `test_naturebench_build_tasks_allows_zero_submit_repeats(tmp_path)` — [`L380`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L380)
- `test_naturebench_build_tasks_extracts_empirical_eda_addendum(tmp_path)` — [`L128`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L128)
- `test_naturebench_build_tasks_fails_when_scm_resource_lines_are_unreadable(tmp_path, monkeypatch)` — [`L338`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L338)
- `test_naturebench_build_tasks_uses_official_scm_resource_lines(tmp_path)` — [`L214`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L214)
- `test_naturebench_build_tasks_uses_task_set_resource_labels(tmp_path)` — [`L176`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L176)
- `test_naturebench_build_tasks_writes_airaevo_config(tmp_path)` — [`L74`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L74)
- `test_naturebench_concurrent_attempts_keep_distinct_workspaces(tmp_path)` — [`L1594`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1594)
- `test_naturebench_default_configs_skip_submit_and_reduce_search_artifacts()` — [`L1453`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1453)
- `test_naturebench_docker_timeout_forcibly_removes_named_container(monkeypatch, tmp_path)` — [`L1667`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1667)
- `test_naturebench_final_selection_ignores_failed_high_score_nodes()` — [`L1113`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1113)
- `test_naturebench_final_submit_is_disabled_by_default_and_uses_search_score()` — [`L1067`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1067)
- `test_naturebench_leaderboard_flags_use_official_thresholds()` — [`L1170`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1170)
- `test_naturebench_local_candidate_env_does_not_inherit_secrets(monkeypatch, tmp_path)` — [`L1754`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1754)
- `test_naturebench_operator_prompts_use_output_dir_not_submission_csv()` — [`L1314`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1314)
- `test_naturebench_operator_templates_accept_verified_visible_data_analysis()` — [`L1034`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1034)
- `test_naturebench_preflight_blocks_package_install_without_evaluation(tmp_path)` — [`L549`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L549)
- `test_naturebench_remote_tar_command_quotes_workspace_component()` — [`L1731`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1731)
- `test_naturebench_runner_uses_naturebench_task_and_prompt_paths()` — [`L984`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L984)
- `test_naturebench_scm_docker_uses_exclusive_gpu_pool_not_all_flag(tmp_path)` — [`L766`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L766)
- `test_naturebench_scm_docker_uses_shared_gpu_slot_pool(tmp_path)` — [`L844`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L844)
- `test_naturebench_scm_gpu_wait_is_reported_separately(monkeypatch, tmp_path)` — [`L609`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L609)
- `test_naturebench_scm_ssh_retries_transient_connection_close(monkeypatch, tmp_path)` — [`L921`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L921)
- `test_naturebench_skipped_submit_outputs_count_as_completed(tmp_path)` — [`L1285`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1285)
- `test_naturebench_summary_does_not_require_mle_leaderboard(tmp_path)` — [`L1481`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1481) — documented in [OpenMLE-Evo-tts_search-eval_utils](../../../concepts/OpenMLE-Evo-tts_search-eval_utils.md)
- `test_naturebench_task_clips_selection_fitness_but_preserves_raw_aggregate(tmp_path)` — [`L486`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L486)
- `test_naturebench_task_registers_eval_service_once_before_evaluation(tmp_path)` — [`L678`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L678)
- `test_naturebench_task_uses_current_aggregate_improvement_as_fitness(tmp_path)` — [`L416`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L416)
- `test_naturebench_valid_final_score_requires_successful_node()` — [`L1253`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1253)
- `test_runner_config_redaction_removes_nested_api_keys()` — [`L1793`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1793)
- `test_solutions_database_can_force_a_fresh_draft_after_repeated_error()` — [`L1199`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L1199)

## Module values
- `REPO_ROOT` — [`L17`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tests/test_naturebench_integration.py#L17)

