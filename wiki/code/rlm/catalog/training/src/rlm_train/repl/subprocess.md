---
title: 'Module: training/src/rlm_train/repl/subprocess.py'
type: catalog
provenance: extracted
module: training/src/rlm_train/repl/subprocess.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `training.src.rlm_train.repl.subprocess`/
symbols:
  SubprocessReplBackend.start: SubprocessReplBackend#start().
  SubprocessReplBackend._proc: SubprocessReplBackend#_proc.
  SubprocessReplBackend._request: SubprocessReplBackend#_request().
  SubprocessReplBackend.execute: SubprocessReplBackend#execute().
  SubprocessReplBackend.stop: SubprocessReplBackend#stop().
  SubprocessReplBackend._read_line: SubprocessReplBackend#_read_line().
  WorkerProtocolError: WorkerProtocolError#
  SubprocessReplBackend: SubprocessReplBackend#
  SubprocessReplBackend._stderr_task: SubprocessReplBackend#_stderr_task.
  SubprocessReplBackend._drain_stderr: SubprocessReplBackend#_drain_stderr().
  SubprocessReplBackend._stderr_buf: SubprocessReplBackend#_stderr_buf.
  SubprocessReplBackend._send: SubprocessReplBackend#_send().
  SubprocessReplBackend._stderr_text: SubprocessReplBackend#_stderr_text().
  SubprocessReplBackend._kill_worker: SubprocessReplBackend#_kill_worker().
  SubprocessReplBackend.load_context: SubprocessReplBackend#load_context().
  SubprocessReplBackend.bootstrap: SubprocessReplBackend#bootstrap().
  WorkerStartupError: WorkerStartupError#
  SubprocessReplBackend._startup_timeout: SubprocessReplBackend#_startup_timeout.
  SubprocessReplBackend._request_timeout: SubprocessReplBackend#_request_timeout.
  SubprocessReplBackend._req_counter: SubprocessReplBackend#_req_counter.
  SubprocessReplBackend._STREAM_LIMIT: SubprocessReplBackend#_STREAM_LIMIT.
  SubprocessReplBackend._python: SubprocessReplBackend#_python.
  SubprocessReplBackend._worker_module: SubprocessReplBackend#_worker_module.
  SubprocessReplBackend._lock: SubprocessReplBackend#_lock.
  SubprocessReplBackend.__init__: SubprocessReplBackend#__init__().
---
# Module: [`training/src/rlm_train/repl/subprocess.py`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py)

## Classes
### `SubprocessReplBackend`  ·  implements/extends ReplBackend
- def: [`training/src/rlm_train/repl/subprocess.py:22`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L22)
- signature: `class SubprocessReplBackend(ReplBackend):`
- members:
  - `bootstrap(self, code: str)` — [`L107`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L107)
  - `execute(self, code: str)` — [`L112`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L112) — documented in [training-src-rlm_train-repl-subprocess](../../../../../concepts/training-src-rlm_train-repl-subprocess.md)
  - `load_context(self, payload: Any, index: int | None = None)` — [`L103`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L103)
  - `start(self, proxy_url: str, rollout_id: str, depth: int = 1)` — [`L42`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L42) — documented in [training-src-rlm_train-repl-subprocess](../../../../../concepts/training-src-rlm_train-repl-subprocess.md)
  - `stop(self)` — [`L73`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L73)
- protocol/private: `_STREAM_LIMIT`[`L23`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L23), `__init__`[`L25`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L25), `_drain_stderr`[`L173`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L173), `_kill_worker`[`L144`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L144), `_lock`[`L38`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L38), `_proc`[`L36`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L36), `_python`[`L32`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L32), `_read_line`[`L162`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L162), `_req_counter`[`L37`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L37), `_request`[`L122`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L122), `_request_timeout`[`L35`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L35), `_send`[`L156`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L156), `_startup_timeout`[`L34`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L34), `_stderr_buf`[`L40`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L40), `_stderr_task`[`L39`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L39), `_stderr_text`[`L184`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L184), `_worker_module`[`L33`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L33)
- uses (calls/refs, reference-scoped): [`ReplBackend`](base.md#ReplBackend), [`ExecResult`](base.md#ExecResult), [`WorkerProtocolError`](subprocess.md#WorkerProtocolError), [`final_answer`](base.md#ExecResult.final_answer), [`WorkerStartupError`](subprocess.md#WorkerStartupError), [`locals_keys`](base.md#ExecResult.locals_keys), [`stderr`](base.md#ExecResult.stderr), [`stdout`](base.md#ExecResult.stdout), [`execution_time`](base.md#ExecResult.execution_time)
- used by: [`ReplBackend`](base.md#ReplBackend), [`execute`](base.md#ReplBackend.execute), [`bootstrap`](base.md#ReplBackend.bootstrap), [`_backend_factory`](../env.md#RLMTrainEnv._backend_factory), [`load_context`](base.md#ReplBackend.load_context), [`start`](base.md#ReplBackend.start), [`stop`](base.md#ReplBackend.stop)

### `WorkerProtocolError`  ·  implements/extends RuntimeError
- def: [`training/src/rlm_train/repl/subprocess.py:18`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L18)
- signature: `class WorkerProtocolError(RuntimeError):`
- used by: [`_request`](subprocess.md#SubprocessReplBackend._request), [`stop`](subprocess.md#SubprocessReplBackend.stop), [`_read_line`](subprocess.md#SubprocessReplBackend._read_line)

### `WorkerStartupError`  ·  implements/extends RuntimeError
- def: [`training/src/rlm_train/repl/subprocess.py:14`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/subprocess.py#L14)
- signature: `class WorkerStartupError(RuntimeError):`
- used by: [`start`](subprocess.md#SubprocessReplBackend.start)

