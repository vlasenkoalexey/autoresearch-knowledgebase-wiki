---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.rollout.data_source`/
symbols:
  RolloutDataSource.get_samples: RolloutDataSource#get_samples().
  RolloutDataSource.dataset: RolloutDataSource#dataset.
  RolloutDataSource.load: RolloutDataSource#load().
  RolloutDataSource.args: RolloutDataSource#args.
  RolloutDataSource.save: RolloutDataSource#save().
  RolloutDataSourceWithBuffer.buffer_filter: RolloutDataSourceWithBuffer#buffer_filter.
  RolloutDataSourceWithBuffer._get_samples_from_buffer: RolloutDataSourceWithBuffer#_get_samples_from_buffer().
  RolloutDataSource.metadata: RolloutDataSource#metadata.
  RolloutDataSource.sample_offset: RolloutDataSource#sample_offset.
  RolloutDataSourceWithBuffer.get_samples: RolloutDataSourceWithBuffer#get_samples().
  RolloutDataSourceWithBuffer.add_samples: RolloutDataSourceWithBuffer#add_samples().
  RolloutDataSourceWithBuffer.buffer: RolloutDataSourceWithBuffer#buffer.
  RolloutDataSource: RolloutDataSource#
  RolloutDataSource.epoch_id: RolloutDataSource#epoch_id.
  DataSource.get_samples: DataSource#get_samples().
  DataSource.add_samples: DataSource#add_samples().
  RolloutDataSource.add_samples: RolloutDataSource#add_samples().
  RolloutDataSource.sample_group_index: RolloutDataSource#sample_group_index.
  RolloutDataSource.sample_index: RolloutDataSource#sample_index.
  DataSource: DataSource#
  pop_first: pop_first().
  logger: logger.
  DataSource.save: DataSource#save().
  DataSource.load: DataSource#load().
  RolloutDataSource.__len__: RolloutDataSource#__len__().
  RolloutDataSourceWithBuffer: RolloutDataSourceWithBuffer#
  RolloutDataSourceWithBuffer.__init__: RolloutDataSourceWithBuffer#__init__().
  RolloutDataSourceWithBuffer.update_metadata: RolloutDataSourceWithBuffer#update_metadata().
  RolloutDataSourceWithBuffer.get_metadata: RolloutDataSourceWithBuffer#get_metadata().
  RolloutDataSourceWithBuffer.get_buffer_length: RolloutDataSourceWithBuffer#get_buffer_length().
  RolloutDataSource.__init__: RolloutDataSource#__init__().
  DataSource.__len__: DataSource#__len__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py)

## Classes
### `DataSource`  ·  implements/extends ABC
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py:17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L17)
- signature: `class DataSource(abc.ABC):`
- members:
  - `__len__(self)` — [`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L43) — Length of the data source. May change when samples are added/fetched.
  - `add_samples(self, samples: list[list[Sample]])` — [`L25`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L25) — Add samples to the data source
  - `get_samples(self, num_samples: int)` — [`L19`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L19) — Return num_samples samples
  - `load(self, rollout_id=None)` — [`L37`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L37) — Load the state of the data source
  - `save(self, rollout_id)` — [`L31`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L31) — Save the state of the data source
