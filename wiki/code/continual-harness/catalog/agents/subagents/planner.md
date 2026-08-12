---
title: 'Module: agents/subagents/planner.py'
type: catalog
provenance: extracted
module: agents/subagents/planner.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.subagents.planner`/
symbols:
  PLANNER_SAFETY_CAP: PLANNER_SAFETY_CAP.
  REPLAN_OBJECTIVES_TOOL_DECLARATION.REPLAN_OBJECTIVES_TOOL_DECLARATION: REPLAN_OBJECTIVES_TOOL_DECLARATION.REPLAN_OBJECTIVES_TOOL_DECLARATION.
  allowed_planner_tool_names: allowed_planner_tool_names().
  format_planner_history: format_planner_history().
  build_planner_prompt: build_planner_prompt().
  PLANNER_HISTORY_CAP: PLANNER_HISTORY_CAP.
  format_full_objective_sequence: format_full_objective_sequence().
---
# Module: [`agents/subagents/planner.py`](../../../../../../raw/code/continual-harness/agents/subagents/planner.py)

## Functions
- `allowed_planner_tool_names()` — [`L16`](../../../../../../raw/code/continual-harness/agents/subagents/planner.py#L16)
- `build_planner_prompt(*, reason: str, objective_sequence: str, current_state_text: str, location: str, progress: Dict[str, Any], memory_summary: str, skill_overview: str = "", planner_history: str, handoff_summary: str, turn_index: int)` — [`L183`](../../../../../../raw/code/continual-harness/agents/subagents/planner.py#L183)
- `format_full_objective_sequence(snapshot: Dict[str, Any])` — [`L105`](../../../../../../raw/code/continual-harness/agents/subagents/planner.py#L105) — Format the full objective sequence snapshot for inclusion in the planner prompt.
- `format_planner_history(history: List[Dict[str, Any]])` — [`L156`](../../../../../../raw/code/continual-harness/agents/subagents/planner.py#L156) — Format the planner's short-term memory, analogous to format_battler_history.

## Module values
- `PLANNER_HISTORY_CAP` — [`L13`](../../../../../../raw/code/continual-harness/agents/subagents/planner.py#L13)
- `PLANNER_SAFETY_CAP` — [`L12`](../../../../../../raw/code/continual-harness/agents/subagents/planner.py#L12)
- `REPLAN_OBJECTIVES_TOOL_DECLARATION` — [`L20`](../../../../../../raw/code/continual-harness/agents/subagents/planner.py#L20)

