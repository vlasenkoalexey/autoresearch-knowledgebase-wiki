---
title: 'Module: openevolve/llm/base.py'
type: catalog
provenance: extracted
module: openevolve/llm/base.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.llm.base`/LLMInterface#
symbols:
  LLMInterface: ''
  LLMInterface.generate_with_context: generate_with_context().
  LLMInterface.generate: generate().
---
# Module: [`openevolve/llm/base.py`](../../../../../../raw/code/openevolve/openevolve/llm/base.py)

## Classes
### `LLMInterface`  ·  implements/extends ABC
- def: [`openevolve/llm/base.py:9`](../../../../../../raw/code/openevolve/openevolve/llm/base.py#L9) — documented in [openevolve-llm-ensemble](../../../concepts/openevolve-llm-ensemble.md)
- doc: Abstract base class for LLM interfaces
- signature: `class LLMInterface(ABC):`
- members:
  - `generate(self, prompt: str, **kwargs)` — [`L13`](../../../../../../raw/code/openevolve/openevolve/llm/base.py#L13) — Generate text from a prompt
  - `generate_with_context(self, system_message: str, messages: List[Dict[str, str]], **kwargs)` — [`L18`](../../../../../../raw/code/openevolve/openevolve/llm/base.py#L18) — Generate text using a system message and conversational context — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
- uses (calls/refs, reference-scoped): [`generate_with_context`](openai.md#OpenAILLM.generate_with_context), [`OpenAILLM`](openai.md#OpenAILLM), [`generate`](openai.md#OpenAILLM.generate)  (3 test-only)
- used by: [`_llm_judge_novelty`](../database.md#ProgramDatabase._llm_judge_novelty), [`_sample_model`](ensemble.md#LLMEnsemble._sample_model), [`OpenAILLM`](openai.md#OpenAILLM), [`generate`](ensemble.md#LLMEnsemble.generate), [`generate_with_context`](ensemble.md#LLMEnsemble.generate_with_context), [`novelty_llm`](../config.md#DatabaseConfig.novelty_llm)  (1 test-only)

