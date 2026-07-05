---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks.smith.per_sample_eval`/
symbols:
  PerSampleEvaluator.run_eval: PerSampleEvaluator#run_eval().
  _cleanup_vllm: _cleanup_vllm().
  PerSampleEvaluator.benchmark_id: PerSampleEvaluator#benchmark_id.
  PerSampleEvaluator: PerSampleEvaluator#
  PerSampleEvaluator.eval_config: PerSampleEvaluator#eval_config.
  _cleanup_vllm._gpu_cleanup: _cleanup_vllm()._gpu_cleanup().
  _apply_range: _apply_range().
  PerSampleEvaluator.__init__: PerSampleEvaluator#__init__().
  PerSampleEvaluator.config: PerSampleEvaluator#config.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py)

## Classes
### `PerSampleEvaluator`  ·  implements/extends BaseEvaluator
- def: [`rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py:19`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L19)
- doc: Evaluator that scores each sample individually using benchmark-specific eval.py.
- signature: `class PerSampleEvaluator(BaseEvaluator):`
- members:
  - `run_eval(self, model_path: str, workspace_path: str, model_name: str = "", gpu_count: int = 1, test_range: str = "[:]", **kwargs)` — [`L27`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L27)
  - `benchmark_id` — [`L24`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L24)
  - `config` — [`L23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L23)
  - `eval_config` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L25)
- protocol/private: `__init__`[`L22`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L22)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`warning`](../../../../../log/logger.md#RDAgentLog.warning), [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`get_default_result`](../../core/evaluator.md#BaseEvaluator.get_default_result), [`validate_model`](../../core/evaluator.md#BaseEvaluator.validate_model)  (2 test-only)
- used by: [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`run_eval`](../../core/evaluator.md#BaseEvaluator.run_eval)

## Functions
- `_apply_range(data: list, test_range: str)` — [`L179`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L179) — Apply a Python-style slice string like '[:]' or '[:100]' to a list.
- `_cleanup_vllm(llm)` — [`L143`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L143) — Release vLLM GPU memory without initializing CUDA in the main process.
- `_gpu_cleanup()` — [`L153`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/smith/per_sample_eval.py#L153)

