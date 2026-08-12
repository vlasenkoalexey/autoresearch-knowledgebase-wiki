---
title: 'Module: agents/subagents/utils/trajectory_window.py'
type: catalog
provenance: extracted
module: agents/subagents/utils/trajectory_window.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.subagents.utils.trajectory_window`/
symbols:
  load_recent_trajectories: load_recent_trajectories().
  format_trajectory_window: format_trajectory_window().
  clamp_trajectory_window: clamp_trajectory_window().
  load_trajectory_range: load_trajectory_range().
  resolve_trajectory_path: resolve_trajectory_path().
  MAX_TRAJECTORY_WINDOW: MAX_TRAJECTORY_WINDOW.
  read_last_jsonl_lines: read_last_jsonl_lines().
  DEFAULT_TRAJECTORY_WINDOW: DEFAULT_TRAJECTORY_WINDOW.
  _trajectory_file_for_run: _trajectory_file_for_run().
  _read_last_jsonl_lines: _read_last_jsonl_lines().
  logger: logger.
  _format_coords: _format_coords().
  _summarize_action: _summarize_action().
  _summarize_outcome: _summarize_outcome().
---
# Module: [`agents/subagents/utils/trajectory_window.py`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py)

## Functions
- `_format_coords(snapshot: Dict[str, Any])` — [`L176`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L176)
- `_read_last_jsonl_lines(path: Path, max_lines: int)` — [`L105`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L105) — Backward-compatible alias for older callsites/tests.
- `_summarize_action(action: Any)` — [`L183`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L183)
- `_summarize_outcome(outcome: Any)` — [`L191`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L191)
- `_trajectory_file_for_run(run_data_manager: Any = None)` — [`L54`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L54) — Backward-compatible alias for legacy callsites/tests.
- `clamp_trajectory_window(last_n_steps: Optional[int])` — [`L18`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L18) — Clamp a requested trajectory window to the supported range.
- `format_trajectory_window(trajectories: List[Dict[str, Any]])` — [`L200`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L200) — Format trajectory entries into a compact, readable window.
- `load_recent_trajectories(run_data_manager: Any, last_n_steps: Optional[int] = None)` — [`L110`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L110) — Load the most recent trajectory entries, preserving chronological order.
- `load_trajectory_range(run_data_manager: Any, start: int, end: int)` — [`L127`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L127) — Load trajectory entries whose ``step`` falls in [start, end].
- `read_last_jsonl_lines(path: Path, max_lines: int)` — [`L59`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L59) — Read the last non-empty lines from a JSONL file without scanning it twice.
- `resolve_trajectory_path(run_data_manager: Any = None)` — [`L29`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L29) — Resolve trajectory_history.jsonl using cache/run_data precedence.

## Module values
- `DEFAULT_TRAJECTORY_WINDOW` — [`L15`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L15)
- `MAX_TRAJECTORY_WINDOW` — [`L14`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L14)
- `logger` — [`L12`](../../../../../../../raw/code/continual-harness/agents/subagents/utils/trajectory_window.py#L12)

