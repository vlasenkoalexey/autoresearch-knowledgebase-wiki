---
title: 'Module: utils/metric_tracking/gemini_session_reader.py'
type: catalog
provenance: extracted
module: utils/metric_tracking/gemini_session_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.metric_tracking.gemini_session_reader`/
symbols:
  load_new_usage_entries: load_new_usage_entries().
  extract_tokens_from_message: extract_tokens_from_message().
  find_session_files: find_session_files().
  extract_tool_calls_from_message: extract_tool_calls_from_message().
  logger: logger.
  CHATS_REL: CHATS_REL.
  _parse_timestamp: _parse_timestamp().
---
# Module: [`utils/metric_tracking/gemini_session_reader.py`](../../../../../../raw/code/continual-harness/utils/metric_tracking/gemini_session_reader.py)

## Functions
- `_parse_timestamp(ts: Any)` — [`L29`](../../../../../../raw/code/continual-harness/utils/metric_tracking/gemini_session_reader.py#L29) — Parse ISO-8601 or UNIX timestamp to UTC datetime.
- `extract_tokens_from_message(msg: dict)` — [`L43`](../../../../../../raw/code/continual-harness/utils/metric_tracking/gemini_session_reader.py#L43) — Extract token counts from a Gemini session message (type=gemini).
- `extract_tool_calls_from_message(msg: dict)` — [`L83`](../../../../../../raw/code/continual-harness/utils/metric_tracking/gemini_session_reader.py#L83) — Extract toolCalls from a Gemini message as {name, args} list.
- `find_session_files(data_path: Path)` — [`L20`](../../../../../../raw/code/continual-harness/utils/metric_tracking/gemini_session_reader.py#L20) — Return all session-*.json files under data_path/tmp/workspace/chats, sorted by mtime.
- `load_new_usage_entries(data_path: Path, processed_hashes: set[str])` — [`L95`](../../../../../../raw/code/continual-harness/utils/metric_tracking/gemini_session_reader.py#L95) — Load gemini messages from session JSON files that have not been processed.

## Module values
- `CHATS_REL` — [`L17`](../../../../../../raw/code/continual-harness/utils/metric_tracking/gemini_session_reader.py#L17)
- `logger` — [`L15`](../../../../../../raw/code/continual-harness/utils/metric_tracking/gemini_session_reader.py#L15)

