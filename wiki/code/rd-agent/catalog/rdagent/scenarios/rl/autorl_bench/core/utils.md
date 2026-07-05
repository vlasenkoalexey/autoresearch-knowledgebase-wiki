---
title: 'Module: rdagent/scenarios/rl/autorl_bench/core/utils.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/core/utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.core.utils`/
symbols:
  get_baseline_score: get_baseline_score().
  download_data: download_data().
  setup_workspace: setup_workspace().
  download_model: download_model().
  append_result: append_result().
  print_summary: print_summary().
  kill_process_group: kill_process_group.
  ensure_symlink: ensure_symlink().
  submit_to_grading_server: submit_to_grading_server().
  update_run_meta: update_run_meta().
  read_run_meta: read_run_meta().
  init_run_meta: init_run_meta().
  detect_driver_model: detect_driver_model().
  kill_process_tree: kill_process_tree().
  _safe_model_name: _safe_model_name().
  set_baseline_to_server: set_baseline_to_server().
  RESULTS_CSV_COLUMNS: RESULTS_CSV_COLUMNS.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/core/utils.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py)

## Functions
- `_safe_model_name(model_name: str)` — [`L178`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L178) — 将模型名转为安全的文件名
- `append_result(row: dict)` — [`L372`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L372) — 追加一行到全局 results.csv，返回文件路径。
- `detect_driver_model(env: dict)` — [`L367`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L367) — 从环境变量检测驱动 agent 的 LLM 模型名。
- `download_data(task: str, data_dir: Optional[str] = None)` — [`L119`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L119) — 下载训练数据（agent 可见部分）
- `download_model(model_name: str, model_dir: Optional[str] = None)` — [`L103`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L103) — 下载模型（已存在则跳过）
- `ensure_symlink(src: Path, dst: Path)` — [`L88`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L88) — 创建软链接（已存在则跳过，并发安全）
- `get_baseline_score(task: str, model_name: str, model_path: str, workspace_path: str, gpu_count: int = 1, test_range: str = "[:]", force_rerun: bool = False)` — [`L183`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L183) — 获取 baseline score（有缓存则读缓存，没有则评测）
- `init_run_meta(workspace: Path, timeout_s: int)` — [`L277`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L277) — 初始化 run_meta.json（单一事实源）。
- `kill_process_tree(proc: subprocess.Popen)` — [`L28`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L28) — Kill a process session first, then its process group as a fallback.
- `print_summary(baseline: float, best: dict | None, scores: list, workspace)` — [`L391`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L391) — 打印运行摘要。
- `read_run_meta(workspace: Path)` — [`L299`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L299) — 读取 run_meta.json。
- `set_baseline_to_server(score: float, grading_url: Optional[str] = None)` — [`L261`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L261) — 设置 baseline score 到 grading server
- `setup_workspace(run_id: str, agent_id: str, task: str, base_model: str, model_path: str, data_path: str, benchmark)` — [`L305`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L305) — 创建隔离的 workspace 目录并挂载资源文件，返回 workspace 路径。
- `submit_to_grading_server(model_path: str, grading_url: Optional[str] = None, timeout: int = 600)` — [`L243`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L243) — 提交模型到 grading server 评测
- `update_run_meta(workspace: Path, **fields)` — [`L290`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L290) — 更新 run_meta.json 的部分字段。

## Module values
- `RESULTS_CSV_COLUMNS` — [`L350`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L350)
- `kill_process_group` — [`L80`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/core/utils.py#L80)

