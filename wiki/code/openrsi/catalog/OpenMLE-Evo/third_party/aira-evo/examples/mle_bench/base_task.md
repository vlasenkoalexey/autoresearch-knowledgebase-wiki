---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.examples.mle_bench.base_task`/SandboxMLEBenchTask#
symbols:
  SandboxMLEBenchTask.evaluate_code_async: evaluate_code_async().
  SandboxMLEBenchTask.evaluate_code: evaluate_code().
  SandboxMLEBenchTask.cfg: cfg.
  SandboxMLEBenchTask._run_eval_async: _run_eval_async().
  SandboxMLEBenchTask.prepare: prepare().
  SandboxMLEBenchTask.test_eval_split: test_eval_split.
  SandboxMLEBenchTask._annotate_eval_scores: _annotate_eval_scores().
  SandboxMLEBenchTask.submit_data_dir: submit_data_dir.
  SandboxMLEBenchTask.validation_time_used: validation_time_used.
  SandboxMLEBenchTask.build_submit_code: build_submit_code().
  SandboxMLEBenchTask._coerce_score: _coerce_score().
  SandboxMLEBenchTask.step_task: step_task().
  SandboxMLEBenchTask.step_task_async: step_task_async().
  SandboxMLEBenchTask.evaluation_protocol: evaluation_protocol.
  SandboxMLEBenchTask._score_to_reward: _score_to_reward().
  SandboxMLEBenchTask._score_protocol: _score_protocol().
  SandboxMLEBenchTask.validation_eval_split: validation_eval_split.
  SandboxMLEBenchTask.evaluate_fitness: evaluate_fitness().
  SandboxMLEBenchTask._eval_split_for_phase: _eval_split_for_phase().
  SandboxMLEBenchTask.validation_data_dir: validation_data_dir.
  SandboxMLEBenchTask._build_task_description: _build_task_description().
  SandboxMLEBenchTask.submit_data_dir_root: submit_data_dir_root.
  SandboxMLEBenchTask.submit_repeats: submit_repeats.
  SandboxMLEBenchTask.submit_dir: submit_dir.
  SandboxMLEBenchTask.raw_task_description: raw_task_description.
  SandboxMLEBenchTask.data_description: data_description.
  SandboxMLEBenchTask.submit_job_timeout: submit_job_timeout.
  SandboxMLEBenchTask.submit_wait_timeout: submit_wait_timeout.
  SandboxMLEBenchTask.time_budget: time_budget.
  SandboxMLEBenchTask._validation_time_lock: _validation_time_lock.
  SandboxMLEBenchTask.validation_dir_name: validation_dir_name.
  SandboxMLEBenchTask.public_system_prompt: public_system_prompt.
  SandboxMLEBenchTask.public_user_prompt: public_user_prompt.
  SandboxMLEBenchTask.task_description: task_description.
  SandboxMLEBenchTask.lower_is_better: lower_is_better.
  SandboxMLEBenchTask.use_clear_run_log_score: use_clear_run_log_score.
  SandboxMLEBenchTask.stop_requested: stop_requested.
  SandboxMLEBenchTask._build_execution_result: _build_execution_result().
  SandboxMLEBenchTask: ''
  SandboxMLEBenchTask._normalize_eval_split: _normalize_eval_split().
  SandboxMLEBenchTask.close: close().
  SandboxMLEBenchTask.__init__: __init__().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py)

## Classes
### `SandboxMLEBenchTask`
- def: [`OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py:34`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L34)
- signature: `class SandboxMLEBenchTask(Task):`
- members:
  - `build_submit_code(self, code: str)` — [`L113`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L113)
  - `close(self, state: dict[str, Any])` — [`L584`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L584)
  - `evaluate_code(self, code: str, *, phase: str)` — [`L400`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L400)
  - `evaluate_code_async(self, code: str, *, phase: str, sandbox_base_url: str | None = None)` — [`L439`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L439)
  - `evaluate_fitness(self, solution: Any | None = None, state: dict[str, Any] | None = None, interpreter: Interpreter | None = None, aux_info: dict[str, Any] | None = None)` — [`L554`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L554)
  - `prepare(self, **task_args: Any)` — [`L274`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L274)
  - `step_task(self, state: dict[str, Any], action: Any)` — [`L498`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L498)
  - `step_task_async(self, state: dict[str, Any], action: Any, *, sandbox_base_url: str | None = None)` — [`L523`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L523)
  - `cfg` — [`L42`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L42)
  - `data_description` — [`L75`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L75)
  - `evaluation_protocol` — [`L46`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L46)
  - `lower_is_better` — [`L77`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L77)
  - `public_system_prompt` — [`L72`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L72)
  - `public_user_prompt` — [`L73`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L73)
  - `raw_task_description` — [`L74`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L74)
  - `stop_requested` — [`L58`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L58)
  - `submit_data_dir` — [`L65`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L65)
  - `submit_data_dir_root` — [`L45`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L45)
  - `submit_dir` — [`L44`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L44)
  - `submit_job_timeout` — [`L81`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L81)
  - `submit_repeats` — [`L83`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L83)
  - `submit_wait_timeout` — [`L82`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L82)
  - `task_description` — [`L76`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L76)
  - `test_eval_split` — [`L52`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L52)
  - `time_budget` — [`L56`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L56)
  - `use_clear_run_log_score` — [`L78`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L78)
  - `validation_data_dir` — [`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L43)
  - `validation_dir_name` — [`L62`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L62)
  - `validation_eval_split` — [`L49`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L49)
  - `validation_time_used` — [`L57`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L57)
- protocol/private: `__init__`[`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L35), `_annotate_eval_scores`[`L139`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L139), `_build_execution_result`[`L484`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L484), `_build_task_description`[`L102`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L102), `_coerce_score`[`L93`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L93), `_eval_split_for_phase`[`L288`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L288), `_normalize_eval_split`[`L86`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L86), `_run_eval_async`[`L291`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L291), `_score_protocol`[`L128`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L128), `_score_to_reward`[`L118`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L118), `_validation_time_lock`[`L59`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/base_task.py#L59)
- uses (calls/refs, reference-scoped): [`score2reward`](../../../../tts_search/reward_func_utils.md#score2reward), [`get_sandbox_result`](../../../../tts_search/reward_func_utils.md#get_sandbox_result), [`acquire_sandbox_slot_async`](../../../../tts_search/airaevo_concurrency.md#acquire_sandbox_slot_async), [`acquire_sandbox_slot`](../../../../tts_search/airaevo_concurrency.md#acquire_sandbox_slot), [`format_sandbox_feedback`](../../../../tts_search/reward_func_utils.md#format_sandbox_feedback), [`API_KEY`](../../../../tts_search/reward_func_utils.md#API_KEY), [`get_clear_log`](../../../../tts_search/reward_func_utils.md#get_clear_log), [`parse_final_validation_score`](../../../../tts_search/reward_func_utils.md#parse_final_validation_score)
- used by: (4 test-only callers)

