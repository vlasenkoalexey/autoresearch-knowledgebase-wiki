---
title: DaytonaREPL — separate-machine sandbox via Daytona
type: concept
provenance: mixed
concept: rlm-environments-daytona_repl
updated: 2026-08-12
status: fresh
---
# DaytonaREPL — separate-machine sandbox via Daytona

## Overview

`DaytonaREPL` is the fourth
[`IsolatedEnv`](rlm-environments-base_env.md) backend, running code in a Daytona sandbox. It follows the same
broker-and-poll shape as [`ModalREPL`](rlm-environments-modal_repl.md) and
[`PrimeREPL`](rlm-environments-prime_repl.md), with one structural difference: rather than injecting custom
tools via a separate step after setup, [`_build_exec_script`](../catalog/rlm/environments/daytona_repl.md#_build_exec_script)
generates one self-contained script per execution that includes state-persistence bookkeeping and custom-tool
injection together, executed as a unit inside the sandbox.

## Entry points
- [`DaytonaREPL._handle_llm_request`](../catalog/rlm/environments/daytona_repl.md#DaytonaREPL._handle_llm_request) —
  the same LLM-request-forwarding shape shared by every isolated backend.

## See also
- [`rlm-environments-base_env`](rlm-environments-base_env.md) — the `IsolatedEnv` contract.
- [`rlm-environments-modal_repl`](rlm-environments-modal_repl.md), [`rlm-environments-prime_repl`](rlm-environments-prime_repl.md) —
  structural siblings.
