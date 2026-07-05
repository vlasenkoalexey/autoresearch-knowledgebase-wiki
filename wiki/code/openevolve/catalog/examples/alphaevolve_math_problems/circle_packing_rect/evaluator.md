---
title: 'Module: examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.circle_packing_rect.evaluator`/
symbols:
  evaluate: evaluate().
  validate_packing_inside_rect_wtol: validate_packing_inside_rect_wtol().
  NUM_CIRCLES: NUM_CIRCLES.
  TOL: TOL.
  BENCHMARK: BENCHMARK.
  minimum_circumscribing_rectangle: minimum_circumscribing_rectangle().
  validate_packing_radii: validate_packing_radii().
  validate_packing_overlap_wtol: validate_packing_overlap_wtol().
---
# Module: [`examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py)

## Functions
- `evaluate(program_path: str)` — [`L69`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py#L69)
- `minimum_circumscribing_rectangle(circles: np.ndarray)` — [`L26`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py#L26) — Returns the width and height of the minimum circumscribing rectangle.
- `validate_packing_inside_rect_wtol(circles: np.array, tol: float = 0.000001)` — [`L63`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py#L63)
- `validate_packing_overlap_wtol(circles: np.ndarray, tol: float = 0.000001)` — [`L52`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py#L52)
- `validate_packing_radii(radii: np.ndarray)` — [`L43`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py#L43)

## Module values
- `BENCHMARK` — [`L21`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py#L21)
- `NUM_CIRCLES` — [`L22`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py#L22)
- `TOL` — [`L23`](../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/circle_packing_rect/evaluator.py#L23)

