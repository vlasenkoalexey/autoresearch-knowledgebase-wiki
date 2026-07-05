---
title: 'Module: examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.heilbronn_triangle.evaluator`/
symbols:
  evaluate: evaluate().
  NUM_POINTS: NUM_POINTS.
  triangle_area: triangle_area().
  BENCHMARK: BENCHMARK.
  TOL: TOL.
  check_inside_triangle_wtol: check_inside_triangle_wtol().
---
# Module: [`examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py)

## Functions
- `check_inside_triangle_wtol(points: np.ndarray, tol: float = 0.000001)` — [`L27`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py#L27) — Checks that all points are inside the triangle with vertices (0,0), (1,0), (0.5, sqrt(3)/2).
- `evaluate(program_path: str)` — [`L49`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py#L49)
- `triangle_area(a: np.array, b: np.array, c: np.array)` — [`L45`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py#L45)

## Module values
- `BENCHMARK` — [`L22`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py#L22)
- `NUM_POINTS` — [`L24`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py#L24)
- `TOL` — [`L23`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/heilbronn_triangle/evaluator.py#L23)

