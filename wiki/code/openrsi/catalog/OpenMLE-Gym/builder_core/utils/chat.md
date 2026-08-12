---
title: 'Module: OpenMLE-Gym/builder_core/utils/chat.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/builder_core/utils/chat.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.builder_core.utils.chat`/OpenAILLMProvider#
symbols:
  OpenAILLMProvider.query: query().
  OpenAILLMProvider.llm: llm.
  OpenAILLMProvider.model: model.
  OpenAILLMProvider.api_key: api_key.
  OpenAILLMProvider.base_url: base_url.
  OpenAILLMProvider: ''
  OpenAILLMProvider.__init__: __init__().
  OpenAILLMProvider.outlen: outlen.
  OpenAILLMProvider.stream: stream.
---
# Module: [`OpenMLE-Gym/builder_core/utils/chat.py`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py)

## Classes
### `OpenAILLMProvider`
- def: [`OpenMLE-Gym/builder_core/utils/chat.py:5`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L5)
- signature: `class OpenAILLMProvider:`
- members:
  - `query(self, prompts)` — [`L24`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L24) — documented in [OpenMLE-Gym-builder_core-utils-nodes](../../../../concepts/OpenMLE-Gym-builder_core-utils-nodes.md)
  - `api_key` — [`L10`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L10)
  - `base_url` — [`L11`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L11)
  - `llm` — [`L15`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L15)
  - `model` — [`L12`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L12)
  - `outlen` — [`L22`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L22)
  - `stream` — [`L13`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L13)
- protocol/private: `__init__`[`L6`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/utils/chat.py#L6)
- uses (calls/refs, reference-scoped): [`build_llm_config`](../../openmle_gym/llm_config.md#build_llm_config), [`api_key`](../../openmle_gym/llm_config.md#OpenAICompatibleConfig.api_key), [`model`](../../openmle_gym/llm_config.md#OpenAICompatibleConfig.model), [`base_url`](../../openmle_gym/llm_config.md#OpenAICompatibleConfig.base_url)
- used by: [`Metric`](nodes.md#NodeExecutor.Metric), [`Perceive`](nodes.md#NodeExecutor.Perceive), [`Prepare`](nodes.md#NodeExecutor.Prepare), [`Describe`](nodes.md#NodeExecutor.Describe), [`llm_provider_tools`](nodes.md#NodeExecutor.llm_provider_tools), [`llm_provider`](nodes.md#NodeExecutor.llm_provider)

