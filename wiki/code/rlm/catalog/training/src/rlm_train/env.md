---
title: 'Module: training/src/rlm_train/env.py'
type: catalog
provenance: extracted
module: training/src/rlm_train/env.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `training.src.rlm_train.env`/
symbols:
  RLMTrainEnv.setup_state: RLMTrainEnv#setup_state().
  RLMTrainEnv.get_prompt_messages: RLMTrainEnv#get_prompt_messages().
  _pack_exec: _pack_exec().
  RLMTrainEnv._ensure_proxy: RLMTrainEnv#_ensure_proxy().
  RLMTrainEnv._proxy: RLMTrainEnv#_proxy.
  RLMTrainEnv._teardown_proxy: RLMTrainEnv#_teardown_proxy().
  RLMTrainEnv.cleanup_rlm: RLMTrainEnv#cleanup_rlm().
  RLMTrainEnv._build_user_iter: RLMTrainEnv#_build_user_iter().
  RLMTrainEnv.__init__: RLMTrainEnv#__init__().
  RLMTrainEnv._proxy_lock: RLMTrainEnv#_proxy_lock.
  RLMTrainEnv._backend_factory: RLMTrainEnv#_backend_factory.
  RLMTrainEnv._system_prompt: RLMTrainEnv#_system_prompt.
  _format_repl_outputs: _format_repl_outputs().
  _format_one: _format_one().
  _MAX_REPL_OUTPUT_CHARS: _MAX_REPL_OUTPUT_CHARS.
  RLMTrainEnv.teardown_rlm: RLMTrainEnv#teardown_rlm().
  RLMTrainEnv._user_prologue: RLMTrainEnv#_user_prologue.
  RLMTrainEnv._bootstrap_code: RLMTrainEnv#_bootstrap_code.
  _normalize_for_api: _normalize_for_api().
  logger: logger.
  RLMTrainEnv: RLMTrainEnv#
  RLMTrainEnv._max_iterations: RLMTrainEnv#_max_iterations.
  RLMTrainEnv._sub_model: RLMTrainEnv#_sub_model.
  RLMTrainEnv._sub_sampling_args: RLMTrainEnv#_sub_sampling_args.
  RLMTrainEnv._orchestrator: RLMTrainEnv#_orchestrator.
  RLMTrainEnv._sub_llm_fn: RLMTrainEnv#_sub_llm_fn.
  RLMTrainEnv._sub_llm_fn_batched: RLMTrainEnv#_sub_llm_fn_batched.
  _last_assistant: _last_assistant().
  _msg_text: _msg_text().
  RLMTrainEnv.env_response: RLMTrainEnv#env_response().
  RLMTrainEnv.has_final_answer: RLMTrainEnv#has_final_answer().
---
# Module: [`training/src/rlm_train/env.py`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py)

## Classes
### `RLMTrainEnv`
- def: [`training/src/rlm_train/env.py:31`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L31)
- signature: `class RLMTrainEnv(vf.MultiTurnEnv):`
- members:
  - `cleanup_rlm(self, state: State)` — [`L229`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L229)
  - `env_response(self, messages: Messages, state: State, **kwargs: Any)` — [`L221`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L221)
  - `get_prompt_messages(self, state: State)` — [`L163`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L163) — documented in [training-src-rlm_train-env](../../../../concepts/training-src-rlm_train-env.md)
  - `has_final_answer(self, state: State)` — [`L225`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L225)
  - `setup_state(self, state: State)` — [`L100`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L100) — documented in [training-src-rlm_train-env](../../../../concepts/training-src-rlm_train-env.md)
  - `teardown_rlm(self)` — [`L242`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L242)
- protocol/private: `__init__`[`L32`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L32), `_backend_factory`[`L54`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L54), `_bootstrap_code`[`L63`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L63), `_build_user_iter`[`L84`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L84), `_ensure_proxy`[`L67`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L67), `_max_iterations`[`L55`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L55), `_orchestrator`[`L59`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L59), `_proxy`[`L64`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L64), `_proxy_lock`[`L65`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L65), `_sub_llm_fn`[`L61`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L61), `_sub_llm_fn_batched`[`L62`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L62), `_sub_model`[`L56`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L56), `_sub_sampling_args`[`L57`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L57), `_system_prompt`[`L58`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L58), `_teardown_proxy`[`L77`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L77), `_user_prologue`[`L60`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L60)
- uses (calls/refs, reference-scoped): [`start`](proxy.md#SubLLMProxy.start), [`build_rlm_system_prompt`](../../../rlm/utils/prompts.md#build_rlm_system_prompt), [`_pack_exec`](env.md#_pack_exec), [`stop`](proxy.md#SubLLMProxy.stop), [`find_code_blocks`](../../../rlm/utils/parsing.md#find_code_blocks), [`build_user_prompt`](../../../rlm/utils/prompts.md#build_user_prompt), [`register`](proxy.md#SubLLMProxy.register), [`QueryMetadata`](../../../rlm/core/types.md#QueryMetadata), [`ReplBackend`](repl/base.md#ReplBackend), [`execute`](repl/base.md#ReplBackend.execute), [`record_call`](proxy.md#ClientHandle.record_call), [`url`](proxy.md#SubLLMProxy.url), [`SubprocessReplBackend`](repl/subprocess.md#SubprocessReplBackend), [`ClientHandle`](proxy.md#ClientHandle), [`RLM_SYSTEM_PROMPT`](../../../rlm/utils/prompts.md#RLM_SYSTEM_PROMPT), [`bootstrap`](repl/base.md#ReplBackend.bootstrap), [`unregister`](proxy.md#SubLLMProxy.unregister), [`fake_query`](proxy.md#ClientHandle.fake_query), [`fake_query_batched`](proxy.md#ClientHandle.fake_query_batched), [`SubLLMProxy`](proxy.md#SubLLMProxy), [`final_answer`](repl/base.md#ExecResult.final_answer), [`_format_repl_outputs`](env.md#_format_repl_outputs), [`load_context`](repl/base.md#ReplBackend.load_context), [`start`](repl/base.md#ReplBackend.start), [`RLMTrainRubric`](rubric.md#RLMTrainRubric), [`model`](proxy.md#ClientHandle.model), [`state_ref`](proxy.md#ClientHandle.state_ref), [`_normalize_for_api`](env.md#_normalize_for_api), [`client`](proxy.md#ClientHandle.client), [`sampling_args`](proxy.md#ClientHandle.sampling_args), [`_last_assistant`](env.md#_last_assistant), [`_msg_text`](env.md#_msg_text), [`logger`](env.md#logger)

## Functions
- `_format_one(o: dict[str, Any])` — [`L322`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L322)
- `_format_repl_outputs(outputs: list[dict[str, Any]])` — [`L310`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L310)
- `_last_assistant(completion: Any)` — [`L274`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L274)
- `_msg_text(msg: Any)` — [`L286`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L286)
- `_normalize_for_api(msgs: list)` — [`L246`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L246)
- `_pack_exec(code: str, result: ExecResult)` — [`L300`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L300) — documented in [training-src-rlm_train-env](../../../../concepts/training-src-rlm_train-env.md)

## Module values
- `_MAX_REPL_OUTPUT_CHARS` — [`L28`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L28)
- `logger` — [`L26`](../../../../../../../raw/code/rlm/training/src/rlm_train/env.py#L26)

