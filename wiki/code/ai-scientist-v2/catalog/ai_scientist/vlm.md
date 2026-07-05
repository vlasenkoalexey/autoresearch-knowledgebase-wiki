---
title: 'Module: ai_scientist/vlm.py'
type: catalog
provenance: extracted
module: ai_scientist/vlm.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.vlm`/
symbols:
  get_response_from_vlm: get_response_from_vlm().
  get_batch_responses_from_vlm: get_batch_responses_from_vlm().
  MAX_NUM_TOKENS: MAX_NUM_TOKENS.
  make_vlm_call: make_vlm_call().
  make_llm_call: make_llm_call().
  create_client: create_client().
  extract_json_between_markers: extract_json_between_markers().
  AVAILABLE_VLMS: AVAILABLE_VLMS.
  encode_image_to_base64: encode_image_to_base64().
  prepare_vlm_prompt: prepare_vlm_prompt().
---
# Module: [`ai_scientist/vlm.py`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py)

## Functions
- `create_client(model: str)` — [`L195`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L195) — Create client for vision-language model. — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `encode_image_to_base64(image_path: str)` — [`L35`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L35) — Convert an image to base64 string. — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `extract_json_between_markers(llm_output: str)` — [`L216`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L216) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `get_batch_responses_from_vlm(msg: str, image_paths: str | list[str], client: Any, model: str, system_message: str, print_debug: bool = False, msg_history: list[dict[str, Any]] | None = None, temperature: float = 0.7, n_responses: int = 1, max_images: int = 200)` — [`L251`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L251) — Get multiple responses from vision-language model for the same input.
- `get_response_from_vlm(msg: str, image_paths: str | list[str], client: Any, model: str, system_message: str, print_debug: bool = False, msg_history: list[dict[str, Any]] | None = None, temperature: float = 0.7, max_images: int = 25)` — [`L132`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L132) — Get response from vision-language model. — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `make_llm_call(client, model, temperature, system_message, prompt)` — [`L53`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L53) — documented in [ai_scientist-utils-token_tracker](../../concepts/ai_scientist-utils-token_tracker.md)
- `make_vlm_call(client, model, temperature, system_message, prompt)` — [`L96`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L96) — documented in [ai_scientist-utils-token_tracker](../../concepts/ai_scientist-utils-token_tracker.md)
- `prepare_vlm_prompt(msg, image_paths, max_images)` — [`L121`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L121)

## Module values
- `AVAILABLE_VLMS` — [`L13`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L13) — documented in [launch_scientist_bfts](../../concepts/launch_scientist_bfts.md)
- `MAX_NUM_TOKENS` — [`L11`](../../../../../raw/code/ai-scientist-v2/ai_scientist/vlm.py#L11)

