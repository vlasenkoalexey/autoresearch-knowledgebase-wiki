---
title: 'Module: rlm/environments/base_env.py'
type: catalog
provenance: extracted
module: rlm/environments/base_env.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.environments.base_env`/
symbols:
  IsolatedEnv: IsolatedEnv#
  format_tools_for_prompt: format_tools_for_prompt().
  NonIsolatedEnv: NonIsolatedEnv#
  parse_tool_entry: parse_tool_entry().
  extract_tool_value: extract_tool_value().
  BaseEnv: BaseEnv#
  validate_custom_tools: validate_custom_tools().
  ToolInfo.description: ToolInfo#description.
  BaseEnv.depth: BaseEnv#depth.
  ToolInfo.name: ToolInfo#name.
  IsolatedEnv.execute_code: IsolatedEnv#execute_code().
  SupportsPersistence: SupportsPersistence#
  ToolInfo.value: ToolInfo#value.
  parse_custom_tools: parse_custom_tools().
  RESERVED_TOOL_NAMES.RESERVED_TOOL_NAMES: RESERVED_TOOL_NAMES.RESERVED_TOOL_NAMES.
  IsolatedEnv.setup: IsolatedEnv#setup().
  IsolatedEnv.load_context: IsolatedEnv#load_context().
  NonIsolatedEnv.execute_code: NonIsolatedEnv#execute_code().
  ToolInfo.is_callable: ToolInfo#is_callable().
  BaseEnv.execute_code: BaseEnv#execute_code().
  BaseEnv.max_concurrent_subcalls: BaseEnv#max_concurrent_subcalls.
  NonIsolatedEnv.setup: NonIsolatedEnv#setup().
  NonIsolatedEnv.load_context: NonIsolatedEnv#load_context().
  IsolatedEnv.__init__: IsolatedEnv#__init__().
  ToolInfo: ToolInfo#
  NonIsolatedEnv.__init__: NonIsolatedEnv#__init__().
  BaseEnv.setup: BaseEnv#setup().
  BaseEnv.load_context: BaseEnv#load_context().
  SupportsCustomTools: SupportsCustomTools#
  SupportsPersistence.get_context_count: SupportsPersistence#get_context_count().
  SupportsPersistence.get_history_count: SupportsPersistence#get_history_count().
  BaseEnv.__init__: BaseEnv#__init__().
  SupportsPersistence.add_history: SupportsPersistence#add_history().
  SupportsCustomTools.custom_tools: SupportsCustomTools#custom_tools.
  BaseEnv.persistent: BaseEnv#persistent.
  BaseEnv.kwargs: BaseEnv#kwargs.
  SupportsPersistence.update_handler_address: SupportsPersistence#update_handler_address().
  SupportsPersistence.add_context: SupportsPersistence#add_context().
---
# Module: [`rlm/environments/base_env.py`](../../../../../../raw/code/rlm/rlm/environments/base_env.py)

## Classes
### `BaseEnv`  ·  implements/extends ABC
- def: [`rlm/environments/base_env.py:197`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L197) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: Base REPL-like environment that the RLM uses to interact with. The primary types are isolated and non-isolated,
- signature: `class BaseEnv(ABC):`
- members:
  - `execute_code(self, code: str)` — [`L233`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L233)
  - `load_context(self, context_payload: dict | list | str)` — [`L229`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L229)
  - `setup(self)` — [`L225`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L225)
  - `depth` — [`L220`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L220)
  - `kwargs` — [`L222`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L222)
  - `max_concurrent_subcalls` — [`L221`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L221)
  - `persistent` — [`L219`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L219)
- protocol/private: `__init__`[`L216`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L216)
- uses (calls/refs, reference-scoped): [`REPLResult`](../core/types.md#REPLResult), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`NonIsolatedEnv`](base_env.md#NonIsolatedEnv), [`execute_code`](base_env.md#IsolatedEnv.execute_code), [`execute_code`](base_env.md#NonIsolatedEnv.execute_code), [`load_context`](base_env.md#IsolatedEnv.load_context), [`setup`](base_env.md#IsolatedEnv.setup), [`load_context`](base_env.md#NonIsolatedEnv.load_context), [`setup`](base_env.md#NonIsolatedEnv.setup)
- used by: [`execute_code`](docker_repl.md#DockerREPL.execute_code), [`_spawn_completion_context`](../core/rlm.md#RLM._spawn_completion_context), [`_setup_subprocess`](ipython_repl.md#IPythonREPL._setup_subprocess), [`_completion_turn`](../core/rlm.md#RLM._completion_turn), [`_handle_llm_request`](daytona_repl.md#DaytonaREPL._handle_llm_request), [`_handle_llm_request`](modal_repl.md#ModalREPL._handle_llm_request), [`_handle_llm_request`](prime_repl.md#PrimeREPL._handle_llm_request), [`setup`](docker_repl.md#DockerREPL.setup), [`_llm_query`](ipython_repl.md#IPythonREPL._llm_query), [`_llm_query`](local_repl.md#LocalREPL._llm_query), [`execute_code`](daytona_repl.md#DaytonaREPL.execute_code), [`get_environment`](__init__.md#get_environment), [`execute_code`](modal_repl.md#ModalREPL.execute_code), [`IsolatedEnv`](base_env.md#IsolatedEnv), [`_llm_query_batched`](ipython_repl.md#IPythonREPL._llm_query_batched), [`_llm_query_batched`](local_repl.md#LocalREPL._llm_query_batched), [`execute_code`](prime_repl.md#PrimeREPL.execute_code), [`_rlm_query_batched`](ipython_repl.md#IPythonREPL._rlm_query_batched), [`NonIsolatedEnv`](base_env.md#NonIsolatedEnv), [`_rlm_query_batched`](local_repl.md#LocalREPL._rlm_query_batched), [`_compact_history`](../core/rlm.md#RLM._compact_history), [`__init__`](base_env.md#IsolatedEnv.__init__), [`_env_supports_persistence`](../core/rlm.md#RLM._env_supports_persistence), [`__init__`](base_env.md#NonIsolatedEnv.__init__)  (6 test-only)

### `IsolatedEnv`  ·  implements/extends ABC, BaseEnv
- def: [`rlm/environments/base_env.py:237`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L237) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: These environments (e.g. Prime Envs, Modal Envs) sit on a completely separate machine from the LM,
- signature: `class IsolatedEnv(BaseEnv, ABC):`
- members:
  - `execute_code(self, code: str)` — [`L255`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L255)
  - `load_context(self, context_payload: dict | list | str)` — [`L251`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L251)
  - `setup(self)` — [`L247`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L247)
- protocol/private: `__init__`[`L243`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L243)
- uses (calls/refs, reference-scoped): [`REPLResult`](../core/types.md#REPLResult), [`setup`](prime_repl.md#PrimeREPL.setup), [`setup`](daytona_repl.md#DaytonaREPL.setup), [`setup`](modal_repl.md#ModalREPL.setup), [`execute_code`](daytona_repl.md#DaytonaREPL.execute_code), [`setup`](e2b_repl.md#E2BREPL.setup), [`execute_code`](modal_repl.md#ModalREPL.execute_code), [`execute_code`](prime_repl.md#PrimeREPL.execute_code), [`BaseEnv`](base_env.md#BaseEnv), [`execute_code`](e2b_repl.md#E2BREPL.execute_code), [`ModalREPL`](modal_repl.md#ModalREPL), [`PrimeREPL`](prime_repl.md#PrimeREPL), [`DaytonaREPL`](daytona_repl.md#DaytonaREPL), [`E2BREPL`](e2b_repl.md#E2BREPL), [`load_context`](daytona_repl.md#DaytonaREPL.load_context), [`load_context`](e2b_repl.md#E2BREPL.load_context), [`load_context`](modal_repl.md#ModalREPL.load_context), [`load_context`](prime_repl.md#PrimeREPL.load_context), [`__init__`](base_env.md#BaseEnv.__init__)
- used by: [`BaseEnv`](base_env.md#BaseEnv), [`ModalREPL`](modal_repl.md#ModalREPL), [`PrimeREPL`](prime_repl.md#PrimeREPL), [`execute_code`](base_env.md#BaseEnv.execute_code), [`DaytonaREPL`](daytona_repl.md#DaytonaREPL), [`load_context`](base_env.md#BaseEnv.load_context), [`setup`](base_env.md#BaseEnv.setup), [`E2BREPL`](e2b_repl.md#E2BREPL), [`__init__`](daytona_repl.md#DaytonaREPL.__init__), [`__init__`](e2b_repl.md#E2BREPL.__init__), [`__init__`](modal_repl.md#ModalREPL.__init__), [`__init__`](prime_repl.md#PrimeREPL.__init__)  (2 test-only)

### `NonIsolatedEnv`  ·  implements/extends ABC, BaseEnv
- def: [`rlm/environments/base_env.py:259`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L259) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: These environments run on the same machine as the LM, and provide different levels of isolation
- signature: `class NonIsolatedEnv(BaseEnv, ABC):`
- members:
  - `execute_code(self, code: str)` — [`L278`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L278)
  - `load_context(self, context_payload: dict | list | str)` — [`L274`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L274)
  - `setup(self)` — [`L270`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L270)
- protocol/private: `__init__`[`L266`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L266)
- uses (calls/refs, reference-scoped): [`execute_code`](local_repl.md#LocalREPL.execute_code), [`LocalREPL`](local_repl.md#LocalREPL), [`execute_code`](docker_repl.md#DockerREPL.execute_code), [`execute_code`](ipython_repl.md#IPythonREPL.execute_code), [`IPythonREPL`](ipython_repl.md#IPythonREPL), [`REPLResult`](../core/types.md#REPLResult), [`setup`](docker_repl.md#DockerREPL.setup), [`DockerREPL`](docker_repl.md#DockerREPL), [`BaseEnv`](base_env.md#BaseEnv), [`setup`](ipython_repl.md#IPythonREPL.setup), [`load_context`](docker_repl.md#DockerREPL.load_context), [`load_context`](ipython_repl.md#IPythonREPL.load_context), [`load_context`](local_repl.md#LocalREPL.load_context), [`__init__`](base_env.md#BaseEnv.__init__), [`setup`](local_repl.md#LocalREPL.setup)
- used by: [`LocalREPL`](local_repl.md#LocalREPL), [`IPythonREPL`](ipython_repl.md#IPythonREPL), [`DockerREPL`](docker_repl.md#DockerREPL), [`BaseEnv`](base_env.md#BaseEnv), [`execute_code`](base_env.md#BaseEnv.execute_code), [`__init__`](ipython_repl.md#IPythonREPL.__init__), [`__init__`](docker_repl.md#DockerREPL.__init__), [`__init__`](local_repl.md#LocalREPL.__init__), [`load_context`](base_env.md#BaseEnv.load_context), [`setup`](base_env.md#BaseEnv.setup)  (2 test-only)

### `SupportsCustomTools`  ·  implements/extends Protocol
- def: [`rlm/environments/base_env.py:152`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L152)
- doc: Protocol for environments that support custom tools.
- signature: `class SupportsCustomTools(Protocol):`
- members:
  - `custom_tools` — [`L194`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L194)
- used by: (1 test-only callers)

### `SupportsPersistence`  ·  implements/extends Protocol
- def: [`rlm/environments/base_env.py:283`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L283)
- doc: Protocol for environments that support persistent multi-turn sessions.
- signature: `class SupportsPersistence(Protocol):`
- members:
  - `add_context(self, context_payload: dict | list | str, context_index: int | None = None)` — [`L326`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L326) — Add a context payload, making it available as context_N in code.
  - `add_history(self, message_history: list[dict[str, Any]], history_index: int | None = None)` — [`L356`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L356) — Add a message history, making it available as history_N in code.
  - `get_context_count(self)` — [`L349`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L349) — Return the number of contexts added so far.
  - `get_history_count(self)` — [`L382`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L382) — Return the number of histories added so far.
  - `update_handler_address(self, address: tuple[str, int])` — [`L314`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L314) — Update the LM handler address for nested LLM calls.
- used by: [`completion`](../core/rlm.md#RLM.completion), [`_persistent_env`](../core/rlm.md#RLM._persistent_env), [`_env_supports_persistence`](../core/rlm.md#RLM._env_supports_persistence)  (5 test-only)

### `ToolInfo`
- def: [`rlm/environments/base_env.py:28`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L28) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- doc: Parsed information about a custom tool.
- signature: `class ToolInfo:`
- members:
  - `is_callable(self)` — [`L36`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L36) — Check if the tool value is callable. — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
  - `description` — [`L33`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L33)
  - `name` — [`L31`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L31)
  - `value` — [`L32`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L32)
- used by: [`format_tools_for_prompt`](base_env.md#format_tools_for_prompt), [`parse_tool_entry`](base_env.md#parse_tool_entry), [`parse_custom_tools`](base_env.md#parse_custom_tools)  (7 test-only)

## Functions
- `extract_tool_value(entry: Any)` — [`L81`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L81) — Extract the actual value from a tool entry.
- `format_tools_for_prompt(custom_tools: dict[str, Any] | None)` — [`L96`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L96) — Format custom tools for inclusion in the system prompt. — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- `parse_custom_tools(custom_tools: dict[str, Any] | None)` — [`L66`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L66) — Parse all custom tools into ToolInfo objects. — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- `parse_tool_entry(name: str, entry: Any)` — [`L41`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L41) — Parse a custom tool entry into its components. — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- `validate_custom_tools(custom_tools: dict[str, Any] | None)` — [`L130`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L130) — Validate that custom tools don't override reserved REPL functions.

## Module values
- `RESERVED_TOOL_NAMES` — [`L13`](../../../../../../raw/code/rlm/rlm/environments/base_env.py#L13)

