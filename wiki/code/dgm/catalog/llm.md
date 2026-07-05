---
title: 'Module: llm.py'
type: catalog
provenance: extracted
module: llm.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 llm/
symbols:
  get_response_from_llm: get_response_from_llm().
  create_client: create_client().
  MAX_OUTPUT_TOKENS: MAX_OUTPUT_TOKENS.
  get_batch_responses_from_llm: get_batch_responses_from_llm().
  extract_json_between_markers: extract_json_between_markers().
  AVAILABLE_LLMS: AVAILABLE_LLMS.
---
# Module: [`llm.py`](../../../../raw/code/dgm/llm.py)

## Functions
- `create_client(model: str)` — [`L44`](../../../../raw/code/dgm/llm.py#L44) — Create and return an LLM client based on the specified model. — documented in [coding_agent](../concepts/coding_agent.md)
- `extract_json_between_markers(llm_output)` — [`L305`](../../../../raw/code/dgm/llm.py#L305)
- `get_batch_responses_from_llm(msg, client, model, system_message, print_debug=False, msg_history=None, temperature=0.75, n_responses=1)` — [`L89`](../../../../raw/code/dgm/llm.py#L89)
- `get_response_from_llm(msg, client, model, system_message, print_debug=False, msg_history=None, temperature=0.7)` — [`L172`](../../../../raw/code/dgm/llm.py#L172) — documented in [coding_agent](../concepts/coding_agent.md)

## Module values
- `AVAILABLE_LLMS` — [`L11`](../../../../raw/code/dgm/llm.py#L11)
- `MAX_OUTPUT_TOKENS` — [`L10`](../../../../raw/code/dgm/llm.py#L10)

