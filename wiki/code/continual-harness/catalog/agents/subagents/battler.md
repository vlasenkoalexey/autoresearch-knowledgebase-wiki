---
title: 'Module: agents/subagents/battler.py'
type: catalog
provenance: extracted
module: agents/subagents/battler.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.subagents.battler`/
symbols:
  allowed_battler_tool_names: allowed_battler_tool_names().
  build_battler_prompt: build_battler_prompt().
  format_battler_history: format_battler_history().
  extract_key_events_from_summary: extract_key_events_from_summary().
---
# Module: [`agents/subagents/battler.py`](../../../../../../raw/code/continual-harness/agents/subagents/battler.py)

## Functions
- `allowed_battler_tool_names()` — [`L12`](../../../../../../raw/code/continual-harness/agents/subagents/battler.py#L12)
- `build_battler_prompt(*, current_state_text: str, location: str, objective_state: Dict[str, Any], progress: Dict[str, Any], memory_summary: str, skill_overview: str = "", handoff_summary: str, battle_history: str, turn_index: int)` — [`L43`](../../../../../../raw/code/continual-harness/agents/subagents/battler.py#L43)
- `extract_key_events_from_summary(summary_text: str)` — [`L91`](../../../../../../raw/code/continual-harness/agents/subagents/battler.py#L91)
- `format_battler_history(history: List[Dict[str, Any]])` — [`L16`](../../../../../../raw/code/continual-harness/agents/subagents/battler.py#L16) — Format the battler's inner turn history, analogous to the orchestrator's short-term memory.