- uses (calls/refs, reference-scoped): [`Sample`](../utils/types.md#Sample), [`get_samples`](data_source.md#RolloutDataSource.get_samples), [`load`](data_source.md#RolloutDataSource.load), [`save`](data_source.md#RolloutDataSource.save), [`RolloutDataSource`](data_source.md#RolloutDataSource), [`add_samples`](data_source.md#RolloutDataSource.add_samples)
- used by: [`RolloutDataSource`](data_source.md#RolloutDataSource)

### `RolloutDataSource`  ·  implements/extends DataSource
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py:50`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L50)
- signature: `class RolloutDataSource(DataSource):`
- members:
  - `add_samples(self, samples: list[list[Sample]])` — [`L120`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L120)
  - `get_samples(self, num_samples)` — [`L90`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L90)
  - `load(self, rollout_id=None)` — [`L138`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L138)
  - `save(self, rollout_id)` — [`L123`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L123)
  - `args` — [`L52`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L52)
  - `dataset` — [`L71`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L71)
  - `epoch_id` — [`L54`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L54)
  - `metadata` — [`L59`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L59)
  - `sample_group_index` — [`L55`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L55)
  - `sample_index` — [`L56`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L56)
  - `sample_offset` — [`L57`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L57)
- protocol/private: `__init__`[`L51`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L51), `__len__`[`L162`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L162)
- uses (calls/refs, reference-scoped): [`Sample`](../utils/types.md#Sample), [`shuffle`](../utils/data.md#Dataset.shuffle), [`load_processor`](../utils/processing_utils.md#load_processor), [`samples`](../utils/data.md#Dataset.samples), [`load_tokenizer`](../utils/processing_utils.md#load_tokenizer), [`add_samples`](data_source.md#RolloutDataSourceWithBuffer.add_samples), [`get_samples`](data_source.md#RolloutDataSourceWithBuffer.get_samples), [`Dataset`](../utils/data.md#Dataset), [`DataSource`](data_source.md#DataSource), [`logger`](data_source.md#logger), [`RolloutDataSourceWithBuffer`](data_source.md#RolloutDataSourceWithBuffer), [`index`](../utils/types.md#Sample.index), [`group_index`](../utils/types.md#Sample.group_index)
- used by: [`buffer_filter`](data_source.md#RolloutDataSourceWithBuffer.buffer_filter), [`_get_samples_from_buffer`](data_source.md#RolloutDataSourceWithBuffer._get_samples_from_buffer), [`add_samples`](data_source.md#RolloutDataSourceWithBuffer.add_samples), [`get_samples`](data_source.md#RolloutDataSourceWithBuffer.get_samples), [`buffer`](data_source.md#RolloutDataSourceWithBuffer.buffer), [`add_samples`](data_source.md#DataSource.add_samples), [`get_samples`](data_source.md#DataSource.get_samples), [`DataSource`](data_source.md#DataSource), [`RolloutDataSourceWithBuffer`](data_source.md#RolloutDataSourceWithBuffer), [`__init__`](data_source.md#RolloutDataSourceWithBuffer.__init__), [`get_metadata`](data_source.md#RolloutDataSourceWithBuffer.get_metadata), [`load`](data_source.md#DataSource.load), [`save`](data_source.md#DataSource.save), [`update_metadata`](data_source.md#RolloutDataSourceWithBuffer.update_metadata)

### `RolloutDataSourceWithBuffer`  ·  implements/extends RolloutDataSource
- def: [`OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py:166`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L166)
- signature: `class RolloutDataSourceWithBuffer(RolloutDataSource):`
- members:
  - `add_samples(self, samples: list[list[Sample]])` — [`L196`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L196) — Add a sample group to buffer.
  - `get_buffer_length(self)` — [`L219`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L219)
  - `get_metadata(self)` — [`L216`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L216)
  - `get_samples(self, num_samples: int)` — [`L175`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L175) — Return num_samples samples
  - `update_metadata(self, metadata: dict)` — [`L212`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L212)
  - `buffer` — [`L169`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L169)
  - `buffer_filter` — [`L171`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L171)
- protocol/private: `__init__`[`L167`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L167), `_get_samples_from_buffer`[`L189`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L189)
- uses (calls/refs, reference-scoped): [`Sample`](../utils/types.md#Sample), [`load_function`](../utils/misc.md#load_function), [`get_samples`](data_source.md#RolloutDataSource.get_samples), [`args`](data_source.md#RolloutDataSource.args), [`metadata`](data_source.md#RolloutDataSource.metadata), [`RolloutDataSource`](data_source.md#RolloutDataSource), [`pop_first`](data_source.md#pop_first), [`__init__`](data_source.md#RolloutDataSource.__init__)
- used by: [`get_samples`](data_source.md#RolloutDataSource.get_samples), [`RolloutDataSource`](data_source.md#RolloutDataSource), [`add_samples`](data_source.md#RolloutDataSource.add_samples)

## Functions
- `pop_first(args, rollout_id, buffer: list[list[Sample]], num_samples: int)` — [`L223`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L223)

## Module values
- `logger` — [`L14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/rollout/data_source.py#L14)

