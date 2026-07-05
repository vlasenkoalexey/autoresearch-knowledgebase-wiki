---
title: 'Module: examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py'
type: catalog
provenance: extracted
module: examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.alphaevolve_math_problems.hexagon_packing.11.evaluator`/
symbols:
  polygons_intersect: polygons_intersect().
  evaluate: evaluate().
  hexagons_are_disjoint: hexagons_are_disjoint().
  all_hexagons_contained: all_hexagons_contained().
  verify_construction: verify_construction().
  get_normals: get_normals().
  hexagon_vertices: hexagon_vertices().
  is_inside_hexagon: is_inside_hexagon().
  N_HEX: N_HEX.
  project_polygon: project_polygon().
  BENCHMARK: BENCHMARK.
  normalize_vector: normalize_vector().
  overlap_1d: overlap_1d().
---
# Module: [`examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py)

## Functions
- `all_hexagons_contained(inner_hex_params_list: list[tuple[float, float, float, float]], outer_hex_params: tuple[float, float, float, float], tol: float = 0.000001)` — [`L135`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L135) — Checks if all inner hexagons are contained within the outer hexagon.
- `evaluate(program_path: str)` — [`L186`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L186)
- `get_normals(vertices: list[tuple[float, float]])` — [`L58`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L58) — Gets the outward normals of a polygon's edges.
- `hexagon_vertices(center_x: float, center_y: float, side_length: float, angle_degrees: float)` — [`L27`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L27) — Generates the vertices of a regular hexagon.
- `hexagons_are_disjoint(hex1_params: tuple[float, float, float, float], hex2_params: tuple[float, float, float, float], tol: float = 0.000001)` — [`L106`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L106) — Determines if two hexagons are disjoint given their parameters.
- `is_inside_hexagon(point: tuple[float, float], hex_params: tuple[float, float, float, float], tol: float = 0.000001)` — [`L117`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L117) — Checks if a point is inside a hexagon (given its parameters).
- `normalize_vector(v: tuple[float, float])` — [`L52`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L52) — Normalizes a 2D vector.
- `overlap_1d(min1: float, max1: float, min2: float, max2: float, tol: float = 0.000001)` — [`L84`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L84) — Determines whether two 1D intervals overlap, allowing for numerical tolerance.
- `polygons_intersect(vertices1: list[tuple[float, float]], vertices2: list[tuple[float, float]], tol: float = 0.000001)` — [`L89`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L89) — Determines if two polygons intersect using the Separating Axis Theorem.
- `project_polygon(vertices: list[tuple[float, float]], axis: tuple[float, float])` — [`L70`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L70) — Projects a polygon onto an axis and returns the min/max values.
- `verify_construction(inner_hex_data: tuple[float, float, float], outer_hex_center: tuple[float, float], outer_hex_side_length: float, outer_hex_angle_degrees: float, tol: float = 0.000001)` — [`L149`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L149) — Verifies the hexagon packing construction with a rotated outer hexagon.

## Module values
- `BENCHMARK` — [`L24`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L24)
- `N_HEX` — [`L23`](../../../../../../../../raw/code/openevolve/examples/alphaevolve_math_problems/hexagon_packing/11/evaluator.py#L23)

