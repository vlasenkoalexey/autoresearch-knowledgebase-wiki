---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks.alfworld.eval`/
symbols:
  ALFWorldEvaluator.run_eval: ALFWorldEvaluator#run_eval().
  _log: _log().
  create_llm_fn: create_llm_fn().
  alfworld_run: alfworld_run().
  ALFWorldEvaluator._expand_env_vars: ALFWorldEvaluator#_expand_env_vars().
  _Tee.write: _Tee#write().
  _Tee.flush: _Tee#flush().
  _Tee.log: _Tee#log.
  _Tee.close: _Tee#close().
  create_llm_fn.vllm_fn: create_llm_fn().vllm_fn().
  create_llm_fn.cleanup: create_llm_fn().cleanup().
  ALFWorldEvaluator._ensure_alfworld_data: ALFWorldEvaluator#_ensure_alfworld_data().
  _Tee.terminal: _Tee#terminal.
  _truncate_prompt_to_fit: _truncate_prompt_to_fit().
  _Tee.fileno: _Tee#fileno().
  ALFWorldEvaluator: ALFWorldEvaluator#
  LOG_DIR: LOG_DIR.
  TASK_PREFIXES: TASK_PREFIXES.
  _Tee: _Tee#
  process_ob: process_ob().
  create_llm_fn.api_fn: create_llm_fn().api_fn().
  ALFWorldEvaluator.benchmark_id: ALFWorldEvaluator#benchmark_id.
  ALFWorldEvaluator.eval_config: ALFWorldEvaluator#eval_config.
  _Tee.__init__: _Tee#__init__().
  _Tee.isatty: _Tee#isatty().
  ALFWorldEvaluator.__init__: ALFWorldEvaluator#__init__().
  ALFWorldEvaluator.config: ALFWorldEvaluator#config.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py)

## Classes
### `ALFWorldEvaluator`  ·  implements/extends BaseEvaluator
- def: [`rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py:217`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L217)
- doc: ALFWorld 评测器（ReAct agent）
- signature: `class ALFWorldEvaluator(BaseEvaluator):`
- members:
  - `_ensure_alfworld_data()` — [`L390`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L390) — 检查 ALFWorld 游戏数据（~2.1GB），没有就自动下载
  - `_expand_env_vars(self, obj)` — [`L401`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L401) — 递归展开 $ENV_VAR
  - `run_eval(self, model_path: str, workspace_path: str, **kwargs)` — [`L235`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L235) — 运行 ALFWorld 评测
  - `benchmark_id` — [`L232`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L232)
  - `config` — [`L231`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L231)
  - `eval_config` — [`L233`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L233)
- protocol/private: `__init__`[`L230`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L230)
- uses (calls/refs, reference-scoped): [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`get_default_result`](../../core/evaluator.md#BaseEvaluator.get_default_result)  (8 test-only)
- used by: [`BaseEvaluator`](../../core/evaluator.md#BaseEvaluator), [`run_eval`](../../core/evaluator.md#BaseEvaluator.run_eval)

### `_Tee`
- def: [`rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py:25`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L25)
- doc: 同时输出到终端和日志文件
- signature: `class _Tee:`
- members:
  - `close(self)` — [`L47`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L47)
  - `fileno(self)` — [`L44`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L44)
  - `flush(self)` — [`L37`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L37)
  - `isatty(self)` — [`L41`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L41)
  - `write(self, message)` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L32)
  - `log` — [`L30`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L30)
  - `terminal` — [`L29`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L29)
- protocol/private: `__init__`[`L28`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L28)
- used by: (1 test-only callers)

## Functions
- `_log(msg: str)` — [`L51`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L51) — 简单的 print 日志（会被 Tee 同时写入文件）
- `_truncate_prompt_to_fit(prompt: str, tokenizer, max_context_tokens: int, max_output_tokens: int)` — [`L56`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L56) — Trim old ReAct history when it no longer fits the vLLM context.
- `alfworld_run(llm_fn: Callable, env, prompt: str, ob: str, max_steps: int = 50)` — [`L89`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L89) — ReAct 官方的单局评测逻辑。
- `api_fn(prompt: str, stop: List[str] = None)` — [`L189`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L189)
- `cleanup()` — [`L157`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L157)
- `create_llm_fn(backend: str, model_path: str, **kwargs)` — [`L126`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L126) — 创建统一的 llm(prompt, stop) 函数。
- `process_ob(ob: str)` — [`L82`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L82) — 官方 ReAct 的 observation 清洗
- `vllm_fn(prompt: str, stop: List[str] = None)` — [`L150`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L150)

## Module values
- `LOG_DIR` — [`L22`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L22)
- `TASK_PREFIXES` — [`L72`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/eval.py#L72)

