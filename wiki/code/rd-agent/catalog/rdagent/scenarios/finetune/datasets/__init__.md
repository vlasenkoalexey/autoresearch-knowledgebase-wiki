---
title: 'Module: rdagent/scenarios/finetune/datasets/__init__.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/datasets/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.datasets`/
symbols:
  DATASETS.DATASETS: DATASETS.DATASETS.
  prepare: prepare().
  path: path.
  DatasetConfig: DatasetConfig#
  DatasetConfig.repo_id: DatasetConfig#repo_id.
  prepare_all: prepare_all().
  DatasetConfig.post_download_fn: DatasetConfig#post_download_fn.
  _remove_eval_splits: _remove_eval_splits().
  dataset_name: dataset_name.
---
# Module: [`rdagent/scenarios/finetune/datasets/__init__.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py)

## Classes
### `DatasetConfig`
- def: [`rdagent/scenarios/finetune/datasets/__init__.py:23`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L23)
- doc: Configuration for a registered dataset.
- signature: `class DatasetConfig:`
- members:
  - `post_download_fn` — [`L32`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L32)
  - `repo_id` — [`L31`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L31)
- used by: [`DATASETS`](__init__.md#DATASETS.DATASETS), [`prepare`](__init__.md#prepare)

## Functions
- `_remove_eval_splits(out_dir: str)` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L35) — Remove validation and test split files to prevent data leakage.
- `prepare(name: str, force: bool = False)` — [`L71`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L71) — Download dataset to local directory using snapshot_download.
- `prepare_all(force: bool = False)` — [`L113`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L113) — Prepare all registered datasets.

## Module values
- `DATASETS` — [`L46`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L46)
- `dataset_name` — [`L129`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L129)
- `path` — [`L130`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/__init__.py#L130)

