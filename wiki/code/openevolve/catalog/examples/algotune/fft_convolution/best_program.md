---
title: 'Module: examples/algotune/fft_convolution/best_program.py'
type: catalog
provenance: extracted
module: examples/algotune/fft_convolution/best_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.fft_convolution.best_program`/
symbols:
  run_solver: run_solver().
  FFTConvolution: FFTConvolution#
  FFTConvolution.solve: FFTConvolution#solve().
  FFTConvolution.__init__: FFTConvolution#__init__().
  FFTConvolution.is_solution: FFTConvolution#is_solution().
---
# Module: [`examples/algotune/fft_convolution/best_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/best_program.py)

## Classes
### `FFTConvolution`
- def: [`examples/algotune/fft_convolution/best_program.py:74`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/best_program.py#L74)
- doc: Initial implementation of fft_convolution task.
- signature: `class FFTConvolution:`
- members:
  - `__init__(self)` — [`L80`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/best_program.py#L80) — Initialize the FFTConvolution.
  - `is_solution(self, problem, solution)` — [`L159`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/best_program.py#L159) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L84`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/best_program.py#L84) — Solve the fft_convolution problem.
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L269`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/best_program.py#L269) — Main function to run the solver.

