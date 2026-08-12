---
title: DockerREPL — container-isolated, same-machine REPL
type: concept
provenance: mixed
concept: rlm-environments-docker_repl
updated: 2026-08-12
status: fresh
---
# DockerREPL — container-isolated, same-machine REPL

## Overview

`DockerREPL` runs model-generated code inside a
Docker container (`python:3.11-slim` by default) rather than a bare subprocess or kernel — still a
[`NonIsolatedEnv`](rlm-environments-base_env.md) by this repo's taxonomy (same machine) but with real process
and filesystem isolation from the caller, one step short of the fully separate-machine `IsolatedEnv`
backends.

## Design rationale

**LLM calls reach out of the container via a local HTTP proxy**, not a direct socket — `self.proxy_server`
(a `ThreadingHTTPServer`) and `self.proxy_thread` run alongside the container, and the container's own
`LLMProxyHandler._handle_single`/`_handle_batched` forward requests through it to the real
[`LMHandler`](rlm-core-lm_handler.md), mirroring the isolated backends' broker-and-forward pattern even
though this backend doesn't strictly need it (it's on the same machine) — the tradeoff of picking Docker
isolation is that the container can't just dial back into the parent process directly.

**Persistence uses versioned context/history snapshots, not a shared live namespace.** The docstring
describes `context_N`/`history_N` bookkeeping reused across `completion()` calls for `persistent=True`
sessions — the container and its `dill`-serialized state stay alive for the environment's lifetime, and each
call layers a new version on top rather than mutating one shared namespace in place, which is a different
persistence strategy than `LocalREPL`'s direct namespace reuse.

## Entry points
- [`DockerREPL.execute_code`](../catalog/rlm/environments/docker_repl.md#DockerREPL.execute_code) —
  implements the `BaseEnv` contract by running code inside the container.
- [`DockerREPL.setup`](../catalog/rlm/environments/docker_repl.md#DockerREPL.setup) — provisions the
  container and generates the in-container injection code for custom tools (see
  [`rlm-environments-base_env`](rlm-environments-base_env.md) for the shared custom-tools mechanism this
  implements per-backend).

## See also
- [`rlm-environments-base_env`](rlm-environments-base_env.md) — the shared abstraction.
- [`rlm-core-comms_utils`](rlm-core-comms_utils.md) — the request/response types this backend's proxy
  translates.
