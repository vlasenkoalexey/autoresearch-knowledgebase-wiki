---
title: comms_utils — the request/response wire format
type: concept
provenance: mixed
concept: rlm-core-comms_utils
updated: 2026-08-12
status: fresh
---
# comms_utils — the request/response wire format

## Overview

`rlm.core.comms_utils` defines the two dataclasses that cross the socket boundary between an environment
backend and [`LMHandler`](rlm-core-lm_handler.md) — [`LMRequest`](../catalog/rlm/core/comms_utils.md#LMRequest)
and [`LMResponse`](../catalog/rlm/core/comms_utils.md#LMResponse) — plus the client-side helper functions,
[`send_lm_request`](../catalog/rlm/core/comms_utils.md#send_lm_request) and
[`send_lm_request_batched`](../catalog/rlm/core/comms_utils.md#send_lm_request_batched), that every
isolated-backend's request handler (`_handle_llm_request` on `DaytonaREPL`, `ModalREPL`, `PrimeREPL`, and
`LLMProxyHandler` on `DockerREPL`) calls into to actually reach the handler.

## Diagram

```mermaid
flowchart LR
    A["sandbox request dict"] --> B["_handle_llm_request<br/>(Daytona/Modal/Prime/Docker)"]
    B --> C["send_lm_request / send_lm_request_batched"]
    C -->|socket to (host,port)| D["LMHandler.LMRequestHandler"]
    D --> C
    C --> B
    B --> A2["response dict back into sandbox"]
```

## Design rationale (why it's built this way)

**A common client-side helper means every isolated backend implements the same three lines**, not four
subtly different socket clients. `DaytonaREPL._handle_llm_request`, `ModalREPL._handle_llm_request`, and
`PrimeREPL._handle_llm_request` all follow the identical shape: parse the sandbox's request dict, build an
[`LMRequest`](../catalog/rlm/core/comms_utils.md#LMRequest), call `send_lm_request` or
`send_lm_request_batched`, and translate the typed `LMResponse` back into a plain dict the sandbox-side code
can consume. Centralizing that translation here is what keeps four otherwise-independent broker
implementations (see [`rlm-environments-base_env`](rlm-environments-base_env.md)) from drifting apart on
wire format.

**Success and error are both first-class response shapes, not exceptions crossing a process boundary.**
Both helpers construct an `error_response`/`success_response` explicitly rather than letting a socket
exception propagate — a network hiccup or a client-side error on one sub-call becomes data in the response,
consistent with the batched-partial-failure design in [`rlm-core-lm_handler`](rlm-core-lm_handler.md).

## Entry points
- [`send_lm_request`](../catalog/rlm/core/comms_utils.md#send_lm_request) /
  [`send_lm_request_batched`](../catalog/rlm/core/comms_utils.md#send_lm_request_batched) — the two
  functions every isolated backend's LLM-request handler calls.

## Mechanism (step-by-step)
1. A sandbox-side handler — [`DaytonaREPL._handle_llm_request`](../catalog/rlm/environments/daytona_repl.md#DaytonaREPL._handle_llm_request),
   [`ModalREPL._handle_llm_request`](../catalog/rlm/environments/modal_repl.md#ModalREPL._handle_llm_request),
   or [`PrimeREPL._handle_llm_request`](../catalog/rlm/environments/prime_repl.md#PrimeREPL._handle_llm_request) —
   receives a raw request dict from inside the sandbox (the model's generated code calling
   `llm_query`/`rlm_query`).
2. It's wrapped into an [`LMRequest`](../catalog/rlm/core/comms_utils.md#LMRequest) and passed to
   `send_lm_request`/`send_lm_request_batched`, which opens a socket connection to the handler's `(host,
   port)`, serializes the request (`to_dict`), and blocks (with a `timeout`, default 300s) for the reply.
3. The handler's response is deserialized (`from_dict`) back into a typed
   [`LMResponse`](../catalog/rlm/core/comms_utils.md#LMResponse) carrying a `chat_completion` field.
4. The calling backend's [`_handle_llm_request`](../catalog/rlm/environments/daytona_repl.md#DaytonaREPL._handle_llm_request)
   (or its Modal/Prime counterpart above) converts that back into a plain dict for the sandbox.

## Key data structures
- [`LMRequest`](../catalog/rlm/core/comms_utils.md#LMRequest) — prompt(s), optional model, depth.
- [`LMResponse`](../catalog/rlm/core/comms_utils.md#LMResponse) — `chat_completion` (an `RLMChatCompletion`)
  on success, or an error field on failure.

## Edge cases
- `depth` is threaded through explicitly on both the request and the handler dispatch path — this is how a
  sandboxed sub-call correctly reports which recursion depth it's operating at, independent of what the
  sandbox itself might infer.

## See also
- [`rlm-core-lm_handler`](rlm-core-lm_handler.md) — the server side of this protocol.
- [`rlm-environments-base_env`](rlm-environments-base_env.md) — the isolated backends that are this
  protocol's clients.
