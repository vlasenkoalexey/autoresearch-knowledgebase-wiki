---
title: 'Module: agents/subagents/utils/context.py'
type: catalog
provenance: extracted
module: agents/subagents/utils/context.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.subagents.utils.context`/
symbols:
  load_subagent_context: load_subagent_context().
  decode_screenshot_base64: decode_screenshot_base64().
  _extract_current_state: _extract_current_state().
  _extract_objective_state: _extract_objective_state().
---
# Module: [`agents/subagents/utils/context.py`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/context.py)

## Functions
- `_extract_current_state(game_state_result: Dict[str, Any])` — [`L23`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/context.py#L23)
- `_extract_objective_state(game_state_result: Dict[str, Any])` — [`L34`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/context.py#L34)
- `decode_screenshot_base64(image_b64: Optional[str])` — [`L14`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/context.py#L14)
- `load_subagent_context(mcp_adapter: Any, run_data_manager: Any, *, last_n_steps: int, include_current_image: bool = True)` — [`L84`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/context.py#L84) — Fetch normalized state for local one-step subagents.

