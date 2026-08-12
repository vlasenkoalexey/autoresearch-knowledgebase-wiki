---
title: 'Module: training/src/rlm_train/worker.py'
type: catalog
provenance: extracted
module: training/src/rlm_train/worker.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `training.src.rlm_train.worker`/
symbols:
  Worker._restore_scaffold: Worker#_restore_scaffold().
  Worker._setup_namespace: Worker#_setup_namespace().
  Worker.execute: Worker#execute().
  Worker.locals: Worker#locals.
  Worker.globals: Worker#globals.
  main: main().
  _send: _send().
  Worker._llm_query: Worker#_llm_query().
  Worker._llm_query_batched: Worker#_llm_query_batched().
  Worker._proxy_post: Worker#_proxy_post().
  Worker.load_context: Worker#load_context().
  Worker._exec_with_timeout: Worker#_exec_with_timeout().
  Worker._last_final_answer: Worker#_last_final_answer.
  Worker._capture_answer: Worker#_capture_answer().
  Worker._show_vars: Worker#_show_vars().
  Worker._capture_output: Worker#_capture_output().
  _AnswerDict: _AnswerDict#
  Worker._context_count: Worker#_context_count.
  _AnswerDict.__setitem__: _AnswerDict#__setitem__().
  _AnswerDict._on_ready: _AnswerDict#_on_ready.
  Worker.depth: Worker#depth.
  _SAFE_BUILTINS: _SAFE_BUILTINS.
  RESERVED_TOOL_NAMES: RESERVED_TOOL_NAMES.
  Worker: Worker#
  Worker.proxy_url: Worker#proxy_url.
  Worker.rollout_id: Worker#rollout_id.
  Worker.exec_timeout_s: Worker#exec_timeout_s.
  Worker._lock: Worker#_lock.
  Worker._on_alarm: Worker#_on_alarm().
  _AnswerDict.__init__: _AnswerDict#__init__().
  Worker.__init__: Worker#__init__().
---
# Module: [`training/src/rlm_train/worker.py`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py)

## Classes
### `Worker`
- def: [`training/src/rlm_train/worker.py:137`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L137)
- signature: `class Worker:`
- members:
  - `execute(self, code: str)` — [`L309`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L309) — documented in [training-src-rlm_train-worker](../../../../concepts/training-src-rlm_train-worker.md)
  - `load_context(self, payload: Any, index: int | None = None)` — [`L271`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L271)
  - `depth` — [`L147`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L147)
  - `exec_timeout_s` — [`L153`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L153)
  - `globals` — [`L157`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L157)
  - `locals` — [`L158`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L158)
  - `proxy_url` — [`L145`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L145)
  - `rollout_id` — [`L146`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L146)
- protocol/private: `__init__`[`L138`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L138), `_capture_answer`[`L196`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L196), `_capture_output`[`L282`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L282), `_context_count`[`L156`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L156), `_exec_with_timeout`[`L292`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L292), `_last_final_answer`[`L155`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L155), `_llm_query`[`L235`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L235), `_llm_query_batched`[`L248`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L248), `_lock`[`L154`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L154), `_on_alarm`[`L298`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L298), `_proxy_post`[`L209`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L209), `_restore_scaffold`[`L171`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L171), `_setup_namespace`[`L161`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L161), `_show_vars`[`L199`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L199)
- uses (calls/refs, reference-scoped): [`_AnswerDict`](worker.md#_AnswerDict), [`RESERVED_TOOL_NAMES`](worker.md#RESERVED_TOOL_NAMES), [`_SAFE_BUILTINS`](worker.md#_SAFE_BUILTINS)
- used by: [`main`](worker.md#main)

### `_AnswerDict`  ·  implements/extends dict
- def: [`training/src/rlm_train/worker.py:121`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L121)
- signature: `class _AnswerDict(dict):`
- protocol/private: `__init__`[`L122`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L122), `__setitem__`[`L128`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L128), `_on_ready`[`L126`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L126)
- used by: [`_restore_scaffold`](worker.md#Worker._restore_scaffold), [`_setup_namespace`](worker.md#Worker._setup_namespace)

## Functions
- `_send(obj: dict[str, Any])` — [`L345`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L345)
- `main()` — [`L351`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L351) — documented in [training-src-rlm_train-worker](../../../../concepts/training-src-rlm_train-worker.md)

## Module values
- `RESERVED_TOOL_NAMES` — [`L107`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L107)
- `_SAFE_BUILTINS` — [`L19`](../../../../../../../raw/code/rlm/training/src/rlm_train/worker.py#L19)

