---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.llm.generic_llm`/GenericLLMConfig#
symbols:
  GenericLLMConfig: ''
  GenericLLMConfig.client: client.
  GenericLLMConfig.validate: validate().
  GenericLLMConfig.generation_kwargs: generation_kwargs.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py)

## Classes
### `GenericLLMConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py:16`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py#L16)
- signature: `class GenericLLMConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L30`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py#L30)
  - `client` — [`L17`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py#L17)
  - `generation_kwargs` — [`L25`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/llm/generic_llm.py#L25)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`ClientConfig`](../client/base.md#ClientConfig)
- used by: [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`client`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM.client), [`llm`](../operators/base.md#OperatorConfig.llm)

