---
title: 'Module: examples/signal_processing/evaluator.py'
type: catalog
provenance: extracted
module: examples/signal_processing/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.signal_processing.evaluator`/
symbols:
  safe_float: safe_float().
  evaluate: evaluate().
  evaluate_stage1: evaluate_stage1().
  evaluate_stage2: evaluate_stage2().
  run_with_timeout: run_with_timeout().
  calculate_slope_changes: calculate_slope_changes().
  calculate_lag_error: calculate_lag_error().
  calculate_average_tracking_error: calculate_average_tracking_error().
  calculate_false_reversal_penalty: calculate_false_reversal_penalty().
  calculate_composite_score: calculate_composite_score().
  generate_test_signals: generate_test_signals().
---
# Module: [`examples/signal_processing/evaluator.py`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py)

## Functions
- `calculate_average_tracking_error(filtered_signal, original_signal, window_size)` — [`L99`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L99) — Calculate average tracking error L_avg(θ) over the window
- `calculate_composite_score(S, L_recent, L_avg, R, alpha=[0.3, 0.2, 0.2, 0.3])` — [`L189`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L189) — Calculate the composite metric J(θ) = α₁·S(θ) + α₂·L_recent(θ) + α₃·L_avg(θ) + α₄·R(θ)
- `calculate_false_reversal_penalty(filtered_signal, clean_signal, window_size)` — [`L134`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L134) — Calculate false reversal penalty R(θ) - mismatched trend changes
- `calculate_lag_error(filtered_signal, original_signal, window_size)` — [`L72`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L72) — Calculate instantaneous lag error L_recent(θ) = |y[n] - x[n]|
- `calculate_slope_changes(signal_data)` — [`L47`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L47) — Calculate slope change penalty S(θ) - counts directional reversals
- `evaluate(program_path)` — [`L266`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L266) — Main evaluation function that tests the signal processing algorithm
- `evaluate_stage1(program_path)` — [`L456`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L456) — Stage 1 evaluation: Quick validation that the program runs without errors
- `evaluate_stage2(program_path)` — [`L508`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L508) — Stage 2 evaluation: Full evaluation with all test signals
- `generate_test_signals(num_signals=5)` — [`L217`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L217) — Generate multiple test signals with different characteristics
- `run_with_timeout(func, args=(), kwargs={}, timeout_seconds=30)` — [`L24`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L24) — Run a function with a timeout using concurrent.futures
- `safe_float(value)` — [`L37`](../../../../../../raw/code/openevolve/examples/signal_processing/evaluator.py#L37) — Convert a value to float safely

