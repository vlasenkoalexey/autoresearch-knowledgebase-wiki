---
title: 'Module: utils/metric_tracking/hermes_session_reader.py'
type: catalog
provenance: extracted
module: utils/metric_tracking/hermes_session_reader.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.metric_tracking.hermes_session_reader`/
symbols:
  load_new_usage_entries: load_new_usage_entries().
  _load_usage_events: _load_usage_events().
  get_latest_session_id: get_latest_session_id().
  _normalize_tool_calls: _normalize_tool_calls().
  _extract_usage_tokens: _extract_usage_tokens().
  logger: logger.
  _parse_timestamp: _parse_timestamp().
  find_session_logs: find_session_logs().
  USAGE_EVENTS_NAME: USAGE_EVENTS_NAME.
  _normalize_tool_name: _normalize_tool_name().
  _coerce_mapping: _coerce_mapping().
  STATE_DB_NAME: STATE_DB_NAME.
---
# Module: [`utils/metric_tracking/hermes_session_reader.py`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py)

## Functions
- `_coerce_mapping(value: Any)` — [`L89`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L89)
- `_extract_usage_tokens(raw: dict[str, Any])` — [`L100`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L100)
- `_load_usage_events(data_path: Path)` — [`L128`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L128)
- `_normalize_tool_calls(raw: Any)` — [`L48`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L48)
- `_normalize_tool_name(name: Any)` — [`L39`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L39)
- `_parse_timestamp(ts: Any)` — [`L23`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L23)
- `find_session_logs(data_path: Path)` — [`L82`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L82)
- `get_latest_session_id(data_path: Path)` — [`L166`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L166)
- `load_new_usage_entries(data_path: Path, processed_hashes: set[str], last_seen_totals: dict[str, dict[str, Any]] | None = None)` — [`L175`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L175) — Load new Hermes usage entries from session JSON plus wrapper usage events.

## Module values
- `STATE_DB_NAME` — [`L20`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L20)
- `USAGE_EVENTS_NAME` — [`L21`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L21)
- `logger` — [`L18`](../../../../../../raw/code/continual-harness/utils/metric_tracking/hermes_session_reader.py#L18)

