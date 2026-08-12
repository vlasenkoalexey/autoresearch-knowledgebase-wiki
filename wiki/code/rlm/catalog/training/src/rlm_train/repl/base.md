---
title: 'Module: training/src/rlm_train/repl/base.py'
type: catalog
provenance: extracted
module: training/src/rlm_train/repl/base.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `training.src.rlm_train.repl.base`/
symbols:
  ReplBackend: ReplBackend#
  ExecResult: ExecResult#
  ReplBackend.execute: ReplBackend#execute().
  ReplBackend.bootstrap: ReplBackend#bootstrap().
  ExecResult.final_answer: ExecResult#final_answer.
  ReplBackend.start: ReplBackend#start().
  ReplBackend.load_context: ReplBackend#load_context().
  ReplBackend.stop: ReplBackend#stop().
  ExecResult.stdout: ExecResult#stdout.
  ExecResult.stderr: ExecResult#stderr.
  ExecResult.locals_keys: ExecResult#locals_keys.
  ExecResult.execution_time: ExecResult#execution_time.
---
# Module: [`training/src/rlm_train/repl/base.py`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py)

## Classes
### `ExecResult`
- def: [`training/src/rlm_train/repl/base.py:9`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L9)
- signature: `class ExecResult:`
- members:
  - `execution_time` — [`L13`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L13)
  - `final_answer` — [`L12`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L12)
  - `locals_keys` — [`L14`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L14)
  - `stderr` — [`L11`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L11)
  - `stdout` — [`L10`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L10)
- used by: [`get_prompt_messages`](../env.md#RLMTrainEnv.get_prompt_messages), [`execute`](subprocess.md#SubprocessReplBackend.execute), [`_pack_exec`](../env.md#_pack_exec), [`execute`](base.md#ReplBackend.execute)

### `ReplBackend`  ·  implements/extends ABC
- def: [`training/src/rlm_train/repl/base.py:17`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L17)
- signature: `class ReplBackend(ABC):`
- members:
  - `bootstrap(self, code: str)` — [`L30`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L30)
  - `execute(self, code: str)` — [`L25`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L25)
  - `load_context(self, payload: Any, index: int | None = None)` — [`L22`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L22)
  - `start(self, proxy_url: str, rollout_id: str, depth: int = 1)` — [`L19`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L19)
  - `stop(self)` — [`L28`](../../../../../../../../raw/code/rlm/training/src/rlm_train/repl/base.py#L28)
- uses (calls/refs, reference-scoped): [`start`](subprocess.md#SubprocessReplBackend.start), [`execute`](subprocess.md#SubprocessReplBackend.execute), [`stop`](subprocess.md#SubprocessReplBackend.stop), [`ExecResult`](base.md#ExecResult), [`SubprocessReplBackend`](subprocess.md#SubprocessReplBackend), [`bootstrap`](subprocess.md#SubprocessReplBackend.bootstrap), [`load_context`](subprocess.md#SubprocessReplBackend.load_context)
- used by: [`setup_state`](../env.md#RLMTrainEnv.setup_state), [`get_prompt_messages`](../env.md#RLMTrainEnv.get_prompt_messages), [`SubprocessReplBackend`](subprocess.md#SubprocessReplBackend), [`__init__`](../env.md#RLMTrainEnv.__init__)

