---
title: ModalREPL — separate-machine sandbox via Modal
type: concept
provenance: mixed
concept: rlm-environments-modal_repl
updated: 2026-08-12
status: fresh
---
# ModalREPL — separate-machine sandbox via Modal

## Overview

[`ModalREPL`](../catalog/rlm/environments/modal_repl.md#ModalREPL) is one of the four
[`IsolatedEnv`](rlm-environments-base_env.md) backends — code runs in a Modal Sandbox, a genuinely separate
machine from the caller. It follows the shared isolated-backend shape: a broker server inside the sandbox
(port 8080 by default) exposed via Modal's `encrypted_ports` tunneling, polled by a background thread in
`ModalREPL` itself, which forwards pending requests to the real [`LMHandler`](rlm-core-lm_handler.md) and
posts responses back.

## Design rationale

**Persistence is explicitly unsupported, and the constructor raises rather than silently degrading.**
`__init__` raises `NotImplementedError` immediately if `persistent=True` is passed — a design choice shared
with [`PrimeREPL`](rlm-environments-prime_repl.md) but not with the non-isolated backends, reflecting that
a fresh sandbox per call is the supported model here.

## Entry points
- [`ModalREPL._handle_llm_request`](../catalog/rlm/environments/modal_repl.md#ModalREPL._handle_llm_request) —
  the poller's per-request handler, translating a sandbox-originated LLM call into a real
  [`send_lm_request`](rlm-core-comms_utils.md) call.

## See also
- [`rlm-environments-base_env`](rlm-environments-base_env.md) — the `IsolatedEnv` contract.
- [`rlm-environments-prime_repl`](rlm-environments-prime_repl.md) — the closest structural sibling.
