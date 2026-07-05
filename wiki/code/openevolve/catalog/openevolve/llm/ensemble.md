---
title: 'Module: openevolve/llm/ensemble.py'
type: catalog
provenance: extracted
module: openevolve/llm/ensemble.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.llm.ensemble`/
symbols:
  LLMEnsemble._sample_model: LLMEnsemble#_sample_model().
  LLMEnsemble: LLMEnsemble#
  LLMEnsemble.random_state: LLMEnsemble#random_state.
  LLMEnsemble.weights: LLMEnsemble#weights.
  LLMEnsemble.models: LLMEnsemble#models.
  LLMEnsemble.generate: LLMEnsemble#generate().
  LLMEnsemble.generate_with_context: LLMEnsemble#generate_with_context().
  LLMEnsemble.generate_all_with_context: LLMEnsemble#generate_all_with_context().
  logger: logger.
  LLMEnsemble.__init__: LLMEnsemble#__init__().
  LLMEnsemble.generate_multiple: LLMEnsemble#generate_multiple().
  LLMEnsemble.parallel_generate: LLMEnsemble#parallel_generate().
  LLMEnsemble.models_cfg: LLMEnsemble#models_cfg.
---
# Module: [`openevolve/llm/ensemble.py`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py)

## Classes
### `LLMEnsemble`
- def: [`openevolve/llm/ensemble.py:17`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L17) — documented in [openevolve-llm-ensemble](../../../concepts/openevolve-llm-ensemble.md)
- doc: Ensemble of LLMs
- signature: `class LLMEnsemble:`
- members:
  - `_sample_model(self)` — [`L70`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L70) — Sample a model from the ensemble based on weights — documented in [openevolve-llm-ensemble](../../../concepts/openevolve-llm-ensemble.md)
  - `generate(self, prompt: str, **kwargs)` — [`L58`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L58) — Generate text using a randomly selected model based on weights — documented in [openevolve-llm-ensemble](../../../concepts/openevolve-llm-ensemble.md)
  - `generate_all_with_context(self, system_message: str, messages: List[Dict[str, str]], **kwargs)` — [`L87`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L87) — Generate text using a all available models and average their returned metrics — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `generate_multiple(self, prompt: str, n: int, **kwargs)` — [`L77`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L77) — Generate multiple texts in parallel
  - `generate_with_context(self, system_message: str, messages: List[Dict[str, str]], **kwargs)` — [`L63`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L63) — Generate text using a system message and conversational context — documented in [openevolve-llm-ensemble](../../../concepts/openevolve-llm-ensemble.md)
  - `parallel_generate(self, prompts: List[str], **kwargs)` — [`L82`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L82) — Generate responses for multiple prompts in parallel
  - `models` — [`L24`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L24) — documented in [openevolve-llm-ensemble](../../../concepts/openevolve-llm-ensemble.md)
  - `models_cfg` — [`L21`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L21)
  - `random_state` — [`L35`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L35) — documented in [openevolve-llm-ensemble](../../../concepts/openevolve-llm-ensemble.md)
  - `weights` — [`L30`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L30) — documented in [openevolve-evaluator](../../../concepts/openevolve-evaluator.md)
- protocol/private: `__init__`[`L20`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L20)
- uses (calls/refs, reference-scoped): [`LLMModelConfig`](../config.md#LLMModelConfig), [`generate_with_context`](openai.md#OpenAILLM.generate_with_context), [`name`](../config.md#LLMModelConfig.name), [`weight`](../config.md#LLMModelConfig.weight), [`LLMInterface`](base.md#LLMInterface), [`random_seed`](../config.md#LLMModelConfig.random_seed), [`OpenAILLM`](openai.md#OpenAILLM), [`generate_with_context`](base.md#LLMInterface.generate_with_context), [`generate`](base.md#LLMInterface.generate), [`logger`](ensemble.md#logger), [`init_client`](../config.md#LLMModelConfig.init_client)
- used by: [`run_iteration_with_shared_db`](../iteration.md#run_iteration_with_shared_db), [`_run_iteration_worker`](../process_parallel.md#_run_iteration_worker), [`_llm_evaluate`](../evaluator.md#Evaluator._llm_evaluate), [`_lazy_init_worker_components`](../process_parallel.md#_lazy_init_worker_components), [`llm_ensemble`](../controller.md#OpenEvolve.llm_ensemble), [`llm_evaluator_ensemble`](../controller.md#OpenEvolve.llm_evaluator_ensemble), [`__init__`](../evaluator.md#Evaluator.__init__)  (2 test-only)

## Module values
- `logger` — [`L14`](../../../../../../raw/code/openevolve/openevolve/llm/ensemble.py#L14)

