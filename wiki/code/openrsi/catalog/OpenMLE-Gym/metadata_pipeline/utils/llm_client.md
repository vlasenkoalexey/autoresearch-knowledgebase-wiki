---
title: 'Module: OpenMLE-Gym/metadata_pipeline/utils/llm_client.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/metadata_pipeline/utils/llm_client.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.metadata_pipeline.utils.llm_client`/OpenAILLMProvider#
symbols:
  OpenAILLMProvider.llm: llm.
  OpenAILLMProvider.query: query().
  OpenAILLMProvider.model: model.
  OpenAILLMProvider: ''
  OpenAILLMProvider.api_key: api_key.
  OpenAILLMProvider.base_url: base_url.
  OpenAILLMProvider.__init__: __init__().
---
# Module: [`OpenMLE-Gym/metadata_pipeline/utils/llm_client.py`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/utils/llm_client.py)

## Classes
### `OpenAILLMProvider`
- def: [`OpenMLE-Gym/metadata_pipeline/utils/llm_client.py:5`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/utils/llm_client.py#L5)
- signature: `class OpenAILLMProvider:`
- members:
  - `query(self, prompts: list[tuple])` — [`L22`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/utils/llm_client.py#L22)
  - `api_key` — [`L11`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/utils/llm_client.py#L11)
  - `base_url` — [`L12`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/utils/llm_client.py#L12)
  - `llm` — [`L15`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/utils/llm_client.py#L15)
  - `model` — [`L13`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/utils/llm_client.py#L13)
- protocol/private: `__init__`[`L6`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/metadata_pipeline/utils/llm_client.py#L6)
- uses (calls/refs, reference-scoped): [`eval_llm_config`](../../openmle_gym/llm_config.md#eval_llm_config), [`api_key`](../../openmle_gym/llm_config.md#OpenAICompatibleConfig.api_key), [`model`](../../openmle_gym/llm_config.md#OpenAICompatibleConfig.model), [`base_url`](../../openmle_gym/llm_config.md#OpenAICompatibleConfig.base_url)
- used by: [`extract_choice_with_llm`](../task_categorizer.md#extract_choice_with_llm), [`extract_compute_requirement_with_llm`](../compute_requirement_classifier.md#extract_compute_requirement_with_llm), [`llm`](../compute_requirement_classifier.md#llm), [`llm`](../task_categorizer.md#llm)

