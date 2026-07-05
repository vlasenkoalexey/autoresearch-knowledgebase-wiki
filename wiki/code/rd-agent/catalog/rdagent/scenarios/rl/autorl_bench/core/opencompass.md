---
title: 'Module: rdagent/scenarios/rl/autorl_bench/core/opencompass.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/core/opencompass.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.core.opencompass`/OpenCompassEvaluator#
symbols:
  OpenCompassEvaluator.run_eval: run_eval().
  OpenCompassEvaluator: ''
  OpenCompassEvaluator._parse_results: _parse_results().
  OpenCompassEvaluator.benchmark_id: benchmark_id.
  OpenCompassEvaluator._get_model_inference_config: _get_model_inference_config().
  OpenCompassEvaluator.eval_config: eval_config.
  OpenCompassEvaluator.__init__: __init__().
  OpenCompassEvaluator.config: config.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/core/opencompass.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py)

## Classes
### `OpenCompassEvaluator`  ·  implements/extends BaseEvaluator
- def: [`rdagent/scenarios/rl/autorl_bench/core/opencompass.py:22`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py#L22)
- doc: OpenCompass 通用评测器
- signature: `class OpenCompassEvaluator(BaseEvaluator):`
- members:
  - `_get_model_inference_config(self, model_name: str, gpu_count: int)` — [`L131`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py#L131) — 从 models.yaml 加载模型推理配置
  - `_parse_results(self, work_dir: Path, result: dict)` — [`L160`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py#L160) — 解析 OpenCompass 输出结果
  - `run_eval(self, model_path: str, workspace_path: str, model_name: str = "", gpu_count: int = 1, test_range: str = "[:]", **kwargs)` — [`L34`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py#L34) — 使用 OpenCompass 评测
  - `benchmark_id` — [`L31`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py#L31)
  - `config` — [`L30`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py#L30)
  - `eval_config` — [`L32`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py#L32)
- protocol/private: `__init__`[`L29`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/opencompass.py#L29)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../log/logger.md#RDAgentLog.info), [`warning`](../../../../log/logger.md#RDAgentLog.warning), [`BaseEvaluator`](evaluator.md#BaseEvaluator), [`get_default_result`](evaluator.md#BaseEvaluator.get_default_result), [`validate_model`](evaluator.md#BaseEvaluator.validate_model)  (2 test-only)
- used by: [`BaseEvaluator`](evaluator.md#BaseEvaluator), [`run_eval`](evaluator.md#BaseEvaluator.run_eval)  (2 test-only)

