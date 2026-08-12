---
title: 'Module: OpenMLE-Gym/openmle_gym/llm_config.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/openmle_gym/llm_config.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.openmle_gym.llm_config`/
symbols:
  eval_llm_config: eval_llm_config().
  _stage_config: _stage_config().
  OpenAICompatibleConfig.require: OpenAICompatibleConfig#require().
  build_llm_config: build_llm_config().
  OpenAICompatibleConfig.api_key: OpenAICompatibleConfig#api_key.
  OpenAICompatibleConfig.model: OpenAICompatibleConfig#model.
  OpenAICompatibleConfig: OpenAICompatibleConfig#
  OpenAICompatibleConfig.base_url: OpenAICompatibleConfig#base_url.
  has_explicit_eval_llm_config: has_explicit_eval_llm_config().
---
# Module: [`OpenMLE-Gym/openmle_gym/llm_config.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py)

## Classes
### `OpenAICompatibleConfig`
- def: [`OpenMLE-Gym/openmle_gym/llm_config.py:8`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L8)
- signature: `class OpenAICompatibleConfig:`
- members:
  - `require(self, stage: str)` — [`L13`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L13)
  - `api_key` — [`L9`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L9)
  - `base_url` — [`L10`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L10)
  - `model` — [`L11`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L11)
- used by: [`_evaluate_with_openai`](local_evaluator.md#_evaluate_with_openai), [`eval_llm_config`](llm_config.md#eval_llm_config), [`_stage_config`](llm_config.md#_stage_config), [`build_llm_config`](llm_config.md#build_llm_config), [`model`](../builder_core/utils/chat.md#OpenAILLMProvider.model), [`_require_llm_env`](overview.md#_require_llm_env), [`model`](../metadata_pipeline/utils/llm_client.md#OpenAILLMProvider.model), [`api_key`](../builder_core/utils/chat.md#OpenAILLMProvider.api_key), [`api_key`](../metadata_pipeline/utils/llm_client.md#OpenAILLMProvider.api_key), [`base_url`](../builder_core/utils/chat.md#OpenAILLMProvider.base_url), [`base_url`](../metadata_pipeline/utils/llm_client.md#OpenAILLMProvider.base_url)  (2 test-only)

## Functions
- `_stage_config(prefix: str)` — [`L29`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L29)
- `build_llm_config()` — [`L37`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L37) — Resolve builder LLM settings, with legacy OPENAI_* compatibility.
- `eval_llm_config()` — [`L42`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L42) — Resolve metadata/evaluator LLM settings, with legacy OPENAI_* compatibility.
- `has_explicit_eval_llm_config()` — [`L47`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/llm_config.py#L47)

