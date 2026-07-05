---
title: 'Module: openevolve/api.py'
type: catalog
provenance: extracted
module: openevolve/api.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.api`/
symbols:
  _run_evolution_async: _run_evolution_async().
  EvolutionResult.best_score: EvolutionResult#best_score.
  EvolutionResult: EvolutionResult#
  run_evolution: run_evolution().
  EvolutionResult.output_dir: EvolutionResult#output_dir.
  EvolutionResult.best_code: EvolutionResult#best_code.
  evolve_function: evolve_function().
  EvolutionResult.best_program: EvolutionResult#best_program.
  evolve_code: evolve_code().
  EvolutionResult.metrics: EvolutionResult#metrics.
  evolve_algorithm: evolve_algorithm().
  _prepare_evaluator: _prepare_evaluator().
  _prepare_program: _prepare_program().
  EvolutionResult.__repr__: EvolutionResult#__repr__().
---
# Module: [`openevolve/api.py`](../../../../../raw/code/openevolve/openevolve/api.py)

## Classes
### `EvolutionResult`
- def: [`openevolve/api.py:20`](../../../../../raw/code/openevolve/openevolve/api.py#L20) — documented in [openevolve-api](../../concepts/openevolve-api.md)
- doc: Result of an evolution run
- signature: `class EvolutionResult:`
- members:
  - `best_code` — [`L25`](../../../../../raw/code/openevolve/openevolve/api.py#L25)
  - `best_program` — [`L23`](../../../../../raw/code/openevolve/openevolve/api.py#L23)
  - `best_score` — [`L24`](../../../../../raw/code/openevolve/openevolve/api.py#L24) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `metrics` — [`L26`](../../../../../raw/code/openevolve/openevolve/api.py#L26)
  - `output_dir` — [`L27`](../../../../../raw/code/openevolve/openevolve/api.py#L27)
- protocol/private: `__repr__`[`L29`](../../../../../raw/code/openevolve/openevolve/api.py#L29)
- uses (calls/refs, reference-scoped): [`Program`](database.md#Program)
- used by: [`_run_evolution_async`](api.md#_run_evolution_async), [`run_evolution`](api.md#run_evolution), [`evolve_function`](api.md#evolve_function), [`evolve_code`](api.md#evolve_code), [`evolve_algorithm`](api.md#evolve_algorithm)  (11 test-only)

## Functions
- `_prepare_evaluator(evaluator: Union[str, Path, Callable], temp_dir: Optional[str], temp_files: List[str])` — [`L237`](../../../../../raw/code/openevolve/openevolve/api.py#L237) — Convert evaluator input to a file path
- `_prepare_program(initial_program: Union[str, Path, List[str]], temp_dir: Optional[str], temp_files: List[str])` — [`L202`](../../../../../raw/code/openevolve/openevolve/api.py#L202) — Convert program input to a file path
- `_run_evolution_async(initial_program: Union[str, Path, List[str]], evaluator: Union[str, Path, Callable], config: Union[str, Path, Config, None], iterations: Optional[int], output_dir: Optional[str], cleanup: bool)` — [`L97`](../../../../../raw/code/openevolve/openevolve/api.py#L97) — Async implementation of run_evolution — documented in [openevolve-api](../../concepts/openevolve-api.md)
- `evolve_algorithm(algorithm_class: type, benchmark: Callable, iterations: int = 100, **kwargs)` — [`L436`](../../../../../raw/code/openevolve/openevolve/api.py#L436) — Evolve an algorithm class based on a benchmark
- `evolve_code(initial_code: str, evaluator: Callable[[str], Dict[str, Any]], iterations: int = 100, **kwargs)` — [`L542`](../../../../../raw/code/openevolve/openevolve/api.py#L542) — Evolve arbitrary code with a custom evaluator
- `evolve_function(func: Callable, test_cases: List[Tuple[Any, Any]], iterations: int = 100, **kwargs)` — [`L314`](../../../../../raw/code/openevolve/openevolve/api.py#L314) — Evolve a Python function based on test cases
- `run_evolution(initial_program: Union[str, Path, List[str]], evaluator: Union[str, Path, Callable], config: Union[str, Path, Config, None] = None, iterations: Optional[int] = None, output_dir: Optional[str] = None, cleanup: bool = True)` — [`L33`](../../../../../raw/code/openevolve/openevolve/api.py#L33) — Run evolution with flexible inputs - the main library API — documented in [openevolve-api](../../concepts/openevolve-api.md)

