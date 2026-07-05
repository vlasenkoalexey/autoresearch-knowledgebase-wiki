---
title: 'Module: openevolve/utils/trace_export_utils.py'
type: catalog
provenance: extracted
module: openevolve/utils/trace_export_utils.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.utils.trace_export_utils`/
symbols:
  export_traces: export_traces().
  load_traces: load_traces().
  export_traces_json: export_traces_json().
  logger: logger.
  export_traces_jsonl: export_traces_jsonl().
  export_traces_hdf5: export_traces_hdf5().
  load_traces_hdf5: load_traces_hdf5().
  append_trace_jsonl: append_trace_jsonl().
  load_traces_jsonl: load_traces_jsonl().
  load_traces_json: load_traces_json().
---
# Module: [`openevolve/utils/trace_export_utils.py`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py)

## Functions
- `append_trace_jsonl(trace: Any, output_path: Union[str, Path], compress: bool = False)` — [`L153`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L153) — Append a single trace to a JSONL file — documented in [openevolve-evolution_trace](../../../concepts/openevolve-evolution_trace.md)
- `export_traces(traces: List[Any], output_path: Union[str, Path], format: str = "jsonl", compress: bool = False, metadata: Optional[Dict[str, Any]] = None)` — [`L295`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L295) — Export traces to specified format — documented in [openevolve-evolution_trace](../../../concepts/openevolve-evolution_trace.md)
- `export_traces_hdf5(traces: List[Any], output_path: Union[str, Path], metadata: Optional[Dict[str, Any]] = None)` — [`L83`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L83) — Export traces to HDF5 format
- `export_traces_json(traces: List[Any], output_path: Union[str, Path], metadata: Optional[Dict[str, Any]] = None)` — [`L48`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L48) — Export traces to JSON format with metadata — documented in [openevolve-evolution_trace](../../../concepts/openevolve-evolution_trace.md)
- `export_traces_jsonl(traces: List[Any], output_path: Union[str, Path], compress: bool = False)` — [`L14`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L14) — Export traces to JSONL format (one JSON object per line)
- `load_traces(input_path: Union[str, Path], format: Optional[str] = None)` — [`L324`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L324) — Load traces from file, auto-detecting format if not specified
- `load_traces_hdf5(input_path: Union[str, Path])` — [`L232`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L232) — Load traces from an HDF5 file
- `load_traces_json(input_path: Union[str, Path])` — [`L213`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L213) — Load traces from a JSON file
- `load_traces_jsonl(input_path: Union[str, Path], compress: bool = False)` — [`L182`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L182) — Load traces from a JSONL file

## Module values
- `logger` — [`L11`](../../../../../../raw/code/openevolve/openevolve/utils/trace_export_utils.py#L11)

