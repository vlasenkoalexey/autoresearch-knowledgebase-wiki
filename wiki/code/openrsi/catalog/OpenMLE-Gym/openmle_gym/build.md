---
title: 'Module: OpenMLE-Gym/openmle_gym/build.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/openmle_gym/build.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.openmle_gym.build`/
symbols:
  _run_one_local: _run_one_local().
  build_tasks: build_tasks().
  _run_all.worker: _run_all().worker().
  _run_all: _run_all().
  _json_safe: _json_safe().
  _dry_run: _dry_run().
  MLEBENCH_SLUGS: MLEBENCH_SLUGS.
  _summarize_results: _summarize_results().
---
# Module: [`OpenMLE-Gym/openmle_gym/build.py`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py)

## Functions
- `_dry_run(slugs: list[str], output_root: Path, batch_name: str, skip_mlebench: bool, delete_raw: bool)` — [`L125`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py#L125)
- `_json_safe(value: Any)` — [`L92`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py#L92) — Convert legacy pipeline return objects into JSON-serializable data.
- `_run_all(builder_root: Path, batch_name: str, slugs: list[str], retry: int, output_root: Path, info_csv: Path, max_concurrency: int, delete_raw: bool, execution_mode: str, task_timeout: float)` — [`L192`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py#L192)
- `_run_one_local(builder_root: str | Path, batch_name: str, slug: str, retry: int, output_root: str | Path, info_csv: str | Path, delete_raw: bool, code_execution_mode: str = "process", code_timeout: float = 600)` — [`L144`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py#L144)
- `_summarize_results(results: list[Any])` — [`L97`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py#L97)
- `build_tasks(slugs_file: str | Path, output_root: str | Path = "artifacts/builds", info_csv: str | Path = "builder_core/info.csv", batch_name: str | None = None, retry: int = 2, max_concurrency: int = 1, limit: int | None = None, skip_mlebench: bool = True, delete_raw: bool = False, execute: bool = False, execution_mode: str = "process", task_timeout: float = 3600)` — [`L263`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py#L263)
- `worker(slug: str)` — [`L206`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py#L206) — documented in [OpenMLE-Gym-openmle_gym-process_runner](../../../concepts/OpenMLE-Gym-openmle_gym-process_runner.md)

## Module values
- `MLEBENCH_SLUGS` — [`L13`](../../../../../../raw/code/openrsi/OpenMLE-Gym/openmle_gym/build.py#L13)

