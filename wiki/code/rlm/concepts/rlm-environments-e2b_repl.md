---
title: E2BREPL — separate-machine sandbox via E2B
type: concept
provenance: mixed
concept: rlm-environments-e2b_repl
updated: 2026-08-12
status: fresh
---
# E2BREPL — separate-machine sandbox via E2B

## Overview

`E2BREPL` is the fifth [`IsolatedEnv`](rlm-environments-base_env.md)
backend, running code in an E2B sandbox — one of five interchangeable separate-machine execution targets
(alongside Modal, Prime, Daytona) that all satisfy the same `BaseEnv` contract and the same
broker-and-poll bridge back to [`LMHandler`](rlm-core-lm_handler.md). Its presence alongside four other
sandbox providers for the identical isolation tier is itself evidence of the design choice
[`rlm-environments-base_env`](rlm-environments-base_env.md) documents: the environment abstraction is
deliberately provider-agnostic, so adding a new sandbox vendor is an additional `IsolatedEnv` subclass, not
a change to `RLM` or `LMHandler`.

## See also
- [`rlm-environments-base_env`](rlm-environments-base_env.md) — the `IsolatedEnv` contract every sandbox
  backend, including this one, implements identically from the caller's perspective.
