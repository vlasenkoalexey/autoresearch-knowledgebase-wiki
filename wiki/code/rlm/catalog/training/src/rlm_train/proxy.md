---
title: 'Module: training/src/rlm_train/proxy.py'
type: catalog
provenance: extracted
module: training/src/rlm_train/proxy.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `training.src.rlm_train.proxy`/
symbols:
  SubLLMProxy._handle_batched: SubLLMProxy#_handle_batched().
  SubLLMProxy.start: SubLLMProxy#start().
  SubLLMProxy._completion: SubLLMProxy#_completion().
  SubLLMProxy.stop: SubLLMProxy#stop().
  SubLLMProxy._handle_single: SubLLMProxy#_handle_single().
  SubLLMProxy.register: SubLLMProxy#register().
  SubLLMProxy.run_one: SubLLMProxy#run_one().
  SubLLMProxy._handles: SubLLMProxy#_handles.
  logger: logger.
  ClientHandle.record_call: ClientHandle#record_call.
  SubLLMProxy.url: SubLLMProxy#url().
  ClientHandle: ClientHandle#
  SubLLMProxy.unregister: SubLLMProxy#unregister().
  ClientHandle.fake_query: ClientHandle#fake_query.
  ClientHandle.fake_query_batched: ClientHandle#fake_query_batched.
  SubLLMProxy: SubLLMProxy#
  SubLLMProxy._runner: SubLLMProxy#_runner.
  SubLLMProxy._port: SubLLMProxy#_port.
  SubLLMProxy._site: SubLLMProxy#_site.
  SubLLMProxy._semaphores: SubLLMProxy#_semaphores.
  ClientHandle.model: ClientHandle#model.
  ClientHandle.state_ref: ClientHandle#state_ref.
  ClientHandle.client: ClientHandle#client.
  ClientHandle.sampling_args: ClientHandle#sampling_args.
  ClientHandle.max_concurrent: ClientHandle#max_concurrent.
  _maybe_await: _maybe_await().
  SubLLMProxy._host: SubLLMProxy#_host.
  SubLLMProxy._app: SubLLMProxy#_app.
  FakeQuery: FakeQuery.
  FakeQueryBatched: FakeQueryBatched.
  _flatten_prompt: _flatten_prompt().
  _coerce_messages: _coerce_messages().
  SubLLMProxy.__init__: SubLLMProxy#__init__().
  SubLLMProxy._lock: SubLLMProxy#_lock.
---
# Module: [`training/src/rlm_train/proxy.py`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py)

## Classes
### `ClientHandle`
- def: [`training/src/rlm_train/proxy.py:22`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L22)
- signature: `class ClientHandle:`
- members:
  - `client` — [`L23`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L23)
  - `fake_query` — [`L28`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L28)
  - `fake_query_batched` — [`L29`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L29)
  - `max_concurrent` — [`L27`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L27)
  - `model` — [`L24`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L24)
  - `record_call` — [`L26`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L26)
  - `sampling_args` — [`L25`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L25)
  - `state_ref` — [`L30`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L30)
- uses (calls/refs, reference-scoped): [`FakeQuery`](proxy.md#FakeQuery), [`FakeQueryBatched`](proxy.md#FakeQueryBatched)
- used by: [`setup_state`](env.md#RLMTrainEnv.setup_state), [`_handle_batched`](proxy.md#SubLLMProxy._handle_batched), [`_completion`](proxy.md#SubLLMProxy._completion), [`_handle_single`](proxy.md#SubLLMProxy._handle_single), [`register`](proxy.md#SubLLMProxy.register), [`run_one`](proxy.md#SubLLMProxy.run_one), [`_handles`](proxy.md#SubLLMProxy._handles)

### `SubLLMProxy`
- def: [`training/src/rlm_train/proxy.py:82`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L82)
- signature: `class SubLLMProxy:`
- members:
  - `register(self, rollout_id: str, handle: ClientHandle)` — [`L124`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L124)
  - `run_one(p: str)` — [`L193`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L193)
  - `start(self)` — [`L93`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L93) — documented in [training-src-rlm_train-proxy](../../../../concepts/training-src-rlm_train-proxy.md)
  - `stop(self)` — [`L111`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L111) — documented in [training-src-rlm_train-proxy](../../../../concepts/training-src-rlm_train-proxy.md)
  - `unregister(self, rollout_id: str)` — [`L128`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L128)
  - `url(self)` — [`L121`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L121)
- protocol/private: `__init__`[`L83`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L83), `_app`[`L86`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L86), `_completion`[`L212`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L212), `_handle_batched`[`L157`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L157), `_handle_single`[`L132`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L132), `_handles`[`L89`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L89), `_host`[`L84`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L84), `_lock`[`L91`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L91), `_port`[`L85`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L85), `_runner`[`L87`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L87), `_semaphores`[`L90`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L90), `_site`[`L88`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L88)
- uses (calls/refs, reference-scoped): [`logger`](proxy.md#logger), [`record_call`](proxy.md#ClientHandle.record_call), [`ClientHandle`](proxy.md#ClientHandle), [`fake_query`](proxy.md#ClientHandle.fake_query), [`fake_query_batched`](proxy.md#ClientHandle.fake_query_batched), [`model`](proxy.md#ClientHandle.model), [`state_ref`](proxy.md#ClientHandle.state_ref), [`_maybe_await`](proxy.md#_maybe_await), [`client`](proxy.md#ClientHandle.client), [`max_concurrent`](proxy.md#ClientHandle.max_concurrent), [`sampling_args`](proxy.md#ClientHandle.sampling_args), [`_coerce_messages`](proxy.md#_coerce_messages), [`_flatten_prompt`](proxy.md#_flatten_prompt)
- used by: [`setup_state`](env.md#RLMTrainEnv.setup_state), [`_ensure_proxy`](env.md#RLMTrainEnv._ensure_proxy), [`_proxy`](env.md#RLMTrainEnv._proxy), [`_teardown_proxy`](env.md#RLMTrainEnv._teardown_proxy), [`cleanup_rlm`](env.md#RLMTrainEnv.cleanup_rlm)

## Functions
- `_coerce_messages(prompt: str | list)` — [`L62`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L62)
- `_flatten_prompt(prompt: str | list)` — [`L39`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L39)
- `_maybe_await(result: Any)` — [`L33`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L33)

## Module values
- `FakeQuery` — [`L17`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L17)
- `FakeQueryBatched` — [`L18`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L18)
- `logger` — [`L14`](../../../../../../../raw/code/rlm/training/src/rlm_train/proxy.py#L14)

