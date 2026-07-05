---
title: 'Module: examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.uncertainty_ineq.evaluator`/
symbols:
  x: x.
  compute_c4_and_rmax: compute_c4_and_rmax().
  _construct_P_with_forced_zero: _construct_P_with_forced_zero().
  evaluate: evaluate().
  _hermite_4k_polys: _hermite_4k_polys().
  _largest_positive_root_of_P_over_x2: _largest_positive_root_of_P_over_x2().
  verify_c4_solution_strict: verify_c4_solution_strict().
  BENCHMARK: BENCHMARK.
---
# Module: [`examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py)

## Functions
- `_construct_P_with_forced_zero(coeffs: np.ndarray)` — [`L28`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py#L28) — Given m input coeffs (c0..c_{m-1}), build the Hermite combo
- `_hermite_4k_polys(m: int)` — [`L22`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py#L22)
- `_largest_positive_root_of_P_over_x2(P: sp.Expr)` — [`L53`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py#L53)
- `compute_c4_and_rmax(input_coeffs: np.ndarray)` — [`L76`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py#L76)
- `evaluate(program_path: str)` — [`L101`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py#L101)
- `verify_c4_solution_strict(user_coeffs: np.ndarray, reported_c4: float, reported_rmax: float, atol=1e-9, rtol=1e-9)` — [`L87`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py#L87)

## Module values
- `BENCHMARK` — [`L17`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py#L17)
- `x` — [`L19`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/uncertainty_ineq/evaluator.py#L19)

