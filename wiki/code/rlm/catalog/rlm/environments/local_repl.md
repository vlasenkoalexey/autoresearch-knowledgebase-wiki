---
title: 'Module: rlm/environments/local_repl.py'
type: catalog
provenance: extracted
module: rlm/environments/local_repl.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.environments.local_repl`/
symbols:
  LocalREPL.execute_code: LocalREPL#execute_code().
  LocalREPL.locals: LocalREPL#locals.
  LocalREPL: LocalREPL#
  LocalREPL.cleanup: LocalREPL#cleanup().
  LocalREPL._restore_scaffold: LocalREPL#_restore_scaffold().
  LocalREPL._llm_query: LocalREPL#_llm_query().
  LocalREPL._last_final_answer: LocalREPL#_last_final_answer.
  LocalREPL._llm_query_batched: LocalREPL#_llm_query_batched().
  LocalREPL.add_context: LocalREPL#add_context().
  LocalREPL._rlm_query_batched: LocalREPL#_rlm_query_batched().
  LocalREPL.globals: LocalREPL#globals.
  LocalREPL.add_history: LocalREPL#add_history().
  LocalREPL._compaction_history: LocalREPL#_compaction_history.
  LocalREPL._rlm_query: LocalREPL#_rlm_query().
  LocalREPL._pending_llm_calls: LocalREPL#_pending_llm_calls.
  LocalREPL.custom_sub_tools: LocalREPL#custom_sub_tools.
  _AnswerDict: _AnswerDict#
  LocalREPL.lm_handler_address: LocalREPL#lm_handler_address.
  LocalREPL._run_subcall: LocalREPL#_run_subcall().
  LocalREPL.get_context_count: LocalREPL#get_context_count().
  LocalREPL.get_history_count: LocalREPL#get_history_count().
  LocalREPL.__init__: LocalREPL#__init__().
  LocalREPL.subcall_fn: LocalREPL#subcall_fn.
  LocalREPL.temp_dir: LocalREPL#temp_dir.
  LocalREPL.append_compaction_entry: LocalREPL#append_compaction_entry().
  LocalREPL._capture_answer: LocalREPL#_capture_answer().
  LocalREPL._show_vars: LocalREPL#_show_vars().
  LocalREPL._context_count: LocalREPL#_context_count.
  LocalREPL._history_count: LocalREPL#_history_count.
  LocalREPL.load_context: LocalREPL#load_context().
  LocalREPL.update_handler_address: LocalREPL#update_handler_address().
  LocalREPL._capture_output: LocalREPL#_capture_output().
  LocalREPL._temp_cwd: LocalREPL#_temp_cwd().
  LocalREPL.compaction: LocalREPL#compaction.
  LocalREPL.custom_tools: LocalREPL#custom_tools.
  _AnswerDict.__setitem__: _AnswerDict#__setitem__().
  LocalREPL.__exit__: LocalREPL#__exit__().
  LocalREPL.__del__: LocalREPL#__del__().
  _AnswerDict._on_ready: _AnswerDict#_on_ready.
  _SAFE_BUILTINS: _SAFE_BUILTINS.
  LocalREPL._lock: LocalREPL#_lock.
  LocalREPL.setup: LocalREPL#setup().
  _AnswerDict.__init__: _AnswerDict#__init__().
  LocalREPL.original_cwd: LocalREPL#original_cwd.
  LocalREPL.__enter__: LocalREPL#__enter__().
---
# Module: [`rlm/environments/local_repl.py`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py)

## Classes
### `LocalREPL`  ·  implements/extends NonIsolatedEnv
- def: [`rlm/environments/local_repl.py:147`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L147) — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)
- doc: Local REPL environment with persistent Python namespace.
- signature: `class LocalREPL(NonIsolatedEnv):`
- members:
  - `_capture_output(self)` — [`L493`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L493) — Thread-safe context manager to capture stdout/stderr.
  - `_llm_query(self, prompt: str, model: str | None = None)` — [`L258`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L258) — Query the LM with a single plain completion (no REPL, no recursion).
  - `_llm_query_batched(self, prompts: list[str], model: str | None = None)` — [`L282`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L282) — Query the LM with multiple prompts concurrently (no REPL, no recursion).
  - `_restore_scaffold(self)` — [`L514`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L514) — Restore scaffold names after execution so overwrites (e.g. context = 'x') don't persist.
  - `_rlm_query(self, prompt: str, model: str | None = None)` — [`L313`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L313) — Spawn a recursive RLM sub-call for deeper thinking on a subtask.
  - `_rlm_query_batched(self, prompts: list[str], model: str | None = None)` — [`L335`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L335) — Spawn recursive RLM sub-calls for multiple prompts in parallel.
  - `_show_vars(self)` — [`L247`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L247) — Show all available variables in the REPL environment.
  - `_temp_cwd(self)` — [`L505`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L505) — Temporarily change to temp directory for execution.
  - `add_context(self, context_payload: dict | list | str, context_index: int | None = None)` — [`L403`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L403) — Add a context with versioned variable name.
  - `add_history(self, message_history: list[dict[str, Any]], history_index: int | None = None)` — [`L449`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L449) — Store a conversation's message history as a versioned variable.
  - `append_compaction_entry(self, entry: list[dict[str, Any]] | dict[str, Any])` — [`L481`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L481) — Append a trajectory segment or a summary to the compaction history.
  - `cleanup(self)` — [`L592`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L592) — Clean up temp directory and reset state.
  - `execute_code(self, code: str)` — [`L547`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L547) — Execute code in the persistent namespace and return result. — documented in [rlm-environments-local_repl](../../../concepts/rlm-environments-local_repl.md)
  - `get_context_count(self)` — [`L445`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L445) — Return the number of contexts loaded.
  - `get_history_count(self)` — [`L477`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L477) — Return the number of conversation histories stored.
  - `load_context(self, context_payload: dict | list | str)` — [`L399`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L399) — Load context into the environment as context_0 (and 'context' alias).
  - `setup(self)` — [`L208`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L208) — Setup the environment.
  - `update_handler_address(self, address: tuple[str, int])` — [`L441`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L441) — Update the LM handler address for a new completion call.
  - `compaction` — [`L181`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L181)
  - `custom_sub_tools` — [`L186`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L186)
  - `custom_tools` — [`L184`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L184)
  - `globals` — [`L211`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L211)
  - `lm_handler_address` — [`L174`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L174)
  - `locals` — [`L215`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L215)
  - `original_cwd` — [`L176`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L176)
  - `subcall_fn` — [`L175`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L175)
  - `temp_dir` — [`L177`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L177)
- protocol/private: `__del__`[`L603`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L603), `__enter__`[`L585`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L585), `__exit__`[`L588`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L588), `__init__`[`L153`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L153), `_capture_answer`[`L244`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L244), `_compaction_history`[`L197`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L197), `_context_count`[`L179`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L179), `_history_count`[`L180`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L180), `_last_final_answer`[`L220`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L220), `_lock`[`L178`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L178), `_pending_llm_calls`[`L218`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L218), `_run_subcall`[`L372`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L372)
- uses (calls/refs, reference-scoped): [`response`](../core/types.md#RLMChatCompletion.response), [`RLMChatCompletion`](../core/types.md#RLMChatCompletion), [`REPLResult`](../core/types.md#REPLResult), [`send_lm_request_batched`](../core/comms_utils.md#send_lm_request_batched), [`chat_completion`](../core/comms_utils.md#LMResponse.chat_completion), [`send_lm_request`](../core/comms_utils.md#send_lm_request), [`LMRequest`](../core/comms_utils.md#LMRequest), [`success`](../core/comms_utils.md#LMResponse.success), [`error`](../core/comms_utils.md#LMResponse.error), [`NonIsolatedEnv`](base_env.md#NonIsolatedEnv), [`extract_tool_value`](base_env.md#extract_tool_value), [`validate_custom_tools`](base_env.md#validate_custom_tools), [`depth`](base_env.md#BaseEnv.depth), [`model`](../core/comms_utils.md#LMRequest.model), [`prompt`](../core/comms_utils.md#LMRequest.prompt), [`RESERVED_TOOL_NAMES`](base_env.md#RESERVED_TOOL_NAMES.RESERVED_TOOL_NAMES), [`depth`](../core/comms_utils.md#LMRequest.depth), [`max_concurrent_subcalls`](base_env.md#BaseEnv.max_concurrent_subcalls), [`_AnswerDict`](local_repl.md#_AnswerDict), [`__init__`](base_env.md#NonIsolatedEnv.__init__), [`_SAFE_BUILTINS`](local_repl.md#_SAFE_BUILTINS)
- used by: [`get_environment`](__init__.md#get_environment), [`NonIsolatedEnv`](base_env.md#NonIsolatedEnv), [`execute_code`](base_env.md#NonIsolatedEnv.execute_code), [`load_context`](base_env.md#NonIsolatedEnv.load_context), [`setup`](base_env.md#NonIsolatedEnv.setup)  (101 test-only)

### `_AnswerDict`  ·  implements/extends dict
- def: [`rlm/environments/local_repl.py:26`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L26)
- doc: REPL-visible dict where `answer["ready"] = True` signals completion.
- signature: `class _AnswerDict(dict):`
- protocol/private: `__init__`[`L35`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L35), `__setitem__`[`L41`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L41), `_on_ready`[`L39`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L39)
- used by: [`_restore_scaffold`](local_repl.md#LocalREPL._restore_scaffold), [`_restore_scaffold_in_process`](ipython_repl.md#IPythonREPL._restore_scaffold_in_process), [`_last_final_answer`](local_repl.md#LocalREPL._last_final_answer), [`_setup_in_process`](ipython_repl.md#IPythonREPL._setup_in_process)

## Module values
- `_SAFE_BUILTINS` — [`L55`](../../../../../../raw/code/rlm/rlm/environments/local_repl.py#L55)

