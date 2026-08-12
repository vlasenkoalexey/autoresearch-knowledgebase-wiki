---
title: PrimeREPL — separate-machine sandbox via Prime Intellect's own infrastructure
type: concept
provenance: mixed
concept: rlm-environments-prime_repl
updated: 2026-08-12
status: fresh
---
# PrimeREPL — separate-machine sandbox via Prime Intellect's own infrastructure

## Overview

`PrimeREPL` is the [`IsolatedEnv`](rlm-environments-base_env.md)
backend running code in Prime Intellect's own sandbox product — notable because the RLM paper's first
author, Alex Zhang, is now a Prime Intellect research fellow (see
[Recursive Language Models](../../../sources/recursive-language-models.md)), making this the backend most
directly tied to where the paper's ideas ended up shipping as a product
([Prime Agent](../../../sources/prime-agent-launch.md)). Structurally it mirrors
[`ModalREPL`](rlm-environments-modal_repl.md): a broker server (port 8888 default) exposed via
`sandboxes.expose()`, polled by `PrimeREPL` and bridged to the real
[`LMHandler`](rlm-core-lm_handler.md).

## Design rationale

Like `ModalREPL`, `persistent=True` raises `NotImplementedError` in the constructor rather than silently
falling back — both separate-machine backends treat persistence as genuinely unsupported rather than
best-effort. `network_access` is an explicit constructor flag (default `True`), a control surface the
non-isolated backends don't need since they don't sandbox network access at all.

## Entry points
- [`PrimeREPL._handle_llm_request`](../catalog/rlm/environments/prime_repl.md#PrimeREPL._handle_llm_request) —
  identical shape to `ModalREPL`'s handler: translate a polled sandbox request into a real
  [`send_lm_request`](rlm-core-comms_utils.md) call.

## See also
- [`rlm-environments-base_env`](rlm-environments-base_env.md) — the `IsolatedEnv` contract.
- [`rlm-environments-modal_repl`](rlm-environments-modal_repl.md) — the closest structural sibling.
