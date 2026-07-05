---
title: 'Module: openevolve/llm/openai.py'
type: catalog
provenance: extracted
module: openevolve/llm/openai.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.llm.openai`/
symbols:
  OpenAILLM.generate_with_context: OpenAILLM#generate_with_context().
  OpenAILLM.client: OpenAILLM#client.
  OpenAILLM._manual_wait_for_answer: OpenAILLM#_manual_wait_for_answer().
  logger: logger.
  OpenAILLM.manual_queue_dir: OpenAILLM#manual_queue_dir.
  OpenAILLM: OpenAILLM#
  OpenAILLM.model: OpenAILLM#model.
  OpenAILLM.generate: OpenAILLM#generate().
  OpenAILLM._call_api: OpenAILLM#_call_api().
  OpenAILLM.retries: OpenAILLM#retries.
  OpenAILLM.reasoning_effort: OpenAILLM#reasoning_effort.
  OpenAILLM.manual_mode: OpenAILLM#manual_mode.
  OpenAILLM.max_tokens: OpenAILLM#max_tokens.
  OpenAILLM.timeout: OpenAILLM#timeout.
  OpenAILLM.api_base: OpenAILLM#api_base.
  _iso_now: _iso_now().
  _build_display_prompt: _build_display_prompt().
  _atomic_write_json: _atomic_write_json().
  OpenAILLM.system_message: OpenAILLM#system_message.
  OpenAILLM.temperature: OpenAILLM#temperature.
  OpenAILLM.top_p: OpenAILLM#top_p.
  OpenAILLM.retry_delay: OpenAILLM#retry_delay.
  OpenAILLM.api_key: OpenAILLM#api_key.
  OpenAILLM.random_seed: OpenAILLM#random_seed.
  OpenAILLM.__init__: OpenAILLM#__init__().
---
# Module: [`openevolve/llm/openai.py`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py)

## Classes
### `OpenAILLM`  ·  implements/extends LLMInterface
- def: [`openevolve/llm/openai.py:47`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L47) — documented in [openevolve-llm-ensemble](../../../concepts/openevolve-llm-ensemble.md)
- doc: LLM interface using OpenAI-compatible APIs
- signature: `class OpenAILLM(LLMInterface):`
- members:
  - `_call_api(self, params: Dict[str, Any])` — [`L212`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L212) — Make the actual API call — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `_manual_wait_for_answer(self, params: Dict[str, Any], timeout: Optional[Union[int, float]])` — [`L228`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L228) — Manual mode: write a task JSON file and poll for *.answer.json — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `generate(self, prompt: str, **kwargs)` — [`L100`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L100) — Generate text from a prompt — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `generate_with_context(self, system_message: str, messages: List[Dict[str, str]], **kwargs)` — [`L108`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L108) — Generate text using a system message and conversational context — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `api_base` — [`L62`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L62) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `api_key` — [`L63`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L63) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `client` — [`L80`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L80) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `manual_mode` — [`L68`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L68) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `manual_queue_dir` — [`L69`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L69) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `max_tokens` — [`L58`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L58) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `model` — [`L54`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L54) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `random_seed` — [`L64`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L64) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `reasoning_effort` — [`L65`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L65) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `retries` — [`L60`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L60) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `retry_delay` — [`L61`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L61) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `system_message` — [`L55`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L55)
  - `temperature` — [`L56`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L56) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `timeout` — [`L59`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L59) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
  - `top_p` — [`L57`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L57) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
- protocol/private: `__init__`[`L50`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L50)
- uses (calls/refs, reference-scoped): [`LLMInterface`](base.md#LLMInterface), [`logger`](openai.md#logger), [`_atomic_write_json`](openai.md#_atomic_write_json), [`_build_display_prompt`](openai.md#_build_display_prompt), [`_iso_now`](openai.md#_iso_now)
- used by: [`LLMInterface`](base.md#LLMInterface), [`models`](ensemble.md#LLMEnsemble.models), [`generate_with_context`](base.md#LLMInterface.generate_with_context), [`generate`](base.md#LLMInterface.generate), [`generate_all_with_context`](ensemble.md#LLMEnsemble.generate_all_with_context)  (3 test-only)

## Functions
- `_atomic_write_json(path: Path, payload: Dict[str, Any])` — [`L40`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L40) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
- `_build_display_prompt(messages: List[Dict[str, str]])` — [`L28`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L28) — Render messages into a single plain-text prompt for the manual UI. — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)
- `_iso_now()` — [`L24`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L24) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)

## Module values
- `logger` — [`L21`](../../../../../../raw/code/openevolve/openevolve/llm/openai.py#L21) — documented in [openevolve-llm-openai](../../../concepts/openevolve-llm-openai.md)

