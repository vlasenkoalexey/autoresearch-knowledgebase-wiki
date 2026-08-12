---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.examples.nature_bench.base_task`/
symbols:
  NatureBenchTask.cfg: NatureBenchTask#cfg.
  NatureBenchTask._run_scm_docker_solution: NatureBenchTask#_run_scm_docker_solution().
  NatureBenchTask._start_attempt: NatureBenchTask#_start_attempt().
  NatureBenchTask._ensure_eval_service_registered: NatureBenchTask#_ensure_eval_service_registered().
  NatureBenchTask.prepare: NatureBenchTask#prepare().
  NatureBenchTask.evaluate_code: NatureBenchTask#evaluate_code().
  NatureBenchTask._run_solution: NatureBenchTask#_run_solution().
  NatureBenchTask._run_docker_solution: NatureBenchTask#_run_docker_solution().
  NatureBenchTask._candidate_preflight: NatureBenchTask#_candidate_preflight().
  NatureBenchTask._eval_service_out_dir_value: NatureBenchTask#_eval_service_out_dir_value().
  NatureBenchTask.scm_task_roots: NatureBenchTask#scm_task_roots.
  NatureBenchTask._run_scm_import_preflight: NatureBenchTask#_run_scm_import_preflight().
  NatureBenchTask._record_validation_timing: NatureBenchTask#_record_validation_timing().
  NatureBenchTask._safe_path_component: NatureBenchTask#_safe_path_component().
  NatureBenchTask.task_name: NatureBenchTask#task_name.
  NatureBenchTask._resolve_scm_task_root: NatureBenchTask#_resolve_scm_task_root().
  NatureBenchTask._eval_service_out_dir: NatureBenchTask#_eval_service_out_dir().
  NatureBenchTask._sync_workspace_to_scm: NatureBenchTask#_sync_workspace_to_scm().
  NatureBenchTask._scm_gpu_setup_and_docker_args: NatureBenchTask#_scm_gpu_setup_and_docker_args().
  NatureBenchTask._start_eval_service_timer: NatureBenchTask#_start_eval_service_timer().
  NatureBenchTask._post_evaluate: NatureBenchTask#_post_evaluate().
  NatureBenchTask._ssh: NatureBenchTask#_ssh().
  NatureBenchTask._coerce_score: NatureBenchTask#_coerce_score().
  NatureBenchTask.batch_name: NatureBenchTask#batch_name.
  NatureBenchTask._build_task_description: NatureBenchTask#_build_task_description().
  NatureBenchTask._solution_env: NatureBenchTask#_solution_env().
  NatureBenchTask._exclusive_gpu_acquire_script: NatureBenchTask#_exclusive_gpu_acquire_script().
  NatureBenchTask._shared_gpu_acquire_script: NatureBenchTask#_shared_gpu_acquire_script().
  NatureBenchTask._uses_scm: NatureBenchTask#_uses_scm().
  NatureBenchTask._post_json: NatureBenchTask#_post_json().
  NatureBenchTask._run_ssh_with_retries: NatureBenchTask#_run_ssh_with_retries().
  NatureBenchTask._gpu_lock_root: NatureBenchTask#_gpu_lock_root().
  NatureBenchTask._solve_timeout_seconds: NatureBenchTask#_solve_timeout_seconds().
  NatureBenchTask._remote_json_request: NatureBenchTask#_remote_json_request().
  NatureBenchTask._annotate_eval_payload: NatureBenchTask#_annotate_eval_payload().
  NatureBenchTask._execution_timeout_seconds: NatureBenchTask#_execution_timeout_seconds().
  NatureBenchTask.scm_host: NatureBenchTask#scm_host.
  NatureBenchTask._workspace_root: NatureBenchTask#_workspace_root().
  NatureBenchTask._scm_gpu_wait_timeout_seconds: NatureBenchTask#_scm_gpu_wait_timeout_seconds().
  NatureBenchTask.eval_service_url: NatureBenchTask#eval_service_url.
  NatureBenchTask._scm_task_root_cache: NatureBenchTask#_scm_task_root_cache.
  NatureBenchTask._selection_score_from_aggregate: NatureBenchTask#_selection_score_from_aggregate().
  NatureBenchTask._candidate_preflight_imports_enabled: NatureBenchTask#_candidate_preflight_imports_enabled().
  NatureBenchTask._candidate_preflight_timeout_seconds: NatureBenchTask#_candidate_preflight_timeout_seconds().
  NatureBenchTask._scm_docker_command_timeout_seconds: NatureBenchTask#_scm_docker_command_timeout_seconds().
  NatureBenchTask._container_eval_service_url: NatureBenchTask#_container_eval_service_url().
  NatureBenchTask._run_local_solution: NatureBenchTask#_run_local_solution().
  NatureBenchTask._gpu_skip_busy_limits: NatureBenchTask#_gpu_skip_busy_limits().
  NatureBenchTask._extract_gpu_wait_seconds: NatureBenchTask#_extract_gpu_wait_seconds().
  _shell_join: _shell_join().
  NatureBenchTask.scm_workspace_root: NatureBenchTask#scm_workspace_root.
  NatureBenchTask.get_budget_exempt_wait_seconds: NatureBenchTask#get_budget_exempt_wait_seconds().
  NatureBenchTask.step_task: NatureBenchTask#step_task().
  NatureBenchTask.evaluate_fitness: NatureBenchTask#evaluate_fitness().
  NatureBenchTask.validation_data_dir: NatureBenchTask#validation_data_dir.
  NatureBenchTask.task_dir: NatureBenchTask#task_dir.
  NatureBenchTask.execution_mode: NatureBenchTask#execution_mode.
  NatureBenchTask.raw_task_description: NatureBenchTask#raw_task_description.
  NatureBenchTask.data_description: NatureBenchTask#data_description.
  NatureBenchTask.visible_data_analysis: NatureBenchTask#visible_data_analysis.
  NatureBenchTask.task_family_guidance: NatureBenchTask#task_family_guidance.
  NatureBenchTask._gpu_external_busy_probe_script: NatureBenchTask#_gpu_external_busy_probe_script().
  _AttemptContext: _AttemptContext#
  _AttemptContext.index: _AttemptContext#index.
  _AttemptContext.workspace: _AttemptContext#workspace.
  _AttemptContext.output_dir: _AttemptContext#output_dir.
  NatureBenchTask.validation_time_used: NatureBenchTask#validation_time_used.
  NatureBenchTask.validation_gpu_wait_time: NatureBenchTask#validation_gpu_wait_time.
  NatureBenchTask._import_preflight_cache: NatureBenchTask#_import_preflight_cache.
  NatureBenchTask.problem_dir: NatureBenchTask#problem_dir.
  NatureBenchTask.scm_eval_service_url: NatureBenchTask#scm_eval_service_url.
  NatureBenchTask.scm_container_eval_service_url: NatureBenchTask#scm_container_eval_service_url.
  NatureBenchTask.public_system_prompt: NatureBenchTask#public_system_prompt.
  NatureBenchTask.public_user_prompt: NatureBenchTask#public_user_prompt.
  NatureBenchTask.task_description: NatureBenchTask#task_description.
  NatureBenchTask.lower_is_better: NatureBenchTask#lower_is_better.
  NatureBenchTask.eval_timeout: NatureBenchTask#eval_timeout.
  NatureBenchTask._candidate_preflight_enabled: NatureBenchTask#_candidate_preflight_enabled().
  NatureBenchTask._ssh_retry_attempts: NatureBenchTask#_ssh_retry_attempts().
  NatureBenchTask._ssh_retry_delay: NatureBenchTask#_ssh_retry_delay().
  NatureBenchTask._remote_tar_extract_command: NatureBenchTask#_remote_tar_extract_command().
  _IMPORT_PREFLIGHT_MARKER: _IMPORT_PREFLIGHT_MARKER.
  NatureBenchTask.time_budget: NatureBenchTask#time_budget.
  NatureBenchTask._state_lock: NatureBenchTask#_state_lock.
  NatureBenchTask.attempt_index: NatureBenchTask#attempt_index.
  NatureBenchTask._preflight_failure: NatureBenchTask#_preflight_failure().
  NatureBenchTask.submit_data_dir: NatureBenchTask#submit_data_dir.
  _RawShell: _RawShell#
  _GPU_WAIT_MARKER_RE: _GPU_WAIT_MARKER_RE.
  _GPU_WAIT_TIMEOUT_MARKER: _GPU_WAIT_TIMEOUT_MARKER.
  _AttemptContext.scm_workspace: _AttemptContext#scm_workspace.
  NatureBenchTask._eval_service_lock: NatureBenchTask#_eval_service_lock.
  NatureBenchTask.validation_preflight_time_used: NatureBenchTask#validation_preflight_time_used.
  NatureBenchTask._eval_service_registered: NatureBenchTask#_eval_service_registered.
  NatureBenchTask._eval_service_timer_started: NatureBenchTask#_eval_service_timer_started.
  NatureBenchTask._timeout_stream_text: NatureBenchTask#_timeout_stream_text().
  NatureBenchTask._ssh_options: NatureBenchTask#_ssh_options().
  NatureBenchTask._build_execution_result: NatureBenchTask#_build_execution_result().
  _CANDIDATE_ENV_ALLOWLIST: _CANDIDATE_ENV_ALLOWLIST.
  _AttemptContext.phase: _AttemptContext#phase.
  NatureBenchTask.stop_requested: NatureBenchTask#stop_requested.
  NatureBenchTask._candidate_import_roots: NatureBenchTask#_candidate_import_roots().
  NatureBenchTask._contains_package_install: NatureBenchTask#_contains_package_install().
  NatureBenchTask._normalize_scm_task_roots: NatureBenchTask#_normalize_scm_task_roots().
  NatureBenchTask._is_transient_ssh_failure: NatureBenchTask#_is_transient_ssh_failure().
  NatureBenchTask._normalize_gpu_devices: NatureBenchTask#_normalize_gpu_devices().
  NatureBenchTask._wrap_scm_docker_command: NatureBenchTask#_wrap_scm_docker_command().
  NatureBenchTask._preflight_failure_payload: NatureBenchTask#_preflight_failure_payload().
  NatureBenchTask: NatureBenchTask#
  NatureBenchTask.__init__: NatureBenchTask#__init__().
  NatureBenchTask.evaluation_protocol: NatureBenchTask#evaluation_protocol.
  NatureBenchTask.submit_repeats: NatureBenchTask#submit_repeats.
  NatureBenchTask.build_submit_code: NatureBenchTask#build_submit_code().
  NatureBenchTask.close: NatureBenchTask#close().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py)

## Classes
### `NatureBenchTask`
- def: [`OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py:75`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L75)
- signature: `class NatureBenchTask(Task):`
- members:
  - `build_submit_code(self, code: str)` — [`L401`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L401)
  - `close(self, state: dict[str, Any])` — [`L1563`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1563)
  - `evaluate_code(self, code: str, *, phase: str)` — [`L1464`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1464)
  - `evaluate_fitness(self, solution: Any | None = None, state: dict[str, Any] | None = None, interpreter: Interpreter | None = None, aux_info: dict[str, Any] | None = None)` — [`L1544`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1544)
  - `get_budget_exempt_wait_seconds(self)` — [`L166`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L166) — Return scheduler delay that should not consume the NatureBench search budget.
  - `prepare(self, **task_args: Any)` — [`L383`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L383)
  - `step_task(self, state: dict[str, Any], action: Any)` — [`L1519`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1519)
  - `attempt_index` — [`L142`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L142)
  - `batch_name` — [`L119`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L119)
  - `cfg` — [`L83`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L83)
  - `data_description` — [`L123`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L123)
  - `eval_service_url` — [`L91`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L91)
  - `eval_timeout` — [`L134`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L134)
  - `evaluation_protocol` — [`L89`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L89)
  - `execution_mode` — [`L90`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L90)
  - `lower_is_better` — [`L131`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L131)
  - `problem_dir` — [`L87`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L87)
  - `public_system_prompt` — [`L120`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L120)
  - `public_user_prompt` — [`L121`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L121)
  - `raw_task_description` — [`L122`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L122)
  - `scm_container_eval_service_url` — [`L97`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L97)
  - `scm_eval_service_url` — [`L94`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L94)
  - `scm_host` — [`L92`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L92)
  - `scm_task_roots` — [`L101`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L101)
  - `scm_workspace_root` — [`L93`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L93)
  - `stop_requested` — [`L141`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L141)
  - `submit_data_dir` — [`L86`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L86)
  - `submit_repeats` — [`L133`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L133)
  - `task_description` — [`L130`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L130)
  - `task_dir` — [`L88`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L88)
  - `task_family_guidance` — [`L127`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L127)
  - `task_name` — [`L84`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L84)
  - `time_budget` — [`L135`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L135)
  - `validation_data_dir` — [`L85`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L85)
  - `validation_gpu_wait_time` — [`L139`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L139)
  - `validation_preflight_time_used` — [`L140`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L140)
  - `validation_time_used` — [`L138`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L138)
  - `visible_data_analysis` — [`L124`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L124)
- protocol/private: `__init__`[`L76`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L76), `_annotate_eval_payload`[`L1347`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1347), `_build_execution_result`[`L1501`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1501), `_build_task_description`[`L366`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L366), `_candidate_import_roots`[`L182`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L182), `_candidate_preflight`[`L316`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L316), `_candidate_preflight_enabled`[`L171`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L171), `_candidate_preflight_imports_enabled`[`L174`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L174), `_candidate_preflight_timeout_seconds`[`L177`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L177), `_coerce_score`[`L149`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L149), `_container_eval_service_url`[`L554`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L554), `_contains_package_install`[`L199`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L199), `_ensure_eval_service_registered`[`L1301`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1301), `_eval_service_lock`[`L137`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L137), `_eval_service_out_dir`[`L433`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L433), `_eval_service_out_dir_value`[`L444`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L444), `_eval_service_registered`[`L143`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L143), `_eval_service_timer_started`[`L144`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L144), `_exclusive_gpu_acquire_script`[`L970`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L970), `_execution_timeout_seconds`[`L472`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L472), `_extract_gpu_wait_seconds`[`L1142`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1142), `_gpu_external_busy_probe_script`[`L943`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L943), `_gpu_lock_root`[`L928`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L928), `_gpu_skip_busy_limits`[`L935`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L935), `_import_preflight_cache`[`L146`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L146), `_is_transient_ssh_failure`[`L751`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L751), `_normalize_gpu_devices`[`L917`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L917), `_normalize_scm_task_roots`[`L421`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L421), `_post_evaluate`[`L1338`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1338), `_post_json`[`L1276`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1276), `_preflight_failure`[`L219`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L219), `_preflight_failure_payload`[`L1409`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1409), `_record_validation_timing`[`L1431`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1431), `_remote_json_request`[`L794`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L794), `_remote_tar_extract_command`[`L889`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L889), `_resolve_scm_task_root`[`L851`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L851), `_run_docker_solution`[`L618`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L618), `_run_local_solution`[`L574`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L574), `_run_scm_docker_solution`[`L1156`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1156), `_run_scm_import_preflight`[`L232`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L232), `_run_solution`[`L1256`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1256), `_run_ssh_with_retries`[`L766`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L766), `_safe_path_component`[`L411`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L411), `_scm_docker_command_timeout_seconds`[`L482`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L482), `_scm_gpu_setup_and_docker_args`[`L1071`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1071), `_scm_gpu_wait_timeout_seconds`[`L491`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L491), `_scm_task_root_cache`[`L145`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L145), `_selection_score_from_aggregate`[`L158`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L158), `_shared_gpu_acquire_script`[`L1011`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1011), `_solution_env`[`L526`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L526), `_solve_timeout_seconds`[`L459`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L459), `_ssh`[`L717`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L717), `_ssh_options`[`L731`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L731), `_ssh_retry_attempts`[`L743`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L743), `_ssh_retry_delay`[`L746`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L746), `_start_attempt`[`L495`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L495), `_start_eval_service_timer`[`L1327`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1327), `_state_lock`[`L136`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L136), `_sync_workspace_to_scm`[`L892`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L892), `_timeout_stream_text`[`L611`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L611), `_uses_scm`[`L430`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L430), `_workspace_root`[`L404`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L404), `_wrap_scm_docker_command`[`L1102`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L1102)
- uses (calls/refs, reference-scoped): (12 test-only callers)

### `_AttemptContext`  ·  implements/extends NamedTuple
- def: [`OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py:67`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L67)
- signature: `class _AttemptContext(NamedTuple):`
- members:
  - `index` — [`L68`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L68)
  - `output_dir` — [`L71`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L71)
  - `phase` — [`L69`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L69)
  - `scm_workspace` — [`L72`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L72)
  - `workspace` — [`L70`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L70)
- used by: (4 test-only callers)

### `_RawShell`  ·  implements/extends str
- def: [`OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py:34`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L34)
- signature: `class _RawShell(str):`
- used by: (2 test-only callers)

## Functions
- `_shell_join(parts: list[Any])` — [`L38`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L38)

## Module values
- `_CANDIDATE_ENV_ALLOWLIST` — [`L50`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L50)
- `_GPU_WAIT_MARKER_RE` — [`L45`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L45)
- `_GPU_WAIT_TIMEOUT_MARKER` — [`L48`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L48)
- `_IMPORT_PREFLIGHT_MARKER` — [`L49`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/nature_bench/base_task.py#L49)

