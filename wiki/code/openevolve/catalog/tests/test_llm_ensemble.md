---
title: 'Module: tests/test_llm_ensemble.py'
type: catalog
provenance: extracted
module: tests/test_llm_ensemble.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_llm_ensemble`/
symbols:
  TestLLMEnsemble.test_weighted_sampling: TestLLMEnsemble#test_weighted_sampling().
  TestEnsembleInit.test_ensemble_initialization: TestEnsembleInit#test_ensemble_initialization().
  TestEnsembleInit.MyCustomLLM: TestEnsembleInit#MyCustomLLM#
  TestEnsembleInit.init_custom_llm: TestEnsembleInit#init_custom_llm().
  TestLLMEnsemble: TestLLMEnsemble#
  TestEnsembleInit: TestEnsembleInit#
  TestEnsembleInit.MyCustomLLM.__init__: TestEnsembleInit#MyCustomLLM#__init__().
  MyCustomLLM.model: MyCustomLLM#model.
  MyCustomLLM.some_field: MyCustomLLM#some_field.
  TestEnsembleInit.MyCustomLLM.generate: TestEnsembleInit#MyCustomLLM#generate().
  TestEnsembleInit.MyCustomLLM.generate_with_context: TestEnsembleInit#MyCustomLLM#generate_with_context().
---
# Module: [`tests/test_llm_ensemble.py`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py)

## Classes
### `MyCustomLLM`  ·  implements/extends LLMInterface
- def: [`tests/test_llm_ensemble.py:40`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L40) — documented in [openevolve-llm-ensemble](../../concepts/openevolve-llm-ensemble.md)
- signature: `class MyCustomLLM(LLMInterface):`
- members:
  - `generate(self, prompt: str, **kwargs)` — [`L45`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L45)
  - `generate_with_context(self, system_message: str, messages: List[Dict[str, str]], **kwargs)` — [`L48`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L48)
  - `model` — [`L42`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L42)
  - `some_field` — [`L43`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L43)
- protocol/private: `__init__`[`L41`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L41)
- uses (calls/refs, reference-scoped): [`LLMInterface`](../openevolve/llm/base.md#LLMInterface)
- used by: [`LLMInterface`](../openevolve/llm/base.md#LLMInterface), [`generate_with_context`](../openevolve/llm/base.md#LLMInterface.generate_with_context), [`generate`](../openevolve/llm/base.md#LLMInterface.generate)  (1 test-only)

### `TestEnsembleInit`  ·  implements/extends TestCase
- def: [`tests/test_llm_ensemble.py:39`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L39)
- signature: `class TestEnsembleInit(unittest.TestCase):`
- members:
  - `init_custom_llm(self, model_cfg)` — [`L51`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L51)
  - `test_ensemble_initialization(self)` — [`L54`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L54) — documented in [openevolve-llm-ensemble](../../concepts/openevolve-llm-ensemble.md)
- uses (calls/refs, reference-scoped): [`LLMModelConfig`](../openevolve/config.md#LLMModelConfig), [`name`](../openevolve/config.md#LLMModelConfig.name), [`LLMEnsemble`](../openevolve/llm/ensemble.md#LLMEnsemble), [`models`](../openevolve/llm/ensemble.md#LLMEnsemble.models), [`model`](../openevolve/llm/openai.md#OpenAILLM.model), [`init_client`](../openevolve/config.md#LLMModelConfig.init_client)  (1 test-only)

### `TestLLMEnsemble`  ·  implements/extends TestCase
- def: [`tests/test_llm_ensemble.py:11`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L11)
- signature: `class TestLLMEnsemble(unittest.TestCase):`
- members:
  - `test_weighted_sampling(self)` — [`L12`](../../../../../raw/code/openevolve/tests/test_llm_ensemble.py#L12) — documented in [openevolve-llm-ensemble](../../concepts/openevolve-llm-ensemble.md)
- uses (calls/refs, reference-scoped): [`LLMModelConfig`](../openevolve/config.md#LLMModelConfig), [`api_key`](../openevolve/config.md#LLMModelConfig.api_key), [`name`](../openevolve/config.md#LLMModelConfig.name), [`weight`](../openevolve/config.md#LLMModelConfig.weight), [`_sample_model`](../openevolve/llm/ensemble.md#LLMEnsemble._sample_model), [`LLMEnsemble`](../openevolve/llm/ensemble.md#LLMEnsemble), [`api_base`](../openevolve/config.md#LLMModelConfig.api_base)

