---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.examples.mle_bench.runner`/
symbols:
  main: main().
  REPO_ROOT: REPO_ROOT.
  run_task: run_task().
  main.run_all: main().run_all().
  _write_failed_task_outputs: _write_failed_task_outputs().
  _load_task_name: _load_task_name().
  _has_completed_task_outputs: _has_completed_task_outputs().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py)

## Functions
- `_has_completed_task_outputs(output_dir: Path)` — [`L89`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py#L89)
- `_load_task_name(task_dir: Path)` — [`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py#L35)
- `_write_failed_task_outputs(output_dir: Path, task_name: str, error: str, return_code: int | None)` — [`L44`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py#L44)
- `main(cfg: DictConfig)` — [`L224`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py#L224) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- `run_all()` — [`L295`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py#L295)
- `run_task(*, task_dir: Path, epoch_index: int, output_root: Path, resolved_runner_config_path: Path, task_concurrency: asyncio.Semaphore, subprocess_env: dict[str, str], strict_resume: bool)` — [`L125`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py#L125)

## Module values
- `REPO_ROOT` — [`L16`](../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/examples/mle_bench/runner.py#L16)

