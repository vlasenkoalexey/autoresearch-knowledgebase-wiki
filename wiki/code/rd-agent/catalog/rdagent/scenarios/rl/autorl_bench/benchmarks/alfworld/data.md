---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/data.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/data.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks.alfworld.data`/
symbols:
  _ensure_alfworld_data: _ensure_alfworld_data().
  download_train_data: download_train_data().
  _run_alfworld_download: _run_alfworld_download().
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/data.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/data.py)

## Functions
- `_ensure_alfworld_data()` — [`L26`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/data.py#L26) — 确保 alfworld 完整数据已下载，返回数据根目录
- `_run_alfworld_download()` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/data.py#L14) — 调用 alfworld-download，兼容 conda env PATH 问题
- `download_train_data(target_dir: Path)` — [`L58`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/alfworld/data.py#L58) — 准备 ALFWorld 训练数据（agent 可见）

