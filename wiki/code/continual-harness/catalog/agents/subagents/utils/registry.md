---
title: 'Module: agents/subagents/utils/registry.py'
type: catalog
provenance: extracted
module: agents/subagents/utils/registry.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.subagents.utils.registry`/
symbols:
  LOCAL_SUBAGENT_SPECS: LOCAL_SUBAGENT_SPECS.
  build_local_subagent_tool_declarations: build_local_subagent_tool_declarations().
  _EMERALD_PUZZLE_SPEC: _EMERALD_PUZZLE_SPEC.
  _RED_PUZZLE_SPEC: _RED_PUZZLE_SPEC.
  LocalSubagentSpec.tool_name: LocalSubagentSpec#tool_name.
  LocalSubagentSpec: LocalSubagentSpec#
  LocalSubagentSpec.handler_method: LocalSubagentSpec#handler_method.
  LocalSubagentSpec.description: LocalSubagentSpec#description.
  LocalSubagentSpec.parameters: LocalSubagentSpec#parameters.
  get_local_subagent_spec: get_local_subagent_spec().
  LocalSubagentSpec.handler_type: LocalSubagentSpec#handler_type.
  LocalSubagentSpec.interaction_name: LocalSubagentSpec#interaction_name.
  BATTLE_ALLOWED_TOOL_NAMES: BATTLE_ALLOWED_TOOL_NAMES.
  PLANNER_ALLOWED_TOOL_NAMES: PLANNER_ALLOWED_TOOL_NAMES.
  BUILTIN_SUBAGENT_TOOL_NAMES.BUILTIN_SUBAGENT_TOOL_NAMES: BUILTIN_SUBAGENT_TOOL_NAMES.BUILTIN_SUBAGENT_TOOL_NAMES.
  is_local_subagent_tool: is_local_subagent_tool().
  LOCAL_SUBAGENT_SPEC_BY_NAME: LOCAL_SUBAGENT_SPEC_BY_NAME.
  _puzzle_tool_name: _puzzle_tool_name().
  SUBAGENT_FORBIDDEN_TOOLS.SUBAGENT_FORBIDDEN_TOOLS: SUBAGENT_FORBIDDEN_TOOLS.SUBAGENT_FORBIDDEN_TOOLS.
  LocalSubagentSpec.allowed_tool_names: LocalSubagentSpec#allowed_tool_names.
  _is_red: _is_red().
---
# Module: [`agents/subagents/utils/registry.py`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py)

## Classes
### `LocalSubagentSpec`
- def: [`agents/subagents/utils/registry.py:11`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L11)
- signature: `class LocalSubagentSpec:`
- members:
  - `allowed_tool_names` — [`L18`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L18)
  - `description` — [`L16`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L16)
  - `handler_method` — [`L15`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L15)
  - `handler_type` — [`L13`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L13)
  - `interaction_name` — [`L14`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L14)
  - `parameters` — [`L17`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L17)
  - `tool_name` — [`L12`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L12)
- used by: [`LOCAL_SUBAGENT_SPECS`](registry.md#LOCAL_SUBAGENT_SPECS), [`_execute_function_call`](../../PokeAgent.md#PokeAgent._execute_function_call), [`_execute_function_call_by_name`](../../PokeAgent.md#PokeAgent._execute_function_call_by_name), [`build_tools_for_scaffold`](../../tools/registry.md#build_tools_for_scaffold), [`build_local_subagent_tool_declarations`](registry.md#build_local_subagent_tool_declarations), [`_EMERALD_PUZZLE_SPEC`](registry.md#_EMERALD_PUZZLE_SPEC), [`_RED_PUZZLE_SPEC`](registry.md#_RED_PUZZLE_SPEC), [`get_local_subagent_spec`](registry.md#get_local_subagent_spec), [`LOCAL_SUBAGENT_SPEC_BY_NAME`](registry.md#LOCAL_SUBAGENT_SPEC_BY_NAME)  (1 test-only)

## Functions
- `_is_red()` — [`L21`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L21)
- `_puzzle_tool_name()` — [`L25`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L25)
- `build_local_subagent_tool_declarations(include_builtins: bool = True)` — [`L469`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L469) — Build tool declarations for all registered local subagents. — documented in [agents-subagents-utils-registry](../../../../concepts/agents-subagents-utils-registry.md)
- `get_local_subagent_spec(tool_name: str)` — [`L461`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L461)
- `is_local_subagent_tool(tool_name: str)` — [`L465`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L465)

## Module values
- `BATTLE_ALLOWED_TOOL_NAMES` — [`L29`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L29)
- `BUILTIN_SUBAGENT_TOOL_NAMES` — [`L60`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L60)
- `LOCAL_SUBAGENT_SPECS` — [`L123`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L123)
- `LOCAL_SUBAGENT_SPEC_BY_NAME` — [`L458`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L458)
- `PLANNER_ALLOWED_TOOL_NAMES` — [`L40`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L40)
- `SUBAGENT_FORBIDDEN_TOOLS` — [`L57`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L57)
- `_EMERALD_PUZZLE_SPEC` — [`L71`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L71)
- `_RED_PUZZLE_SPEC` — [`L96`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/registry.py#L96)

