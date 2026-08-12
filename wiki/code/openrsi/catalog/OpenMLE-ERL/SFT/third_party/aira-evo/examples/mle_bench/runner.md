---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.examples.mle_bench.runner`/
symbols:
  main: main().
  _terminal_done_reason_for_task: _terminal_done_reason_for_task().
  run_task: run_task().
  _safe_int: _safe_int().
  _infer_legacy_done_reason: _infer_legacy_done_reason().
  main.run_all: main().run_all().
  _load_task_name: _load_task_name().
  main.run_all.progress_history_loop: main().run_all().progress_history_loop().
  _safe_float: _safe_float().
  _load_task_config: _load_task_config().
  _write_failed_task_outputs: _write_failed_task_outputs().
  TERMINAL_SKIP_DONE_REASONS: TERMINAL_SKIP_DONE_REASONS.
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py)

## Functions
- `_infer_legacy_done_reason(*, task_state: dict[str, Any], output_dir: Path, runner_cfg: dict[str, Any])` — [`L60`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L60)
- `_load_task_config(task_dir: Path)` — [`L48`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L48)
- `_load_task_name(task_dir: Path)` — [`L55`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L55)
- `_safe_float(value: Any, default: float = 0)` — [`L34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L34)
- `_safe_int(value: Any, default: int = 0)` — [`L41`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L41)
- `_terminal_done_reason_for_task(*, output_root: Path, task_dir: Path, epoch_index: int, runner_cfg: dict[str, Any])` — [`L127`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L127)
- `_write_failed_task_outputs(output_dir: Path, task_name: str, error: str, return_code: int | None)` — [`L160`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L160)
- `main(cfg: DictConfig)` — [`L303`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L303)
- `progress_history_loop()` — [`L363`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L363)
- `run_all()` — [`L356`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L356)
- `run_task(*, task_dir: Path, epoch_index: int, output_root: Path, resolved_runner_config_path: Path, runner_cfg: dict[str, Any], task_concurrency: asyncio.Semaphore, subprocess_env: dict[str, str])` — [`L205`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L205)

## Module values
- `TERMINAL_SKIP_DONE_REASONS` — [`L25`](../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/examples/mle_bench/runner.py#L25)

