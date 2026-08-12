---
title: 'Module: OpenMLE-ERL/SFT/tts_search/data_produce/common.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/data_produce/common.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.data_produce.common`/
symbols:
  maybe_float: maybe_float().
  read_text: read_text().
  json_safe: json_safe().
  summary_stats: summary_stats().
  read_jsonl: read_jsonl().
  write_jsonl: write_jsonl().
  safe_task_output_name: safe_task_output_name().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/data_produce/common.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/common.py)

## Functions
- `json_safe(value: Any)` — [`L33`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/common.py#L33) — Convert nested values to JSON-serializable Python objects.
- `maybe_float(value: Any)` — [`L13`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/common.py#L13) — Convert a value to a finite float.
- `read_jsonl(path: Path)` — [`L71`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/common.py#L71) — Read newline-delimited JSON records.
- `read_text(path: Path)` — [`L57`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/common.py#L57) — Read text from disk if present. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `safe_task_output_name(task_name: str, task_id: str | None = None)` — [`L104`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/common.py#L104) — Build a filesystem-safe task directory name.
- `summary_stats(values: Iterable[float])` — [`L121`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/common.py#L121) — Summarize numeric values for reports.
- `write_jsonl(path: Path, rows: Iterable[dict[str, Any]])` — [`L88`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/common.py#L88) — Write rows as newline-delimited JSON.

