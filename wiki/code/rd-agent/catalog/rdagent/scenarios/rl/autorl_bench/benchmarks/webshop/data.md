---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks.webshop.data`/
symbols:
  WEBSHOP_REPO_DIR: WEBSHOP_REPO_DIR.
  download_train_data: download_train_data().
  _clone_webshop_repo: _clone_webshop_repo().
  _download_webshop_data: _download_webshop_data().
  _ensure_repo_in_path: _ensure_repo_in_path().
  _build_search_index: _build_search_index().
  WEBSHOP_CACHE_DIR: WEBSHOP_CACHE_DIR.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py)

## Functions
- `_build_search_index()` — [`L96`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py#L96) — 构建 WebShop 搜索引擎索引
- `_clone_webshop_repo()` — [`L18`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py#L18) — 克隆 WebShop 仓库到缓存目录
- `_download_webshop_data()` — [`L61`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py#L61) — 下载 WebShop 数据（手动下载，避免 setup.sh 破坏环境依赖）
- `_ensure_repo_in_path()` — [`L36`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py#L36) — 确保 webshop 仓库在 Python 路径中（优先于 PyPI 包）。
- `download_train_data(target_dir: Path)` — [`L127`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py#L127) — 准备 WebShop 训练数据（agent 可见）

## Module values
- `WEBSHOP_CACHE_DIR` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py#L14)
- `WEBSHOP_REPO_DIR` — [`L15`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/webshop/data.py#L15)

