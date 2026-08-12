---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.client.base`/ClientConfig#
symbols:
  ClientConfig: ''
  ClientConfig.validate: validate().
  ClientConfig.api: api.
  ClientConfig.model_id: model_id.
  ClientConfig.base_url: base_url.
  ClientConfig.api_key: api_key.
  ClientConfig.use_azure_client: use_azure_client.
  ClientConfig.provider: provider.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py)

## Classes
### `ClientConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py:15`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py#L15)
- signature: `class ClientConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L67`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py#L67)
  - `api` — [`L16`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py#L16)
  - `api_key` — [`L42`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py#L42)
  - `base_url` — [`L33`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py#L33)
  - `model_id` — [`L25`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py#L25)
  - `provider` — [`L58`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py#L58)
  - `use_azure_client` — [`L50`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/client/base.py#L50)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate)
- used by: [`BaseConfig`](../../../aira_core/config/base.md#BaseConfig), [`validate`](../../../aira_core/config/base.md#BaseConfig.validate), [`client`](../llm/generic_llm.md#GenericLLMConfig.client)

