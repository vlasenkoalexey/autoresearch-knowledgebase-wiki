---
title: 'Module: OpenMLE-ERL/SFT/tts_search/services/result_persistence.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/services/result_persistence.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.services.result_persistence`/
symbols:
  StreamingJSONLWriter.write: StreamingJSONLWriter#write().
  update_progress_snapshot: update_progress_snapshot().
  append_compact_progress_snapshot: append_compact_progress_snapshot().
  append_jsonl_record: append_jsonl_record().
  StreamingJSONLWriter._count: StreamingJSONLWriter#_count.
  StreamingJSONLWriter: StreamingJSONLWriter#
  StreamingJSONLWriter._path: StreamingJSONLWriter#_path.
  build_compact_progress_snapshot: build_compact_progress_snapshot().
  StreamingJSONLWriter.get_count: StreamingJSONLWriter#get_count().
  _file_lock: _file_lock().
  iter_jsonl_records: iter_jsonl_records().
  StreamingJSONLWriter._lock: StreamingJSONLWriter#_lock.
  atomic_write_json: atomic_write_json().
  StreamingJSONLWriter.__init__: StreamingJSONLWriter#__init__().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/services/result_persistence.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py)

## Classes
### `StreamingJSONLWriter`
- def: [`OpenMLE-ERL/SFT/tts_search/services/result_persistence.py:25`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L25)
- doc: Async JSONL writer used by the service scheduler.
- signature: `class StreamingJSONLWriter:`
- members:
  - `get_count(self)` — [`L45`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L45)
  - `write(self, data: dict[str, Any])` — [`L40`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L40)
- protocol/private: `__init__`[`L28`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L28), `_count`[`L31`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L31), `_lock`[`L30`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L30), `_path`[`L29`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L29)
- uses (calls/refs, reference-scoped): [`append_jsonl_record`](result_persistence.md#append_jsonl_record)
- used by: [`_run_looping_tasks`](scheduler.md#Scheduler._run_looping_tasks), [`_process_eval_batch`](scheduler.md#Scheduler._process_eval_batch), [`run_evaluation_only`](scheduler.md#Scheduler.run_evaluation_only), [`_gen_worker`](scheduler.md#Scheduler._gen_worker), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`_eval_writer`](scheduler.md#Scheduler._eval_writer), [`_gen_writer`](scheduler.md#Scheduler._gen_writer)

## Functions
- `_file_lock(path: Path)` — [`L50`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L50) — Process-safe advisory lock for writers sharing a run directory.
- `append_compact_progress_snapshot(output_dir: Path)` — [`L158`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L158) — Append one compact progress_history row and return it.
- `append_jsonl_record(path: Path, record: dict[str, Any])` — [`L65`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L65) — Append one JSON object to a JSONL file and flush it to disk.
- `atomic_write_json(path: Path, payload: Any)` — [`L77`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L77) — Atomically replace a JSON file.
- `build_compact_progress_snapshot(output_dir: Path)` — [`L107`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L107) — Build the compact progress_history row used by distillation runs.
- `iter_jsonl_records(path: Path)` — [`L89`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L89) — Yield JSON objects from a JSONL file, skipping blank or invalid lines.
- `update_progress_snapshot(path: Path, *, task_id: str, task_state: dict[str, Any], total_tasks: int, history_path: Path | None = None)` — [`L166`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/result_persistence.py#L166) — Merge one task state into progress.json and optionally append history.

