---
title: 'Module: utils/metric_tracking/codex_session_reader.py'
type: catalog
provenance: extracted
module: utils/metric_tracking/codex_session_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.metric_tracking.codex_session_reader`/
symbols:
  load_new_usage_entries: load_new_usage_entries().
  find_session_files: find_session_files().
  extract_tool_calls_from_entry: extract_tool_calls_from_entry().
  logger: logger.
  extract_tokens_from_entry: extract_tokens_from_entry().
  _normalize_tool_args: _normalize_tool_args().
  extract_usage_snapshot: extract_usage_snapshot().
  SESSIONS_REL: SESSIONS_REL.
  _parse_timestamp: _parse_timestamp().
  _create_step_hash: _create_step_hash().
---
# Module: [`utils/metric_tracking/codex_session_reader.py`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py)

## Functions
- `_create_step_hash(session_key: str, cumulative_total: int | None, parsed_ts: datetime | None, line_idx: int, compaction_offset: int = 0)` — [`L53`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L53) — Stable dedup key for one logical Codex usage step (a bit more complex due to how session rollout log emits data).
- `_normalize_tool_args(raw_args: Any)` — [`L71`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L71) — Best-effort normalization for tool-call args.
- `_parse_timestamp(ts: Any)` — [`L39`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L39) — Parse ISO-8601 or UNIX timestamp to UTC datetime.
- `extract_tokens_from_entry(entry: dict)` — [`L148`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L148) — Extract token counts from a Codex session entry.
- `extract_tool_calls_from_entry(entry: dict)` — [`L159`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L159) — Extract tool/MCP calls from entry if present. Best-effort.
- `extract_usage_snapshot(entry: dict)` — [`L84`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L84) — Extract step token usage and cumulative total from a Codex entry.
- `find_session_files(data_path: Path)` — [`L25`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L25) — Return JSONL files under data_path/sessions/, sorted by mtime (most recent first).
- `load_new_usage_entries(data_path: Path, processed_hashes: set[str])` — [`L180`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L180) — Load Codex session entries that have not been processed.

## Module values
- `SESSIONS_REL` — [`L22`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L22)
- `logger` — [`L20`](../../../../../../raw/code/continual-harness/utils/metric_tracking/codex_session_reader.py#L20)

