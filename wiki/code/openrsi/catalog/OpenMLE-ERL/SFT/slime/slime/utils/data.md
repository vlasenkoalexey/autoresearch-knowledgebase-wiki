---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/data.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/data.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.data`/
symbols:
  Dataset.__init__: Dataset#__init__().
  Dataset.shuffle: Dataset#shuffle().
  read_file: read_file().
  filter_long_prompt: filter_long_prompt().
  _build_messages: _build_messages().
  Dataset.samples: Dataset#samples.
  Dataset.origin_samples: Dataset#origin_samples.
  process_rollout_data: process_rollout_data().
  logger: logger.
  Dataset: Dataset#
  get_minimum_num_micro_batch_size: get_minimum_num_micro_batch_size().
  Dataset.__getitem__: Dataset#__getitem__().
  Dataset.__len__: Dataset#__len__().
  Dataset.epoch_id: Dataset#epoch_id.
  read_file.jsonl_reader: read_file().jsonl_reader().
  read_file.parquet_reader: read_file().parquet_reader().
  _parse_generalized_path: _parse_generalized_path().
  Dataset.seed: Dataset#seed.
  __all__: __all__.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/data.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py)

## Classes
### `Dataset`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/data.py:180`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L180)
- signature: `class Dataset:`
- members:
  - `shuffle(self, new_epoch_id)` — [`L253`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L253)
  - `epoch_id` — [`L249`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L249)
  - `origin_samples` — [`L245`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L245)
  - `samples` — [`L251`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L251)
  - `seed` — [`L250`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L250)
- protocol/private: `__getitem__`[`L263`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L263), `__init__`[`L181`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L181), `__len__`[`L266`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L266)
- uses (calls/refs, reference-scoped): [`Sample`](types.md#Sample), [`metadata`](types.md#Sample.metadata), [`_build_messages`](data.md#_build_messages), [`filter_long_prompt`](data.md#filter_long_prompt), [`prompt`](types.md#Sample.prompt), [`read_file`](data.md#read_file), [`process_vision_info`](processing_utils.md#process_vision_info), [`multimodal_inputs`](types.md#Sample.multimodal_inputs), [`label`](types.md#Sample.label)
- used by: [`eval_rollout_single_dataset`](../rollout/sglang_rollout.md#eval_rollout_single_dataset), [`get_samples`](../rollout/data_source.md#RolloutDataSource.get_samples), [`dataset`](../rollout/data_source.md#RolloutDataSource.dataset), [`load`](../rollout/data_source.md#RolloutDataSource.load)

## Functions
- `_build_messages(data: dict, prompt_key: str, as_conversation: bool, multimodal_keys: dict = None)` — [`L115`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L115)
- `_parse_generalized_path(s: str)` — [`L71`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L71)
- `filter_long_prompt(origin_samples: list[Sample], tokenizer, processor, max_length: int | None)` — [`L81`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L81)
- `get_minimum_num_micro_batch_size(total_lengths, max_tokens_per_gpu)` — [`L270`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L270)
- `jsonl_reader(p)` — [`L34`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L34)
- `parquet_reader(p)` — [`L52`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L52)
- `process_rollout_data(args, rollout_data_ref, dp_rank, dp_size)` — [`L284`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L284)
- `read_file(path)` — [`L25`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L25)

## Module values
- `__all__` — [`L20`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L20)
- `logger` — [`L22`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/data.py#L22)

