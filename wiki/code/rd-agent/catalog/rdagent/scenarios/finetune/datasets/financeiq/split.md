---
title: 'Module: rdagent/scenarios/finetune/datasets/financeiq/split.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/datasets/financeiq/split.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.datasets.financeiq.split`/
symbols:
  split_financeiq_dataset: split_financeiq_dataset().
  get_split_indices: get_split_indices().
---
# Module: [`rdagent/scenarios/finetune/datasets/financeiq/split.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/financeiq/split.py)

## Functions
- `get_split_indices(total_count: int, split: Literal["train", "test"], test_limit: int = 100, test_ratio: float = 0.5)` — [`L7`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/financeiq/split.py#L7) — Calculate the slice for train/test split.
- `split_financeiq_dataset(data_dir: str, split: Literal["train", "test"])` — [`L26`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/datasets/financeiq/split.py#L26) — Iterate over CSV files in the directory and apply the split in-place.

