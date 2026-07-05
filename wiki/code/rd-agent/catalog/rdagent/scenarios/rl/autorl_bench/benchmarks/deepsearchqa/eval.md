---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks.deepsearchqa.eval`/
symbols:
  DeepSearchQAEvaluator.run_eval: DeepSearchQAEvaluator#run_eval().
  DeepSearchQAEvaluator._get_search_function: DeepSearchQAEvaluator#_get_search_function().
  DeepSearchQAEvaluator._judge_answer: DeepSearchQAEvaluator#_judge_answer().
  DeepSearchQAEvaluator._react_loop: DeepSearchQAEvaluator#_react_loop().
  DeepSearchQAEvaluator.eval_config: DeepSearchQAEvaluator#eval_config.
  DeepSearchQAEvaluator: DeepSearchQAEvaluator#
  REACT_SYSTEM_PROMPT: REACT_SYSTEM_PROMPT.
  DeepSearchQAEvaluator.benchmark_id: DeepSearchQAEvaluator#benchmark_id.
  DeepSearchQAEvaluator._serpapi_search: DeepSearchQAEvaluator#_serpapi_search().
  DeepSearchQAEvaluator._duckduckgo_search: DeepSearchQAEvaluator#_duckduckgo_search().
  DeepSearchQAEvaluator._string_match: DeepSearchQAEvaluator#_string_match().
  DeepSearchQAEvaluator.__init__: DeepSearchQAEvaluator#__init__().
  DeepSearchQAEvaluator.config: DeepSearchQAEvaluator#config.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py)

## Classes
### `DeepSearchQAEvaluator`  ·  implements/extends BaseEvaluator
- def: [`rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py:49`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L49)
- doc: DeepSearchQA 评测器
- signature: `class DeepSearchQAEvaluator(BaseEvaluator):`
- members:
  - `_duckduckgo_search(self, query: str)` — [`L310`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L310) — DuckDuckGo 即时答案 API（免费，但结果较少）
  - `_get_search_function(self)` — [`L283`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L283) — 返回搜索函数，优先使用 SerpAPI，降级到 DuckDuckGo
  - `_react_loop(self, llm: LLM, sampling_params: SamplingParams, search_fn, question: str, answer_type: str)` — [`L185`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L185) — ReAct multi-step reasoning loop, return final answer string
  - `_serpapi_search(self, query: str, api_key: str)` — [`L296`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L296) — SerpAPI 搜索，返回摘要文本
  - `_string_match(self, predicted: str, gold: str, answer_type: str)` — [`L361`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L361) — fallback: simple string matching
  - `run_eval(self, model_path: str, workspace_path: str, **kwargs)` — [`L65`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L65)
  - `benchmark_id` — [`L62`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L62)
  - `config` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L61)
  - `eval_config` — [`L63`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L63)
- protocol/private: `__init__`[`L60`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L60), `_judge_answer`[`L329`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L329)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../../../oai/llm_utils.md#APIBackend), [`warning`](../../../../../log/logger.md#RDAgentLog.warning), [`build_messages_and_create_chat_completion`](../../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`get_default_result`](../../core/evaluator.md#BaseEvaluator.get_default_result), [`validate_model`](../../core/evaluator.md#BaseEvaluator.validate_model)  (7 test-only)
- used by: [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`run_eval`](../../core/evaluator.md#BaseEvaluator.run_eval)

## Module values
- `REACT_SYSTEM_PROMPT` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/eval.py#L32)

