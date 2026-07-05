---
title: 'Module: examples/mlx_metal_kernel_opt/mlx_lm_generate_with_hook.py'
type: catalog
provenance: extracted
module: examples/mlx_metal_kernel_opt/mlx_lm_generate_with_hook.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.mlx_metal_kernel_opt.mlx_lm_generate_with_hook`/
symbols:
  _apply_hook_from_program: _apply_hook_from_program().
  main: main().
  _load_module_from_path: _load_module_from_path().
---
# Module: [`examples/mlx_metal_kernel_opt/mlx_lm_generate_with_hook.py`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/mlx_lm_generate_with_hook.py)

## Functions
- `_apply_hook_from_program(module_path: str)` — [`L43`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/mlx_lm_generate_with_hook.py#L43) — Load an evolved hook program and apply its attention optimization.
- `_load_module_from_path(module_path: str)` — [`L28`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/mlx_lm_generate_with_hook.py#L28) — Dynamically load a Python module from an arbitrary filesystem path.
- `main(argv: Optional[List[str]] = None)` — [`L82`](../../../../../../raw/code/openevolve/examples/mlx_metal_kernel_opt/mlx_lm_generate_with_hook.py#L82) — Entry point: parse CLI arguments, apply the hook, and run mlx_lm.generate.

