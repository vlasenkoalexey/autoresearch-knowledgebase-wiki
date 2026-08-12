---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.examples.mle_bench.base_task`/SandboxMLEBenchTask#
symbols:
  SandboxMLEBenchTask.evaluate_code: evaluate_code().
  SandboxMLEBenchTask.prepare: prepare().
  SandboxMLEBenchTask._run_eval_async: _run_eval_async().
  SandboxMLEBenchTask.cfg: cfg.
  SandboxMLEBenchTask.submit_data_dir: submit_data_dir.
  SandboxMLEBenchTask.build_submit_code: build_submit_code().
  SandboxMLEBenchTask.validation_time_used: validation_time_used.
  SandboxMLEBenchTask.step_task: step_task().
  SandboxMLEBenchTask.stop_requested: stop_requested.
  SandboxMLEBenchTask._build_task_description: _build_task_description().
  SandboxMLEBenchTask.validation_data_dir: validation_data_dir.
  SandboxMLEBenchTask.submit_data_dir_root: submit_data_dir_root.
  SandboxMLEBenchTask.evaluate_fitness: evaluate_fitness().
  SandboxMLEBenchTask.submit_dir: submit_dir.
  SandboxMLEBenchTask.raw_task_description: raw_task_description.
  SandboxMLEBenchTask.data_description: data_description.
  SandboxMLEBenchTask.validation_dir_name: validation_dir_name.
  SandboxMLEBenchTask.public_system_prompt: public_system_prompt.
  SandboxMLEBenchTask.public_user_prompt: public_user_prompt.
  SandboxMLEBenchTask.task_description: task_description.
  SandboxMLEBenchTask.lower_is_better: lower_is_better.
  SandboxMLEBenchTask: ''
  SandboxMLEBenchTask.time_budget: time_budget.
  SandboxMLEBenchTask._fake_sandbox_failure: _fake_sandbox_failure().
  SandboxMLEBenchTask._build_execution_result: _build_execution_result().
  SandboxMLEBenchTask.close: close().
  SandboxMLEBenchTask._next_fake_score: _next_fake_score().
  SandboxMLEBenchTask.__init__: __init__().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py)

## Classes
### `SandboxMLEBenchTask`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py:32`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L32)
- signature: `class SandboxMLEBenchTask(Task):`
- members:
  - `build_submit_code(self, code: str)` — [`L75`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L75)
  - `close(self, state: dict[str, Any])` — [`L313`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L313)
  - `evaluate_code(self, code: str, *, phase: str)` — [`L242`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L242)
  - `evaluate_fitness(self, solution: Any | None = None, state: dict[str, Any] | None = None, interpreter: Interpreter | None = None, aux_info: dict[str, Any] | None = None)` — [`L293`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L293)
  - `prepare(self, **task_args: Any)` — [`L80`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L80)
  - `step_task(self, state: dict[str, Any], action: Any)` — [`L276`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L276)
  - `cfg` — [`L40`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L40)
  - `data_description` — [`L62`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L62)
  - `lower_is_better` — [`L64`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L64)
  - `public_system_prompt` — [`L59`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L59)
  - `public_user_prompt` — [`L60`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L60)
  - `raw_task_description` — [`L61`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L61)
  - `stop_requested` — [`L46`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L46)
  - `submit_data_dir` — [`L52`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L52)
  - `submit_data_dir_root` — [`L43`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L43)
  - `submit_dir` — [`L42`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L42)
  - `task_description` — [`L63`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L63)
  - `time_budget` — [`L44`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L44)
  - `validation_data_dir` — [`L41`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L41)
  - `validation_dir_name` — [`L49`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L49)
  - `validation_time_used` — [`L45`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L45)
- protocol/private: `__init__`[`L33`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L33), `_build_execution_result`[`L262`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L262), `_build_task_description`[`L66`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L66), `_fake_sandbox_failure`[`L226`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L226), `_next_fake_score`[`L205`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L205), `_run_eval_async`[`L94`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/base_task.py#L94)
- uses (calls/refs, reference-scoped): [`score2reward`](../../../../tts_search/reward_func_utils.md#score2reward), [`get_sandbox_result`](../../../../tts_search/reward_func_utils.md#get_sandbox_result), [`format_sandbox_feedback`](../../../../tts_search/reward_func_utils.md#format_sandbox_feedback), [`get_clear_log`](../../../../tts_search/reward_func_utils.md#get_clear_log), [`acquire_sandbox_slot`](../../../../tts_search/airaevo_concurrency.md#acquire_sandbox_slot)
- used by: (5 test-only callers)

