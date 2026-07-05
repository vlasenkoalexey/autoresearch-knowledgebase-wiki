---
title: 'Module: examples/algotune/fft_convolution/initial_program.py'
type: catalog
provenance: extracted
module: examples/algotune/fft_convolution/initial_program.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.algotune.fft_convolution.initial_program`/
symbols:
  run_solver: run_solver().
  FFTConvolution: FFTConvolution#
  FFTConvolution.solve: FFTConvolution#solve().
  FFTConvolution.__init__: FFTConvolution#__init__().
  FFTConvolution.is_solution: FFTConvolution#is_solution().
---
# Module: [`examples/algotune/fft_convolution/initial_program.py`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/initial_program.py)

## Classes
### `FFTConvolution`
- def: [`examples/algotune/fft_convolution/initial_program.py:73`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/initial_program.py#L73)
- doc: Initial implementation of fft_convolution task.
- signature: `class FFTConvolution:`
- members:
  - `__init__(self)` — [`L79`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/initial_program.py#L79) — Initialize the FFTConvolution.
  - `is_solution(self, problem, solution)` — [`L117`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/initial_program.py#L117) — Check if the provided solution is valid.
  - `solve(self, problem)` — [`L83`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/initial_program.py#L83) — Solve the fft_convolution problem.
- used by: (1 test-only callers)

## Functions
- `run_solver(problem)` — [`L227`](../../../../../../../raw/code/openevolve/examples/algotune/fft_convolution/initial_program.py#L227) — Main function to run the solver.

