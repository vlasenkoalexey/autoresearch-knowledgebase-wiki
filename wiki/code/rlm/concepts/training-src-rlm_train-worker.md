---
title: Worker — the sandboxed code-execution process for training rollouts
type: concept
provenance: mixed
concept: training-src-rlm_train-worker
updated: 2026-08-12
status: fresh
---
# Worker — the sandboxed code-execution process for training rollouts

## Overview

`Worker` is the training-time analog of [`LocalREPL`](rlm-environments-local_repl.md): it owns the
`globals`/`locals` namespace a training rollout's generated code executes against, running as its own
`__main__` entry point ([`main`](../catalog/training/src/rlm_train/worker.md#main)) spawned as a subprocess
by [`SubprocessReplBackend`](training-src-rlm_train-repl-subprocess.md).

## Design rationale

**The reserved-name re-injection pattern shows up here too** — [`_restore_scaffold`](../catalog/training/src/rlm_train/worker.md#Worker._restore_scaffold)
re-asserts `_llm_query`, `_llm_query_batched`, and the answer-capture mechanism into the namespace, the same
defensive re-injection [`IPythonREPL._restore_scaffold_in_process`](rlm-environments-ipython_repl.md) does
for the inference-time in-process backend — independently arrived at in two different execution substrates
for the same reason: a model can overwrite a reserved name mid-session, and the scaffold has to survive that.

**`_llm_query`/`_llm_query_batched` reach the model through an HTTP POST to the proxy**, not a direct socket
like [`LMHandler`](rlm-core-lm_handler.md) — `_proxy_post` is the training stack's equivalent client-side
call, talking to [`SubLLMProxy`](training-src-rlm_train-proxy.md) over HTTP rather than the inference
stack's raw socket protocol.

## Entry points
- [`Worker.execute`](../catalog/training/src/rlm_train/worker.md#Worker.execute) — runs one code block with
  a timeout ([`_exec_with_timeout`](../catalog/training/src/rlm_train/worker.md#Worker.execute)), the
  training-loop's counterpart to every inference backend's `execute_code`.

## See also
- [`training-src-rlm_train-repl-subprocess`](training-src-rlm_train-repl-subprocess.md) — the parent process
  that spawns and talks to this worker.
- [`rlm-environments-local_repl`](rlm-environments-local_repl.md) — the closest inference-time analog.
