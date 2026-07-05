---
title: 'Module: rdagent/scenarios/rl/autorl_bench/core/server.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/core/server.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.core.server`/
symbols:
  GradingServer.submit: GradingServer#submit().
  LocalServerContext.__enter__: LocalServerContext#__enter__().
  submit: submit().
  health: health().
  args: args.
  GradingServer.available_gpus: GradingServer#available_gpus.
  run_server: run_server().
  time_status: time_status().
  GradingServer.set_baseline: GradingServer#set_baseline().
  get_server: get_server().
  init_server: init_server().
  parser: parser.
  _server._server: _server._server.
  app: app.
  GradingServer: GradingServer#
  create_grading_server: create_grading_server().
  set_baseline: set_baseline().
  LocalServerContext.get_baseline: LocalServerContext#get_baseline().
  GradingServer._eval_cache: GradingServer#_eval_cache.
  GradingServer.workspace: GradingServer#workspace.
  GradingServer.get_evaluator: GradingServer#get_evaluator().
  GradingServer.scores_file: GradingServer#scores_file.
  LocalServerContext._http_server: LocalServerContext#_http_server.
  LocalServerContext.load_scores: LocalServerContext#load_scores().
  GradingServer.load_scores: GradingServer#load_scores().
  GradingServerContext: GradingServerContext#
  GradingServer.baseline_score: GradingServer#baseline_score.
  LocalServerContext.port: LocalServerContext#port.
  LocalServerContext.server: LocalServerContext#server.
  GradingServer.save_scores: GradingServer#save_scores().
  GradingServer.resolve_model_path: GradingServer#resolve_model_path().
  GradingServerContext.get_baseline: GradingServerContext#get_baseline().
  GradingServerContext.load_scores: GradingServerContext#load_scores().
  LocalServerContext: LocalServerContext#
  GradingServer._make_cache_key: GradingServer#_make_cache_key().
  LocalServerContext.__exit__: LocalServerContext#__exit__().
  _validate_gpu: _validate_gpu().
  GradingServer.task: GradingServer#task.
  LocalServerContext._thread: LocalServerContext#_thread.
  _get_available_gpus: _get_available_gpus().
  GradingServer.base_model: GradingServer#base_model.
  GradingServer._eval_lock: GradingServer#_eval_lock.
  LocalServerContext.task: LocalServerContext#task.
  LocalServerContext.base_model: LocalServerContext#base_model.
  LocalServerContext.workspace: LocalServerContext#workspace.
  GradingServer.__init__: GradingServer#__init__().
  GradingServerContext.__enter__: GradingServerContext#__enter__().
  GradingServerContext.__exit__: GradingServerContext#__exit__().
  LocalServerContext.__init__: LocalServerContext#__init__().
---
# Module: [`rdagent/scenarios/rl/autorl_bench/core/server.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py)

## Classes
### `GradingServer`
- def: [`rdagent/scenarios/rl/autorl_bench/core/server.py:44`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L44)
- doc: 评测服务器
- signature: `class GradingServer:`
- members:
  - `_make_cache_key(resolved_path: Path)` — [`L63`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L63) — 用路径 + safetensors/bin 文件最新 mtime 组合作为 cache key。
  - `get_evaluator(self)` — [`L85`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L85) — 获取当前 task 的评测器
  - `load_scores(self)` — [`L77`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L77)
  - `resolve_model_path(self, model_path: str)` — [`L91`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L91) — 将模型路径约束在 workspace 下，防止访问任意文件系统路径。
  - `save_scores(self, scores: list[dict])` — [`L82`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L82)
  - `set_baseline(self, score: float)` — [`L226`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L226) — 设置 baseline 分数
  - `submit(self, model_path: str, gpu: Optional[str] = None)` — [`L113`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L113) — 提交模型评测
  - `available_gpus` — [`L58`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L58)
  - `base_model` — [`L54`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L54)
  - `baseline_score` — [`L57`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L57)
  - `scores_file` — [`L56`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L56)
  - `task` — [`L53`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L53)
  - `workspace` — [`L55`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L55)
