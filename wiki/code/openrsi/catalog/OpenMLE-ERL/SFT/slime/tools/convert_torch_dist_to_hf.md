---
title: 'Module: OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.tools.convert_torch_dist_to_hf`/
symbols:
  args: args.
  megatron_args: megatron_args.
  parser: parser.
  save_tensors: save_tensors().
  hf_config: hf_config.
  state_dict: state_dict.
  get_layer_param: get_layer_param().
  get_named_params: get_named_params().
  UnpicklerWrapper.find_class: UnpicklerWrapper#find_class().
  WrappedStorageReader.read_metadata: WrappedStorageReader#read_metadata().
  UnpicklerWrapper: UnpicklerWrapper#
  get_expert_param: get_expert_param().
  UnpicklerWrapper.find_class.DummyClass: UnpicklerWrapper#find_class().DummyClass#
  WrappedStorageReader: WrappedStorageReader#
  EmptyStateDictLoadPlanner: EmptyStateDictLoadPlanner#
  copy_assets: copy_assets().
  t: t.
  UnpicklerWrapper.find_class.DummyClass.__init__: UnpicklerWrapper#find_class().DummyClass#__init__().
  EmptyStateDictLoadPlanner.set_up_planner: EmptyStateDictLoadPlanner#set_up_planner().
---
# Module: [`OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py)

## Classes
### `DummyClass`
- def: [`OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py:22`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L22)
- signature: `class DummyClass:`
- protocol/private: `__init__`[`L23`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L23)
- used by: [`find_class`](convert_torch_dist_to_hf.md#UnpicklerWrapper.find_class)

### `EmptyStateDictLoadPlanner`
- def: [`OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py:48`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L48)
- signature: `class EmptyStateDictLoadPlanner(dist_cp.default_planner.DefaultLoadPlanner):`
- members:
  - `set_up_planner(self, state_dict: dist_cp.metadata.STATE_DICT_TYPE, metadata: dist_cp.metadata.Metadata | None = None, is_coordinator: bool = False)` — [`L50`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L50)
- used by: [`megatron_args`](convert_torch_dist_to_hf.md#megatron_args)

### `UnpicklerWrapper`  ·  implements/extends Unpickler
- def: [`OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py:19`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L19)
- signature: `class UnpicklerWrapper(pickle.Unpickler):`
- members:
  - `find_class(self, mod_name, name)` — [`L21`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L21)
- uses (calls/refs, reference-scoped): [`DummyClass`](convert_torch_dist_to_hf.md#UnpicklerWrapper.find_class.DummyClass)
- used by: [`read_metadata`](convert_torch_dist_to_hf.md#WrappedStorageReader.read_metadata)

### `WrappedStorageReader`
- def: [`OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py:34`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L34)
- signature: `class WrappedStorageReader(dist_cp.FileSystemReader):`
- members:
  - `read_metadata(self)` — [`L36`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L36)
- uses (calls/refs, reference-scoped): [`UnpicklerWrapper`](convert_torch_dist_to_hf.md#UnpicklerWrapper)
- used by: [`megatron_args`](convert_torch_dist_to_hf.md#megatron_args)

## Functions
- `copy_assets(origin_hf_dir, output_dir)` — [`L151`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L151)
- `get_expert_param(args, name, param)` — [`L66`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L66)
- `get_layer_param(args, name, param)` — [`L89`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L89)
- `get_named_params(args, state_dict)` — [`L106`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L106)
- `save_tensors(args, model_name, state_dict, output_dir, chunk_size, vocab_size=None)` — [`L112`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L112)

## Module values
- `args` — [`L190`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L190)
- `hf_config` — [`L201`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L201)
- `megatron_args` — [`L207`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L207)
- `parser` — [`L165`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L165)
- `state_dict` — [`L204`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L204)
- `t` — [`L206`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/tools/convert_torch_dist_to_hf.py#L206)

