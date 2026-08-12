---
title: 'Module: rlm/core/comms_utils.py'
type: catalog
provenance: extracted
module: rlm/core/comms_utils.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.core.comms_utils`/
symbols:
  send_lm_request_batched: send_lm_request_batched().
  LMResponse.chat_completion: LMResponse#chat_completion.
  send_lm_request: send_lm_request().
  LMRequest: LMRequest#
  LMResponse: LMResponse#
  LMResponse.success: LMResponse#success().
  LMResponse.error: LMResponse#error.
  LMRequest.model: LMRequest#model.
  LMRequest.prompt: LMRequest#prompt.
  LMRequest.to_dict: LMRequest#to_dict().
  LMRequest.depth: LMRequest#depth.
  LMResponse.to_dict: LMResponse#to_dict().
  LMResponse.error_response: LMResponse#error_response().
  LMResponse.from_dict: LMResponse#from_dict().
  socket_send: socket_send().
  LMRequest.prompts: LMRequest#prompts.
  LMResponse.chat_completions: LMResponse#chat_completions.
  LMResponse.success_response: LMResponse#success_response().
  socket_recv: socket_recv().
  socket_request: socket_request().
  LMResponse.batched_success_response: LMResponse#batched_success_response().
  LMRequest.is_batched: LMRequest#is_batched().
  LMRequest.from_dict: LMRequest#from_dict().
  LMResponse.is_batched: LMResponse#is_batched().
---
# Module: [`rlm/core/comms_utils.py`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py)

## Classes
### `LMRequest`
- def: [`rlm/core/comms_utils.py:22`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L22) — documented in [rlm-core-comms_utils](../../../concepts/rlm-core-comms_utils.md)
- doc: Request message sent to the LM Handler.
- signature: `class LMRequest:`
- members:
  - `from_dict(cls, data: dict)` — [`L51`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L51) — Create from dict.
  - `is_batched(self)` — [`L34`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L34) — Check if this is a batched request.
  - `to_dict(self)` — [`L38`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L38) — Convert to dict, excluding None values.
  - `depth` — [`L31`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L31)
  - `model` — [`L30`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L30)
  - `prompt` — [`L28`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L28)
  - `prompts` — [`L29`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L29)
- used by: [`send_lm_request_batched`](comms_utils.md#send_lm_request_batched), [`_handle_batched`](lm_handler.md#LMRequestHandler._handle_batched), [`_handle_single`](lm_handler.md#LMRequestHandler._handle_single), [`_handle_llm_request`](../environments/daytona_repl.md#DaytonaREPL._handle_llm_request), [`_handle_llm_request`](../environments/modal_repl.md#ModalREPL._handle_llm_request), [`_handle_llm_request`](../environments/prime_repl.md#PrimeREPL._handle_llm_request), [`send_lm_request`](comms_utils.md#send_lm_request), [`_handle_single`](../environments/docker_repl.md#LLMProxyHandler._handle_single), [`_llm_query`](../environments/ipython_repl.md#IPythonREPL._llm_query), [`_llm_query`](../environments/local_repl.md#LocalREPL._llm_query), [`_handle_llm_request`](../environments/e2b_repl.md#E2BREPL._handle_llm_request), [`handle`](lm_handler.md#LMRequestHandler.handle), [`run_all`](lm_handler.md#LMRequestHandler.run_all)  (2 test-only)

### `LMResponse`
- def: [`rlm/core/comms_utils.py:62`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L62) — documented in [rlm-core-comms_utils](../../../concepts/rlm-core-comms_utils.md)
- doc: Response message from the LM Handler.
- signature: `class LMResponse:`
- members:
  - `batched_success_response(cls, chat_completions: list[RLMChatCompletion])` — [`L131`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L131) — Create a successful batched response.
  - `error_response(cls, error: str)` — [`L136`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L136) — Create an error response.
  - `from_dict(cls, data: dict)` — [`L109`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L109) — Create from dict.
  - `is_batched(self)` — [`L78`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L78) — Check if this is a batched response.
  - `success(self)` — [`L73`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L73) — Check if response was successful.
  - `success_response(cls, chat_completion: RLMChatCompletion)` — [`L126`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L126) — Create a successful single response.
  - `to_dict(self)` — [`L82`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L82) — Convert to dict, excluding None values.
  - `chat_completion` — [`L69`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L69)
  - `chat_completions` — [`L70`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L70)
  - `error` — [`L68`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L68)
- uses (calls/refs, reference-scoped): [`RLMChatCompletion`](types.md#RLMChatCompletion), [`to_dict`](types.md#RLMChatCompletion.to_dict), [`from_dict`](types.md#RLMChatCompletion.from_dict)
- used by: [`send_lm_request_batched`](comms_utils.md#send_lm_request_batched), [`_handle_batched`](lm_handler.md#LMRequestHandler._handle_batched), [`_handle_single`](lm_handler.md#LMRequestHandler._handle_single), [`_handle_llm_request`](../environments/daytona_repl.md#DaytonaREPL._handle_llm_request), [`_handle_llm_request`](../environments/modal_repl.md#ModalREPL._handle_llm_request), [`_handle_llm_request`](../environments/prime_repl.md#PrimeREPL._handle_llm_request), [`send_lm_request`](comms_utils.md#send_lm_request), [`_handle_single`](../environments/docker_repl.md#LLMProxyHandler._handle_single), [`_llm_query`](../environments/ipython_repl.md#IPythonREPL._llm_query), [`_llm_query`](../environments/local_repl.md#LocalREPL._llm_query), [`_handle_llm_request`](../environments/e2b_repl.md#E2BREPL._handle_llm_request), [`handle`](lm_handler.md#LMRequestHandler.handle), [`_handle_batched`](../environments/docker_repl.md#LLMProxyHandler._handle_batched), [`_llm_query_batched`](../environments/ipython_repl.md#IPythonREPL._llm_query_batched), [`_llm_query_batched`](../environments/local_repl.md#LocalREPL._llm_query_batched), [`_safe_send`](lm_handler.md#LMRequestHandler._safe_send)  (5 test-only)

## Functions
- `send_lm_request(address: tuple[str, int], request: LMRequest, timeout: int = 300, depth: int | None = None)` — [`L204`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L204) — Send an LM request and return typed response. — documented in [rlm-core-comms_utils](../../../concepts/rlm-core-comms_utils.md)
- `send_lm_request_batched(address: tuple[str, int], prompts: list[str | dict[str, Any]], model: str | None = None, timeout: int = 300, depth: int = 0)` — [`L227`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L227) — Send a batched LM request and return a list of typed responses. — documented in [rlm-core-comms_utils](../../../concepts/rlm-core-comms_utils.md)
- `socket_recv(sock: socket.socket)` — [`L155`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L155) — Receive a length-prefixed JSON message from socket.
- `socket_request(address: tuple[str, int], data: dict, timeout: int = 300)` — [`L179`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L179) — Send a request and receive a response over a new socket connection.
- `socket_send(sock: socket.socket, data: dict)` — [`L146`](../../../../../../raw/code/rlm/rlm/core/comms_utils.py#L146) — Send a length-prefixed JSON message over socket.

