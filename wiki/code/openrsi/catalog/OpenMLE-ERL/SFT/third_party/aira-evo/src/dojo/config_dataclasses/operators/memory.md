---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.config_dataclasses.operators.memory`/MemoryOpConfig#
symbols:
  MemoryOpConfig: ''
  MemoryOpConfig.validate: validate().
  MemoryOpConfig.memory_processor: memory_processor.
  MemoryOpConfig.memory_op_kwargs: memory_op_kwargs.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py)

## Classes
### `MemoryOpConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py:15`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py#L15)
- signature: `class MemoryOpConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L31`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py#L31)
  - `memory_op_kwargs` — [`L23`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py#L23)
  - `memory_processor` — [`L16`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/config_dataclasses/operators/memory.py#L16)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate)
- used by: [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`create_memory_op`](../../core/solvers/operators/memory.md#create_memory_op), [`debug_memory`](../solver/base.md#SolverConfig.debug_memory), [`memory`](../solver/base.md#SolverConfig.memory)

