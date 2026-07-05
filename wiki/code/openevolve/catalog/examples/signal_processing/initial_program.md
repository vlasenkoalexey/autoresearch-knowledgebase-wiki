---
title: 'Module: examples/signal_processing/initial_program.py'
type: catalog
provenance: extracted
module: examples/signal_processing/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.signal_processing.initial_program`/
symbols:
  results: results.
  process_signal: process_signal().
  run_signal_processing: run_signal_processing().
  adaptive_filter: adaptive_filter().
  enhanced_filter_with_trend_preservation: enhanced_filter_with_trend_preservation().
  generate_test_signal: generate_test_signal().
---
# Module: [`examples/signal_processing/initial_program.py`](../../../../../../raw/code/openevolve/examples/signal_processing/initial_program.py)

## Functions
- `adaptive_filter(x, window_size=20)` — [`L13`](../../../../../../raw/code/openevolve/examples/signal_processing/initial_program.py#L13) — Adaptive signal processing algorithm using sliding window approach.
- `enhanced_filter_with_trend_preservation(x, window_size=20)` — [`L41`](../../../../../../raw/code/openevolve/examples/signal_processing/initial_program.py#L41) — Enhanced version with trend preservation using weighted moving average.
- `generate_test_signal(length=1000, noise_level=0.3, seed=42)` — [`L92`](../../../../../../raw/code/openevolve/examples/signal_processing/initial_program.py#L92) — Generate synthetic test signal with known characteristics.
- `process_signal(input_signal, window_size=20, algorithm_type="enhanced")` — [`L71`](../../../../../../raw/code/openevolve/examples/signal_processing/initial_program.py#L71) — Main signal processing function that applies the selected algorithm.
- `run_signal_processing(signal_length=1000, noise_level=0.3, window_size=20)` — [`L130`](../../../../../../raw/code/openevolve/examples/signal_processing/initial_program.py#L130) — Run the signal processing algorithm on a test signal.

## Module values
- `results` — [`L185`](../../../../../../raw/code/openevolve/examples/signal_processing/initial_program.py#L185)

