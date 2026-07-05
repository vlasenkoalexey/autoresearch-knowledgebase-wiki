---
title: 'Module: rdagent/core/utils.py'
type: catalog
provenance: extracted
module: rdagent/core/utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.utils`/
symbols:
  import_class: import_class().
  cache_with_pickle: cache_with_pickle().
  multiprocessing_wrapper: multiprocessing_wrapper().
  SingletonBaseClass: SingletonBaseClass#
  LLM_CACHE_SEED_GEN: LLM_CACHE_SEED_GEN.
  cache_with_pickle.cache_decorator.cache_wrapper: cache_with_pickle().cache_decorator().cache_wrapper().
  CacheSeedGen.set_seed: CacheSeedGen#set_seed().
  SingletonBaseClass.__new__: SingletonBaseClass#__new__().
  CacheSeedGen.__init__: CacheSeedGen#__init__().
  _subprocess_wrapper: _subprocess_wrapper().
  cache_with_pickle.cache_decorator: cache_with_pickle().cache_decorator().
  SingletonBaseClass._instance_dict: SingletonBaseClass#_instance_dict.
  CacheSeedGen.get_next_seed: CacheSeedGen#get_next_seed().
  RDAgentException: RDAgentException#
  CacheSeedGen: CacheSeedGen#
  SingletonBaseClass.__reduce__: SingletonBaseClass#__reduce__().
  parse_json: parse_json().
  similarity: similarity().
---
# Module: [`rdagent/core/utils.py`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py)

## Classes
### `CacheSeedGen`
- def: [`rdagent/core/utils.py:91`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L91)
- doc: It is a global seed generator to generate a sequence of seeds.
- signature: `class CacheSeedGen:`
- members:
  - `get_next_seed(self)` — [`L107`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L107) — generate next random int
  - `set_seed(self, seed: int)` — [`L104`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L104)
- protocol/private: `__init__`[`L101`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L101)
- uses (calls/refs, reference-scoped): [`LLM_SETTINGS`](../oai/llm_conf.md#LLM_SETTINGS), [`init_chat_cache_seed`](../oai/llm_conf.md#LLMSettings.init_chat_cache_seed)
- used by: [`_create_chat_completion_auto_continue`](../oai/backend/base.md#APIBackend._create_chat_completion_auto_continue), [`multiprocessing_wrapper`](utils.md#multiprocessing_wrapper), [`LLM_CACHE_SEED_GEN`](utils.md#LLM_CACHE_SEED_GEN), [`_subprocess_wrapper`](utils.md#_subprocess_wrapper)  (2 test-only)

### `RDAgentException`  ·  implements/extends Exception
- def: [`rdagent/core/utils.py:20`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L20)
- signature: `class RDAgentException(Exception):`
- used by: [`__new__`](utils.md#SingletonBaseClass.__new__)

### `SingletonBaseClass`
- def: [`rdagent/core/utils.py:24`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L24) — documented in [rdagent-log-timer](../../../concepts/rdagent-log-timer.md)
- doc: Because we try to support defining Singleton with `class A(SingletonBaseClass)`
- signature: `class SingletonBaseClass:`
- members:
  - `__reduce__(self)` — [`L47`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L47) — NOTE:
- protocol/private: `__new__`[`L32`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L32), `_instance_dict`[`L30`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L30)
- uses (calls/refs, reference-scoped): [`RDAgentLog`](../log/logger.md#RDAgentLog), [`Prompts`](prompts.md#Prompts), [`RDAgentTimerWrapper`](../log/timer.md#RDAgentTimerWrapper), [`SQliteLazyCache`](../oai/backend/base.md#SQliteLazyCache), [`SessionChatHistoryCache`](../oai/backend/base.md#SessionChatHistoryCache), [`RDAgentException`](utils.md#RDAgentException)  (1 test-only)
- used by: [`RDAgentLog`](../log/logger.md#RDAgentLog), [`Prompts`](prompts.md#Prompts), [`RDAgentTimerWrapper`](../log/timer.md#RDAgentTimerWrapper), [`SQliteLazyCache`](../oai/backend/base.md#SQliteLazyCache), [`SessionChatHistoryCache`](../oai/backend/base.md#SessionChatHistoryCache)  (1 test-only)

## Functions
- `_subprocess_wrapper(f: Callable, seed: int, args: list)` — [`L115`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L115) — It is a function wrapper. To ensure the subprocess has a fixed start seed.
- `cache_decorator(func: Callable)` — [`L176`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L176)
- `cache_with_pickle(hash_func: Callable, post_process_func: Callable | None = None, force: bool = False)` — [`L156`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L156) — This decorator will cache the return value of the function with pickle. — documented in [rdagent-components-coder-factor_coder-factor](../../../concepts/rdagent-components-coder-factor_coder-factor.md)
- `cache_wrapper(*args: Any, **kwargs: Any)` — [`L178`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L178)
- `import_class(class_path: str)` — [`L75`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L75) — Parameters — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- `multiprocessing_wrapper(func_calls: list[tuple[Callable, tuple]], n: int)` — [`L124`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L124) — It will use multiprocessing to call the functions in func_calls with the given parameters.
- `parse_json(response: str)` — [`L58`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L58)
- `similarity(text1: str, text2: str)` — [`L67`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L67)

## Module values
- `LLM_CACHE_SEED_GEN` — [`L112`](../../../../../../raw/code/rd-agent/rdagent/core/utils.py#L112)

