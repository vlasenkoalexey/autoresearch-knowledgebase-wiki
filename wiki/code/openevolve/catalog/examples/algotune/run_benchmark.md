---
title: 'Module: examples/algotune/run_benchmark.py'
type: catalog
provenance: extracted
module: examples/algotune/run_benchmark.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.run_benchmark`/
symbols:
  main: main().
  run_openevolve_task: run_openevolve_task().
  generate_summary: generate_summary().
  parse_args: parse_args().
  discover_algotune_tasks: discover_algotune_tasks().
  parse_task_results: parse_task_results().
  calculate_algotune_score: calculate_algotune_score().
---
# Module: [`examples/algotune/run_benchmark.py`](../../../../../../raw/code/openevolve/examples/algotune/run_benchmark.py)

## Functions
- `calculate_algotune_score(speedups: List[float])` — [`L275`](../../../../../../raw/code/openevolve/examples/algotune/run_benchmark.py#L275) — Calculate AlgoTune Score as harmonic mean of speedups.
- `discover_algotune_tasks(algotune_dir: Path)` — [`L82`](../../../../../../raw/code/openevolve/examples/algotune/run_benchmark.py#L82) — Discover all AlgoTune task directories.
- `generate_summary(task_results: Dict[str, Dict[str, Any]])` — [`L297`](../../../../../../raw/code/openevolve/examples/algotune/run_benchmark.py#L297) — Generate summary statistics from task results.
- `main()` — [`L334`](../../../../../../raw/code/openevolve/examples/algotune/run_benchmark.py#L334) — Main function.
- `parse_args()` — [`L27`](../../../../../../raw/code/openevolve/examples/algotune/run_benchmark.py#L27) — Parse command-line arguments.
- `parse_task_results(task_dir: Path, task_name: str, runtime_seconds: float)` — [`L209`](../../../../../../raw/code/openevolve/examples/algotune/run_benchmark.py#L209) — Parse OpenEvolve results from the output directory.
- `run_openevolve_task(task_name: str, task_dir: Path, iterations: int, timeout: int, custom_config: Optional[str] = None, verbose: bool = False)` — [`L105`](../../../../../../raw/code/openevolve/examples/algotune/run_benchmark.py#L105) — Run OpenEvolve on a single AlgoTune task.

