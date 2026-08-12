---
title: 'Module: OpenMLE-Gym/openmle_gym/overview.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/openmle_gym/overview.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.openmle_gym.overview`/
symbols:
  generate_overview.run_one_impl: generate_overview().run_one_impl().
  generate_overview: generate_overview().
  _analyze_task_full: _analyze_task_full().
  _run_metadata_pipeline: _run_metadata_pipeline().
  _run_metadata_pipeline.analyze_in_process: _run_metadata_pipeline().analyze_in_process().
  analyze_task: analyze_task().
  _chunked_map: _chunked_map().
  _require_llm_env: _require_llm_env().
  _write_overview_rows: _write_overview_rows().
  _chunked_map.process_chunk: _chunked_map().process_chunk().
  generate_overview.run_one: generate_overview().run_one().
  overview_has_task_failures: overview_has_task_failures().
  R: R.
  T: T.
  _format_size: _format_size().
  _failed_overview_row: _failed_overview_row().
  _directory_size: _directory_size().
  FIELDNAMES: FIELDNAMES.
  _read_overview_rows: _read_overview_rows().
---
# Module: [`OpenMLE-Gym/openmle_gym/overview.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py)

## Functions
- `_analyze_task_full(task_dir: Path, skip_llm: bool = False, metric_execution_mode: str = "process", metric_timeout: float = 120)` — [`L211`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L211) — Analyze one task entirely inside its task worker process.
- `_chunked_map(items: list[T], worker_count: int, func: Callable[[T], R], desc: str)` — [`L75`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L75) — Run work in deterministic chunks and return results in input order.
- `_directory_size(path: Path)` — [`L31`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L31)
- `_failed_overview_row(task_dir: Path, reason: str, skip_llm: bool)` — [`L246`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L246)
- `_format_size(num_bytes: int)` — [`L45`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L45)
- `_read_overview_rows(path: Path)` — [`L110`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L110)
- `_require_llm_env()` — [`L68`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L68)
- `_run_metadata_pipeline(task_dirs: list[Path], output_csv: Path, workers: int, execution_mode: str = "process", task_timeout: float = 600)` — [`L124`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L124) — Update the base CSV with metadata pipeline LLM and metric steps.
- `_write_overview_rows(path: Path, rows: list[dict[str, Any]])` — [`L115`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L115)
- `analyze_in_process(task_dir: Path)` — [`L141`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L141) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)
- `analyze_task(task_dir: Path, skip_llm: bool = False, metric_execution_mode: str = "process", metric_timeout: float = 120)` — [`L164`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L164)
- `generate_overview(tasks_root: str | Path, output_csv: str | Path, workers: int = 1, skip_llm: bool = False, execution_mode: str = "process", task_timeout: float = 600)` — [`L269`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L269)
- `overview_has_task_failures(path: str | Path)` — [`L262`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L262)
- `process_chunk(chunk: list[tuple[int, T]])` — [`L96`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L96)
- `run_one(task_dir: Path)` — [`L317`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L317)
- `run_one_impl(task_dir: Path)` — [`L283`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L283) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)

## Module values
- `FIELDNAMES` — [`L54`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L54)
- `R` — [`L28`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L28)
- `T` — [`L27`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/overview.py#L27)

