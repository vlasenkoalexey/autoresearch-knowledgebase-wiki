---
title: 'Module: examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py'
type: catalog
provenance: extracted
module: examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.fft_cmplx_scipy_fftpack.evaluator`/
symbols:
  evaluate: evaluate().
  evaluate_stage1: evaluate_stage1().
  safe_convert: safe_convert().
  run_with_timeout: run_with_timeout().
  measure_baseline_performance: measure_baseline_performance().
  measure_evolved_performance: measure_evolved_performance().
  e: e.
  evaluate_stage2: evaluate_stage2().
  setup_algotune_paths: setup_algotune_paths().
  calculate_speedup: calculate_speedup().
---
# Module: [`examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py)

## Functions
- `calculate_speedup(baseline_time_ms: float, evolved_time_ms: float, is_valid: bool)` — [`L101`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L101) — Calculate speedup between baseline and evolved solution.
- `evaluate(program_path, config=None)` — [`L260`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L260) — Enhanced evaluation with baseline comparison for fft_cmplx_scipy_fftpack task.
- `evaluate_stage1(program_path, config=None)` — [`L505`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L505) — First stage evaluation with basic functionality check of the evolved solve method
- `evaluate_stage2(program_path, config=None)` — [`L600`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L600) — Second stage evaluation with more thorough testing of the evolved solve method
- `measure_baseline_performance(task_instance, problem, num_runs=3, warmup_runs=1)` — [`L130`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L130) — Measure baseline performance using the original AlgoTune implementation.
- `measure_evolved_performance(program, problem, num_runs=3, warmup_runs=1, timeout_seconds=30)` — [`L191`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L191) — Measure evolved solution performance.
- `run_with_timeout(func, args=(), kwargs={}, timeout_seconds=30)` — [`L68`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L68) — Run a function with a timeout using concurrent.futures
- `safe_convert(value)` — [`L89`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L89) — Convert a value safely for evaluation
- `setup_algotune_paths()` — [`L28`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L28) — Setup Python import paths for AlgoTune modules.

## Module values
- `e` — [`L60`](../../../../../../../raw/code/openevolve/examples/algotune/fft_cmplx_scipy_fftpack/evaluator.py#L60)

