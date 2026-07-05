---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks.alpacaeval.eval`/
symbols:
  AlpacaEvalEvaluator.run_eval: AlpacaEvalEvaluator#run_eval().
  AlpacaEvalEvaluator._generate_model_outputs: AlpacaEvalEvaluator#_generate_model_outputs().
  AlpacaEvalEvaluator.eval_config: AlpacaEvalEvaluator#eval_config.
  AlpacaEvalEvaluator: AlpacaEvalEvaluator#
  DEFAULT_REFERENCE_FILE: DEFAULT_REFERENCE_FILE.
  DEFAULT_ANNOTATORS_CONFIG: DEFAULT_ANNOTATORS_CONFIG.
  AlpacaEvalEvaluator.benchmark_id: AlpacaEvalEvaluator#benchmark_id.
  AlpacaEvalEvaluator._load_reference_outputs: AlpacaEvalEvaluator#_load_reference_outputs().
  AlpacaEvalEvaluator._format_prompt: AlpacaEvalEvaluator#_format_prompt().
  AlpacaEvalEvaluator._extract_score: AlpacaEvalEvaluator#_extract_score().
  AlpacaEvalEvaluator.__init__: AlpacaEvalEvaluator#__init__().
  AlpacaEvalEvaluator.config: AlpacaEvalEvaluator#config.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py)

## Classes
### `AlpacaEvalEvaluator`  ·  implements/extends BaseEvaluator
- def: [`rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py:23`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L23)
- doc: AlpacaEval 2.0 评测器（LLM Judge）
- signature: `class AlpacaEvalEvaluator(BaseEvaluator):`
- members:
  - `run_eval(self, model_path: str, workspace_path: str, model_name: str = "", gpu_count: int = 1, test_range: str = "[:]", **kwargs)` — [`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L31)
  - `benchmark_id` — [`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L28)
  - `config` — [`L27`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L27)
  - `eval_config` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L29)
- protocol/private: `__init__`[`L26`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L26), `_extract_score`[`L181`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L181), `_format_prompt`[`L123`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L123), `_generate_model_outputs`[`L132`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L132), `_load_reference_outputs`[`L112`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L112)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`warning`](../../../../../log/logger.md#RDAgentLog.warning), [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`get_default_result`](../../core/evaluator.md#BaseEvaluator.get_default_result), [`validate_model`](../../core/evaluator.md#BaseEvaluator.validate_model)  (2 test-only)
- used by: [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`run_eval`](../../core/evaluator.md#BaseEvaluator.run_eval)

## Module values
- `DEFAULT_ANNOTATORS_CONFIG` — [`L20`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L20)
- `DEFAULT_REFERENCE_FILE` — [`L19`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alpacaeval/eval.py#L19)

