---
title: 'Module: rlm/core/lm_handler.py'
type: catalog
provenance: extracted
module: rlm/core/lm_handler.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.core.lm_handler`/
symbols:
  LMRequestHandler._handle_batched: LMRequestHandler#_handle_batched().
  LMRequestHandler._handle_single: LMRequestHandler#_handle_single().
  LMHandler: LMHandler#
  LMRequestHandler.handle: LMRequestHandler#handle().
  LMHandler.address: LMHandler#address().
  LMHandler.start: LMHandler#start().
  LMHandler.get_usage_summary: LMHandler#get_usage_summary().
  LMHandler.get_client: LMHandler#get_client().
  LMHandler._server: LMHandler#_server.
  LMRequestHandler._safe_send: LMRequestHandler#_safe_send().
  LMHandler.register_client: LMHandler#register_client().
  LMHandler.port: LMHandler#port().
  LMHandler.completion: LMHandler#completion().
  LMHandler.stop: LMHandler#stop().
  LMHandler.clients: LMHandler#clients.
  LMHandler.batch_max_concurrent: LMHandler#batch_max_concurrent.
  LMRequestHandler.run_all: LMRequestHandler#run_all().
  LMHandler.other_backend_client: LMHandler#other_backend_client.
  LMHandler.host: LMHandler#host.
  LMRequestHandler.run_one: LMRequestHandler#run_one().
  LMHandler._thread: LMHandler#_thread.
  LMHandler.__init__: LMHandler#__init__().
  LMHandler.__enter__: LMHandler#__enter__().
  LMHandler.__exit__: LMHandler#__exit__().
  ThreadingLMServer: ThreadingLMServer#
  LMHandler.default_client: LMHandler#default_client.
  LMHandler._port: LMHandler#_port.
  LMRequestHandler: LMRequestHandler#
  ThreadingLMServer.daemon_threads: ThreadingLMServer#daemon_threads.
  ThreadingLMServer.allow_reuse_address: ThreadingLMServer#allow_reuse_address.
---
# Module: [`rlm/core/lm_handler.py`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py)

## Classes
### `LMHandler`
- def: [`rlm/core/lm_handler.py:145`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L145) — documented in [rlm-core-lm_handler](../../../concepts/rlm-core-lm_handler.md)
- members:
  - `address(self)` — [`L201`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L201) — Get (host, port) tuple for connecting.
  - `completion(self, prompt: str, model: str | None = None)` — [`L225`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L225) — Direct completion call (for main process use).
  - `get_client(self, model: str | None = None, depth: int = 0)` — [`L176`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L176) — Get client by model name or depth, or return default. — documented in [rlm-core-lm_handler](../../../concepts/rlm-core-lm_handler.md)
  - `get_usage_summary(self)` — [`L237`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L237) — Get the usage summary for all clients, merged into a single dict.
  - `port(self)` — [`L194`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L194) — Get the actual port (useful when auto-assigned).
  - `register_client(self, model_name: str, client: BaseLM)` — [`L172`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L172) — Register a client for a specific model name.
  - `start(self)` — [`L205`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L205) — Start the socket server in a background thread. Returns (host, port).
  - `stop(self)` — [`L218`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L218) — Stop the socket server.
  - `batch_max_concurrent` — [`L168`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L168)
  - `clients` — [`L163`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L163)
  - `default_client` — [`L161`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L161)
  - `host` — [`L164`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L164)
  - `other_backend_client` — [`L162`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L162)
- protocol/private: `__enter__`[`L229`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L229), `__exit__`[`L233`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L233), `__init__`[`L153`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L153), `_port`[`L167`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L167), `_server`[`L165`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L165), `_thread`[`L166`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L166)
- uses (calls/refs, reference-scoped): [`UsageSummary`](types.md#UsageSummary), [`BaseLM`](../clients/base_lm.md#BaseLM), [`model_usage_summaries`](types.md#UsageSummary.model_usage_summaries), [`get_usage_summary`](../clients/base_lm.md#BaseLM.get_usage_summary), [`completion`](../clients/base_lm.md#BaseLM.completion), [`model_name`](../clients/base_lm.md#BaseLM.model_name), [`ThreadingLMServer`](lm_handler.md#ThreadingLMServer), [`LMRequestHandler`](lm_handler.md#LMRequestHandler)
- used by: [`completion`](rlm.md#RLM.completion), [`_spawn_completion_context`](rlm.md#RLM._spawn_completion_context), [`_check_iteration_limits`](rlm.md#RLM._check_iteration_limits), [`_handle_batched`](lm_handler.md#LMRequestHandler._handle_batched), [`_handle_single`](lm_handler.md#LMRequestHandler._handle_single), [`_completion_turn`](rlm.md#RLM._completion_turn), [`handle`](lm_handler.md#LMRequestHandler.handle), [`_default_answer`](rlm.md#RLM._default_answer), [`_compact_history`](rlm.md#RLM._compact_history)  (11 test-only)

### `LMRequestHandler`  ·  implements/extends StreamRequestHandler
- def: [`rlm/core/lm_handler.py:17`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L17)
- doc: Socket handler for LLM completion requests.
- signature: `class LMRequestHandler(StreamRequestHandler):`
- members:
  - `_handle_batched(self, request: LMRequest, handler: LMHandler)` — [`L82`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L82) — Handle a batched prompts request using async for concurrency. — documented in [rlm-core-lm_handler](../../../concepts/rlm-core-lm_handler.md)
  - `_handle_single(self, request: LMRequest, handler: LMHandler)` — [`L61`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L61) — Handle a single prompt request. — documented in [rlm-core-lm_handler](../../../concepts/rlm-core-lm_handler.md)
  - `_safe_send(self, response: LMResponse)` — [`L52`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L52) — Send response, returning False if the socket is broken.
  - `handle(self)` — [`L20`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L20) — documented in [rlm-core-lm_handler](../../../concepts/rlm-core-lm_handler.md)
  - `run_all()` — [`L94`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L94)
  - `run_one(prompt: str)` — [`L90`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L90)
- uses (calls/refs, reference-scoped): [`response`](types.md#RLMChatCompletion.response), [`RLMChatCompletion`](types.md#RLMChatCompletion), [`UsageSummary`](types.md#UsageSummary), [`model_usage_summaries`](types.md#UsageSummary.model_usage_summaries), [`get_last_usage`](../clients/base_lm.md#BaseLM.get_last_usage), [`completion`](../clients/base_lm.md#BaseLM.completion), [`usage_summary`](types.md#RLMChatCompletion.usage_summary), [`LMHandler`](lm_handler.md#LMHandler), [`execution_time`](types.md#RLMChatCompletion.execution_time), [`acompletion`](../clients/base_lm.md#BaseLM.acompletion), [`LMRequest`](comms_utils.md#LMRequest), [`LMResponse`](comms_utils.md#LMResponse), [`prompt`](types.md#RLMChatCompletion.prompt), [`root_model`](types.md#RLMChatCompletion.root_model), [`model`](comms_utils.md#LMRequest.model), [`get_client`](lm_handler.md#LMHandler.get_client), [`prompt`](comms_utils.md#LMRequest.prompt), [`depth`](comms_utils.md#LMRequest.depth), [`to_dict`](comms_utils.md#LMResponse.to_dict), [`error_response`](comms_utils.md#LMResponse.error_response), [`socket_send`](comms_utils.md#socket_send), [`prompts`](comms_utils.md#LMRequest.prompts), [`model_name`](../clients/base_lm.md#BaseLM.model_name), [`socket_recv`](comms_utils.md#socket_recv), [`success_response`](comms_utils.md#LMResponse.success_response), [`batch_max_concurrent`](lm_handler.md#LMHandler.batch_max_concurrent), [`batched_success_response`](comms_utils.md#LMResponse.batched_success_response), [`error`](types.md#RLMChatCompletion.error), [`from_dict`](comms_utils.md#LMRequest.from_dict), [`is_batched`](comms_utils.md#LMRequest.is_batched)
- used by: [`start`](lm_handler.md#LMHandler.start)

### `ThreadingLMServer`  ·  implements/extends ThreadingTCPServer
- def: [`rlm/core/lm_handler.py:138`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L138)
- doc: Multi-threaded TCP server for LM requests.
- signature: `class ThreadingLMServer(ThreadingTCPServer):`
- members:
  - `allow_reuse_address` — [`L142`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L142)
  - `daemon_threads` — [`L141`](../../../../../../raw/code/rlm/rlm/core/lm_handler.py#L141)
- used by: [`start`](lm_handler.md#LMHandler.start), [`_server`](lm_handler.md#LMHandler._server)

