---
title: 'Module: OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.data_produce.pipeline`/
symbols:
  build_sft_dataset: build_sft_dataset().
  DataProductionConfig: DataProductionConfig#
  DataProductionConfig.source_parquet: DataProductionConfig#source_parquet.
  DataProductionConfig.output_dir: DataProductionConfig#output_dir.
  DataProductionConfig.task_manifest: DataProductionConfig#task_manifest.
  DataProductionConfig.relative_gap_limit: DataProductionConfig#relative_gap_limit.
  DataProductionConfig.run_dir: DataProductionConfig#run_dir.
  DataProductionConfig.tokenizer_model: DataProductionConfig#tokenizer_model.
  DataProductionConfig.task_metadata_parquet: DataProductionConfig#task_metadata_parquet.
  DataProductionConfig.metric_metadata_parquet: DataProductionConfig#metric_metadata_parquet.
  DataProductionConfig.token_limit: DataProductionConfig#token_limit.
  DataProductionConfig.top_k_per_task: DataProductionConfig#top_k_per_task.
  DataProductionConfig.token_workers: DataProductionConfig#token_workers.
---
# Module: [`OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py)

## Classes
### `DataProductionConfig`
- def: [`OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py:26`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L26)
- doc: Configuration for the end-to-end SFT data production pipeline.
- signature: `class DataProductionConfig:`
- members:
  - `metric_metadata_parquet` — [`L54`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L54)
  - `output_dir` — [`L51`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L51)
  - `relative_gap_limit` — [`L56`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L56)
  - `run_dir` — [`L48`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L48)
  - `source_parquet` — [`L49`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L49)
  - `task_manifest` — [`L52`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L52)
  - `task_metadata_parquet` — [`L53`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L53)
  - `token_limit` — [`L55`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L55)
  - `token_workers` — [`L58`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L58)
  - `tokenizer_model` — [`L50`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L50)
  - `top_k_per_task` — [`L57`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L57)
- used by: [`build_sft_dataset`](pipeline.md#build_sft_dataset)

## Functions
- `build_sft_dataset(config: DataProductionConfig)` — [`L61`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/pipeline.py#L61) — Run collect -> token filter -> gap filter -> top-k -> write dataset. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)

