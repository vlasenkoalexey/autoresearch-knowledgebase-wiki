---
title: 'Module: utils/metric_tracking/claude_session_reader.py'
type: catalog
provenance: extracted
module: utils/metric_tracking/claude_session_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.metric_tracking.claude_session_reader`/
symbols:
  load_new_usage_entries: load_new_usage_entries().
  _parse_timestamp: _parse_timestamp().
  extract_tokens_from_entry: extract_tokens_from_entry().
  _create_unique_hash: _create_unique_hash().
  extract_tool_calls_from_entry: extract_tool_calls_from_entry().
  logger: logger.
  find_jsonl_files: find_jsonl_files().
---
# Module: [`utils/metric_tracking/claude_session_reader.py`](../../../../../../raw/code/continual-harness/utils/metric_tracking/claude_session_reader.py)

## Functions
- `_create_unique_hash(entry: dict)` — [`L44`](../../../../../../raw/code/continual-harness/utils/metric_tracking/claude_session_reader.py#L44) — Derive a dedup key that groups all content blocks from a single API call.
- `_parse_timestamp(ts: Any)` — [`L26`](../../../../../../raw/code/continual-harness/utils/metric_tracking/claude_session_reader.py#L26) — Parse a timestamp value into a timezone-aware UTC datetime.
- `extract_tokens_from_entry(entry: dict)` — [`L62`](../../../../../../raw/code/continual-harness/utils/metric_tracking/claude_session_reader.py#L62) — Extract token counts and cost from a Claude Code JSONL assistant entry.
- `extract_tool_calls_from_entry(entry: dict)` — [`L116`](../../../../../../raw/code/continual-harness/utils/metric_tracking/claude_session_reader.py#L116) — Extract tool_use blocks from message.content as {name, args} dicts.
- `find_jsonl_files(data_path: Path)` — [`L19`](../../../../../../raw/code/continual-harness/utils/metric_tracking/claude_session_reader.py#L19) — Return all *.jsonl files under data_path, sorted by path for reproducibility.
- `load_new_usage_entries(data_path: Path, processed_hashes: set[str], since_timestamp: datetime | None = None)` — [`L134`](../../../../../../raw/code/continual-harness/utils/metric_tracking/claude_session_reader.py#L134) — Load assistant JSONL entries that have not yet been processed.

## Module values
- `logger` — [`L16`](../../../../../../raw/code/continual-harness/utils/metric_tracking/claude_session_reader.py#L16)