- protocol/private: `__init__`[`L47`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L47), `_eval_cache`[`L60`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L60), `_eval_lock`[`L59`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L59)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../log/logger.md#RDAgentLog.info), [`run_eval`](evaluator.md#BaseEvaluator.run_eval), [`update_run_meta`](utils.md#update_run_meta), [`_validate_gpu`](server.md#_validate_gpu), [`_get_available_gpus`](server.md#_get_available_gpus)  (1 test-only)
- used by: [`submit`](server.md#submit), [`health`](server.md#health), [`time_status`](server.md#time_status), [`get_server`](server.md#get_server), [`init_server`](server.md#init_server), [`_server`](server.md#_server._server), [`get_baseline`](server.md#LocalServerContext.get_baseline), [`set_baseline`](server.md#set_baseline), [`load_scores`](server.md#LocalServerContext.load_scores)  (3 test-only)

### `GradingServerContext`
- def: [`rdagent/scenarios/rl/autorl_bench/core/server.py:361`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L361)
- doc: Grading Server 基类
- signature: `class GradingServerContext:`
- members:
  - `get_baseline(self, task: str, model_name: str, model_path: str, workspace_path: str)` — [`L370`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L370)
  - `load_scores(self)` — [`L373`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L373)
- protocol/private: `__enter__`[`L364`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L364), `__exit__`[`L367`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L367)
- uses (calls/refs, reference-scoped): [`get_baseline`](server.md#LocalServerContext.get_baseline), [`load_scores`](server.md#LocalServerContext.load_scores), [`LocalServerContext`](server.md#LocalServerContext)
- used by: [`run`](../run.md#run), [`create_grading_server`](server.md#create_grading_server), [`LocalServerContext`](server.md#LocalServerContext)

### `LocalServerContext`  ·  implements/extends GradingServerContext
- def: [`rdagent/scenarios/rl/autorl_bench/core/server.py:377`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L377)
- doc: 本地 Flask Server
- signature: `class LocalServerContext(GradingServerContext):`
- members:
  - `get_baseline(self, task: str, model_name: str, model_path: str, workspace_path: str)` — [`L417`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L417)
  - `load_scores(self)` — [`L424`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L424)
  - `base_model` — [`L382`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L382)
  - `port` — [`L384`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L384)
  - `server` — [`L385`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L385)
  - `task` — [`L381`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L381)
  - `workspace` — [`L383`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L383)
- protocol/private: `__enter__`[`L389`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L389), `__exit__`[`L412`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L412), `__init__`[`L380`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L380), `_http_server`[`L386`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L386), `_thread`[`L387`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L387)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../../log/logger.md#RDAgentLog.info), [`get_baseline_score`](utils.md#get_baseline_score), [`set_baseline`](server.md#GradingServer.set_baseline), [`init_server`](server.md#init_server), [`app`](server.md#app), [`GradingServerContext`](server.md#GradingServerContext), [`load_scores`](server.md#GradingServer.load_scores)
- used by: [`create_grading_server`](server.md#create_grading_server), [`GradingServerContext`](server.md#GradingServerContext), [`get_baseline`](server.md#GradingServerContext.get_baseline), [`load_scores`](server.md#GradingServerContext.load_scores)

## Functions
- `_get_available_gpus()` — [`L25`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L25) — 从 CUDA_VISIBLE_DEVICES 获取可用 GPU 集合
- `_validate_gpu(gpu: str, available: Set[str])` — [`L33`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L33) — 校验 gpu 参数，返回错误信息或 None（合法）
- `create_grading_server(benchmark, workspace: Path, port: int, base_model: str)` — [`L428`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L428) — 创建 Grading Server 上下文
- `get_server()` — [`L236`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L236)
- `health()` — [`L302`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L302) — 健康检查
- `init_server(task: str, base_model: str, workspace: str)` — [`L243`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L243) — 初始化服务器
- `run_server(task: str, base_model: str, workspace: str, host: str = "0.0.0.0", port: int = 5000)` — [`L349`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L349) — 启动服务器
- `set_baseline()` — [`L336`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L336) — 设置 baseline 分数
- `submit()` — [`L252`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L252) — 提交模型评测
- `time_status()` — [`L316`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L316) — 时间与预算信号

## Module values
- `_server` — [`L233`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L233)
- `app` — [`L22`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L22)
- `args` — [`L447`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L447)
- `parser` — [`L441`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/server.py#L441)

