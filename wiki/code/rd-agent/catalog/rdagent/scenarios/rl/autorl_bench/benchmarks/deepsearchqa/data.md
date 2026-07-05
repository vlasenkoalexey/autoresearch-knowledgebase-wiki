---
title: 'Module: rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.rl.autorl_bench.benchmarks.deepsearchqa.data`/
symbols:
  download_train_data: download_train_data().
  split_dataset: split_dataset().
  load_source_dataset: load_source_dataset().
  UNUSED_SIZE: UNUSED_SIZE.
  TRAIN_SIZE: TRAIN_SIZE.
  DATASET_NAME: DATASET_NAME.
  SOURCE_SPLIT: SOURCE_SPLIT.
  DEFAULT_EVAL_SIZE: DEFAULT_EVAL_SIZE.
  SPLIT_SEED: SPLIT_SEED.
  TOTAL_SIZE: TOTAL_SIZE.
---
# Module: [`rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py)

## Functions
- `download_train_data(target_dir: Path)` — [`L32`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L32) — Download and persist the held-in 100-sample training split for agents.
- `load_source_dataset()` — [`L17`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L17) — Load the single official DeepSearchQA split.
- `split_dataset(dataset: Dataset)` — [`L22`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L22) — Create a deterministic 100/200 train/eval split from the 900-item eval set.

## Module values
- `DATASET_NAME` — [`L8`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L8)
- `DEFAULT_EVAL_SIZE` — [`L12`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L12)
- `SOURCE_SPLIT` — [`L9`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L9)
- `SPLIT_SEED` — [`L10`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L10)
- `TOTAL_SIZE` — [`L13`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L13)
- `TRAIN_SIZE` — [`L11`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L11)
- `UNUSED_SIZE` — [`L14`](../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/rl/autorl_bench/benchmarks/deepsearchqa/data.py#L14)

