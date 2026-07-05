---
title: 'Module: ai_scientist/llm.py'
type: catalog
provenance: extracted
module: ai_scientist/llm.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.llm`/
symbols:
  get_response_from_llm: get_response_from_llm().
  extract_json_between_markers: extract_json_between_markers().
  MAX_NUM_TOKENS: MAX_NUM_TOKENS.
  create_client: create_client().
  AVAILABLE_LLMS: AVAILABLE_LLMS.
  get_batch_responses_from_llm: get_batch_responses_from_llm().
  make_llm_call: make_llm_call().
---
# Module: [`ai_scientist/llm.py`](../../../../../raw/code/ai-scientist-v2/ai_scientist/llm.py)

## Functions
- `create_client(model)` — [`L480`](../../../../../raw/code/ai-scientist-v2/ai_scientist/llm.py#L480) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `extract_json_between_markers(llm_output: str)` — [`L452`](../../../../../raw/code/ai-scientist-v2/ai_scientist/llm.py#L452) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `get_batch_responses_from_llm(prompt, client, model, system_message, print_debug=False, msg_history=None, temperature=0.7, n_responses=1)` — [`L87`](../../../../../raw/code/ai-scientist-v2/ai_scientist/llm.py#L87) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `get_response_from_llm(prompt, client, model, system_message, print_debug=False, msg_history=None, temperature=0.7)` — [`L267`](../../../../../raw/code/ai-scientist-v2/ai_scientist/llm.py#L267) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `make_llm_call(client, model, temperature, system_message, prompt)` — [`L216`](../../../../../raw/code/ai-scientist-v2/ai_scientist/llm.py#L216) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)

## Module values
- `AVAILABLE_LLMS` — [`L13`](../../../../../raw/code/ai-scientist-v2/ai_scientist/llm.py#L13) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `MAX_NUM_TOKENS` — [`L11`](../../../../../raw/code/ai-scientist-v2/ai_scientist/llm.py#L11) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)

