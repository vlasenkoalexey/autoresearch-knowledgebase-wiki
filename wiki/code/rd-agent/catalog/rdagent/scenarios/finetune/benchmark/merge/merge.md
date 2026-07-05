---
title: 'Module: rdagent/scenarios/finetune/benchmark/merge/merge.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/benchmark/merge/merge.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.benchmark.merge.merge`/
symbols:
  merge_model: merge_model().
  check_if_merging_needed: check_if_merging_needed().
  is_blackwell_gpu: is_blackwell_gpu().
  BLACKWELL_GPU_KEYWORDS: BLACKWELL_GPU_KEYWORDS.
---
# Module: [`rdagent/scenarios/finetune/benchmark/merge/merge.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/merge/merge.py)

## Functions
- `check_if_merging_needed(model_path: str | Path)` — [`L29`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/merge/merge.py#L29) — Check if the model needs to be merged before benchmarking.
- `is_blackwell_gpu()` — [`L12`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/merge/merge.py#L12) — Check if the current GPU is NVIDIA Blackwell architecture (B100, B200, B300).
- `merge_model(env, workspace_path: Path, base_model_path: str, adapter_path: str, output_path: str)` — [`L50`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/merge/merge.py#L50) — Merge LoRA adapter into base model using a template-generated script.

## Module values
- `BLACKWELL_GPU_KEYWORDS` — [`L9`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/merge/merge.py#L9)

