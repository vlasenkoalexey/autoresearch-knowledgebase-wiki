---
title: 'Module: rdagent/scenarios/rl/autorl_bench/core/evaluator.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/core/evaluator.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.core.evaluator`/
symbols:
  BaseEvaluator: BaseEvaluator#
  BaseEvaluator.run_eval: BaseEvaluator#run_eval().
  BaseEvaluator.get_default_result: BaseEvaluator#get_default_result().
  validate_eval_result: validate_eval_result().
  BaseEvaluator.validate_model: BaseEvaluator#validate_model().
  EvalResult: EvalResult#
  EvalResult.benchmark: EvalResult#benchmark.
  EvalResult.model_path: EvalResult#model_path.
  EvalResult.score: EvalResult#score.
  EvalResult.accuracy_summary: EvalResult#accuracy_summary.
  EvalResult.eval_type: EvalResult#eval_type.
  EvalResult.error: EvalResult#error.
  EvalResult.raw_output: EvalResult#raw_output.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/core/evaluator.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py)

## Classes
### `BaseEvaluator`  ·  implements/extends ABC
- def: [`rdagent/scenarios/rl/autorl_bench/core/evaluator.py:54`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L54)
- doc: Benchmark 评测器基类
- signature: `class BaseEvaluator(ABC):`
- members:
  - `get_default_result(self, benchmark_name: str, model_path: str)` — [`L145`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L145) — 返回默认的结果结构
  - `run_eval(self, model_path: str, workspace_path: str, model_name: str = "", gpu_count: int = 1, test_range: str = "[:]", **kwargs)` — [`L116`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L116) — 执行评测
  - `validate_model(self, model_path: str)` — [`L141`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L141) — 验证模型路径是否有效
- uses (calls/refs, reference-scoped): [`run_eval`](opencompass.md#OpenCompassEvaluator.run_eval), [`OpenCompassEvaluator`](opencompass.md#OpenCompassEvaluator), [`EvalResult`](evaluator.md#EvalResult)  (10 test-only)
- used by: [`submit`](server.md#GradingServer.submit), [`run_eval`](opencompass.md#OpenCompassEvaluator.run_eval), [`get_baseline_score`](utils.md#get_baseline_score), [`OpenCompassEvaluator`](opencompass.md#OpenCompassEvaluator)  (11 test-only)

### `EvalResult`  ·  implements/extends _TypedDict
- def: [`rdagent/scenarios/rl/autorl_bench/core/evaluator.py:21`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L21)
- doc: 评测输出结果
- signature: `class EvalResult(TypedDict):`
- members:
  - `accuracy_summary` — [`L41`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L41)
  - `benchmark` — [`L38`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L38)
  - `error` — [`L45`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L45)
  - `eval_type` — [`L44`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L44)
  - `model_path` — [`L39`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L39)
  - `raw_output` — [`L46`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L46)
  - `score` — [`L40`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L40)
- used by: [`run_eval`](evaluator.md#BaseEvaluator.run_eval), [`get_default_result`](evaluator.md#BaseEvaluator.get_default_result)

## Functions
- `validate_eval_result(result: Dict[str, Any])` — [`L155`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/evaluator.py#L155) — Return whether an evaluator result represents a completed evaluation.

