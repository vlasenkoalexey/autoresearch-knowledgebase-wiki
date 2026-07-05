---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks.webshop.eval`/
symbols:
  WebShopEvaluator.run_eval: WebShopEvaluator#run_eval().
  _log: _log().
  create_llm_fn: create_llm_fn().
  webshop_run: webshop_run().
  _Tee.write: _Tee#write().
  _Tee.flush: _Tee#flush().
  create_llm_fn.cleanup: create_llm_fn().cleanup().
  WebShopEvaluator: WebShopEvaluator#
  _Tee.terminal: _Tee#terminal.
  _Tee.log: _Tee#log.
  _Tee.fileno: _Tee#fileno().
  LOG_DIR: LOG_DIR.
  _Tee: _Tee#
  create_llm_fn.vllm_fn: create_llm_fn().vllm_fn().
  create_llm_fn.api_fn: create_llm_fn().api_fn().
  _format_available_actions: _format_available_actions().
  build_react_prompt: build_react_prompt().
  WebShopEvaluator.benchmark_id: WebShopEvaluator#benchmark_id.
  WebShopEvaluator.eval_config: WebShopEvaluator#eval_config.
  _Tee.__init__: _Tee#__init__().
  _Tee.isatty: _Tee#isatty().
  WebShopEvaluator.__init__: WebShopEvaluator#__init__().
  WebShopEvaluator.config: WebShopEvaluator#config.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py)

## Classes
### `WebShopEvaluator`  ·  implements/extends BaseEvaluator
- def: [`rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py:266`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L266)
- doc: WebShop 评测器（ReAct agent）
- signature: `class WebShopEvaluator(BaseEvaluator):`
- members:
  - `run_eval(self, model_path: str, workspace_path: str, **kwargs)` — [`L284`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L284) — 运行 WebShop 评测
  - `benchmark_id` — [`L281`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L281)
  - `config` — [`L280`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L280)
  - `eval_config` — [`L282`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L282)
- protocol/private: `__init__`[`L279`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L279)
- uses (calls/refs, reference-scoped): [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`get_default_result`](../../core/evaluator.md#BaseEvaluator.get_default_result)  (7 test-only)
- used by: [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`run_eval`](../../core/evaluator.md#BaseEvaluator.run_eval)

### `_Tee`
- def: [`rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py:28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L28)
- doc: 同时输出到终端和日志文件
- signature: `class _Tee:`
- members:
  - `fileno(self)` — [`L47`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L47)
  - `flush(self)` — [`L40`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L40)
  - `isatty(self)` — [`L44`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L44)
  - `write(self, message)` — [`L35`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L35)
  - `log` — [`L33`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L33)
  - `terminal` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L32)
- protocol/private: `__init__`[`L31`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L31)
- used by: (1 test-only callers)

## Functions
- `_format_available_actions(avail: dict)` — [`L153`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L153) — 将环境返回的 available_actions 格式化为文本列表
- `_log(msg: str)` — [`L51`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L51) — 简单的 print 日志（会被 Tee 同时写入文件）
- `api_fn(prompt: str, stop: List[str] = None)` — [`L128`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L128)
- `build_react_prompt(instruction: str, history: List[Tuple[str, str]], observation: str, available_actions: str = "", history_window: int = 5)` — [`L163`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L163) — 构建 ReAct 风格的提示词，包含 available_actions 和有限历史窗口
- `cleanup()` — [`L96`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L96)
- `create_llm_fn(backend: str, model_path: str, **kwargs)` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L61) — 创建统一的 llm(prompt, stop) 函数。
- `vllm_fn(prompt: str, stop: List[str] = None)` — [`L87`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L87)
- `webshop_run(llm_fn: Callable, env, instruction: str, observation: str, max_steps: int = 50, history_window: int = 5)` — [`L201`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L201) — 单轮 WebShop 评测逻辑。

## Module values
- `LOG_DIR` — [`L25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/eval.py#L25)

