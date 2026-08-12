---
title: 'Module: agents/subagents/utils/executor.py'
type: catalog
provenance: extracted
module: agents/subagents/utils/executor.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.subagents.utils.executor`/
symbols:
  SubagentExecutor.run_generic_loop: SubagentExecutor#run_generic_loop().
  SubagentExecutor._execute_custom_subagent_inner: SubagentExecutor#_execute_custom_subagent_inner().
  SubagentExecutor._process_trajectory_history_inner: SubagentExecutor#_process_trajectory_history_inner().
  SubagentExecutor.execute_custom_subagent: SubagentExecutor#execute_custom_subagent().
  SubagentExecutor.process_trajectory_history: SubagentExecutor#process_trajectory_history().
  logger: logger.
  MAX_CONSECUTIVE_FAILURES: MAX_CONSECUTIVE_FAILURES.
  SubagentExecutor: SubagentExecutor#
  SubagentExecutor.runtime: SubagentExecutor#runtime.
  SubagentExecutor._get_run_data_manager: SubagentExecutor#_get_run_data_manager.
  SubagentExecutor._get_subagent_vlm: SubagentExecutor#_get_subagent_vlm.
  SubagentExecutor._extract_text: SubagentExecutor#_extract_text.
  SubagentExecutor.llm_logger: SubagentExecutor#llm_logger.
  SubagentExecutor.mcp_adapter: SubagentExecutor#mcp_adapter.
  SubagentExecutor.server_url: SubagentExecutor#server_url.
  SubagentExecutor._handle_vlm_function_calls: SubagentExecutor#_handle_vlm_function_calls.
  SubagentExecutor._log_trajectory: SubagentExecutor#_log_trajectory.
  SubagentExecutor.prompt_builder: SubagentExecutor#prompt_builder().
  SubagentExecutor.on_turn_complete: SubagentExecutor#on_turn_complete().
  SubagentExecutor.should_continue: SubagentExecutor#should_continue().
  SubagentExecutor.__init__: SubagentExecutor#__init__().
  SubagentExecutor._wait_for_actions: SubagentExecutor#_wait_for_actions.
---
# Module: [`agents/subagents/utils/executor.py`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py)

## Classes
### `SubagentExecutor`
- def: [`agents/subagents/utils/executor.py:32`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L32)
- doc: Runs generic and custom subagent loops on behalf of PokeAgent.
- signature: `class SubagentExecutor:`
- members:
  - `execute_custom_subagent(self, arguments: dict)` — [`L223`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L223) — Launch a custom subagent from the registry or with an inline config.
  - `on_turn_complete(turn: int, reasoning: str, tool_calls: List[Dict])` — [`L379`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L379)
  - `process_trajectory_history(self, arguments: dict)` — [`L423`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L423) — One-step VLM analysis on a trajectory window with a custom directive.
  - `prompt_builder(context: Dict[str, Any], turn_index: int, history: List[Dict[str, Any]])` — [`L330`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L330)
  - `run_generic_loop(self, *, vlm, prompt_builder: Callable[[Dict[str, Any], int, List[Dict[str, Any]]], str], allowed_tool_names: Set[str], safety_cap: int, owner: str, interaction_name: str, should_continue_fn: Optional[Callable[[Dict[str, Any], int], bool]] = None, on_turn_complete_fn: Optional[Callable[[int, str, List[Dict[str, Any]]], None]] = None)` — [`L79`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L79) — Core subagent loop used by battler, planner, and custom subagents.
  - `should_continue(context: Dict, turn: int)` — [`L397`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L397)
  - `llm_logger` — [`L72`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L72)
  - `mcp_adapter` — [`L65`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L65)
  - `runtime` — [`L64`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L64)
  - `server_url` — [`L67`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L67)
- protocol/private: `__init__`[`L50`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L50), `_execute_custom_subagent_inner`[`L231`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L231), `_extract_text`[`L70`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L70), `_get_run_data_manager`[`L66`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L66), `_get_subagent_vlm`[`L68`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L68), `_handle_vlm_function_calls`[`L69`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L69), `_log_trajectory`[`L71`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L71), `_process_trajectory_history_inner`[`L431`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L431), `_wait_for_actions`[`L73`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L73)
- uses (calls/refs, reference-scoped): [`get`](../../../utils/stores/base_store.md#BaseStore.get), [`load_subagent_context`](context.md#load_subagent_context), [`format_trajectory_window`](trajectory_window.md#format_trajectory_window), [`update_server_metrics`](../../../utils/metric_tracking/server_metrics.md#update_server_metrics), [`get_subagent_store`](../../../utils/stores/subagents.md#get_subagent_store), [`load_trajectory_range`](trajectory_window.md#load_trajectory_range), [`name`](../../../utils/stores/subagents.md#SubagentEntry.name), [`logger`](executor.md#logger), [`MAX_CONSECUTIVE_FAILURES`](executor.md#MAX_CONSECUTIVE_FAILURES), [`available_tools`](../../../utils/stores/subagents.md#SubagentEntry.available_tools), [`SUBAGENT_FORBIDDEN_TOOLS`](registry.md#SUBAGENT_FORBIDDEN_TOOLS.SUBAGENT_FORBIDDEN_TOOLS), [`max_turns`](../../../utils/stores/subagents.md#SubagentEntry.max_turns), [`directive`](../../../utils/stores/subagents.md#SubagentEntry.directive), [`return_condition`](../../../utils/stores/subagents.md#SubagentEntry.return_condition), [`system_instructions`](../../../utils/stores/subagents.md#SubagentEntry.system_instructions)
- used by: [`executor`](../../PokeAgent.md#PokeAgent.executor), [`_execute_custom_subagent`](../../PokeAgent.md#PokeAgent._execute_custom_subagent), [`_execute_process_trajectory_history`](../../PokeAgent.md#PokeAgent._execute_process_trajectory_history)  (17 test-only)

## Module values
- `MAX_CONSECUTIVE_FAILURES` — [`L25`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L25)
- `logger` — [`L23`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/executor.py#L23)

