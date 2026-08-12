---
title: SubprocessReplBackend — the training environment's worker-process bridge
type: concept
provenance: mixed
concept: training-src-rlm_train-repl-subprocess
updated: 2026-08-12
status: fresh
---
# SubprocessReplBackend — the training environment's worker-process bridge

## Overview

`SubprocessReplBackend` spawns and talks to a [`Worker`](training-src-rlm_train-worker.md) subprocess,
functioning as the training-time equivalent of [`IPythonREPL`](rlm-environments-ipython_repl.md)'s
subprocess kernel mode — genuine process isolation for the code a training rollout generates, with a
line-based request/response protocol (`_request`, `_send`, `_read_line`) rather than Jupyter's kernel
protocol.

## Design rationale

**Startup failures and protocol violations are distinct, explicitly-typed errors** —
`WorkerStartupError` (the subprocess didn't come up within `_startup_timeout`) versus `WorkerProtocolError`
(a malformed response from an already-running worker) — so a caller can distinguish "the sandbox never
started" from "the sandbox is misbehaving," which matters for a training loop deciding whether to retry a
rollout or treat it as a hard failure.

## Entry points
- [`SubprocessReplBackend.start`](../catalog/training/src/rlm_train/repl/subprocess.md#SubprocessReplBackend.start) —
  spawns the worker subprocess and waits for it to signal readiness, with a bounded startup timeout.
- [`SubprocessReplBackend.execute`](../catalog/training/src/rlm_train/repl/subprocess.md#SubprocessReplBackend.execute) —
  sends code to the worker and returns an `ExecResult` — the training-loop's `REPLResult` equivalent.

## See also
- [`training-src-rlm_train-worker`](training-src-rlm_train-worker.md) — the subprocess this backend manages.
- [`rlm-environments-ipython_repl`](rlm-environments-ipython_repl.md) — the closest inference-time analog
  (subprocess kernel mode).
