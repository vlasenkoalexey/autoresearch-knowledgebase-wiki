---
title: 'Module: examples/k_module_problem/run_random_baseline.py'
type: catalog
provenance: extracted
module: examples/k_module_problem/run_random_baseline.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.k_module_problem.run_random_baseline`/
symbols:
  main: main().
  run_random_search: run_random_search().
  generate_random_config: generate_random_config().
  score_config: score_config().
  run_multiple_trials: run_multiple_trials().
  theoretical_pass_at_k: theoretical_pass_at_k().
  calculate_pass_at_k: calculate_pass_at_k().
---
# Module: [`examples/k_module_problem/run_random_baseline.py`](../../../../../../raw/code/openevolve/examples/k_module_problem/run_random_baseline.py)

## Functions
- `calculate_pass_at_k(trial_results: list, k_values: list)` — [`L95`](../../../../../../raw/code/openevolve/examples/k_module_problem/run_random_baseline.py#L95) — Calculate pass@k metrics.
- `generate_random_config()` — [`L28`](../../../../../../raw/code/openevolve/examples/k_module_problem/run_random_baseline.py#L28) — Generate a random pipeline configuration.
- `main()` — [`L125`](../../../../../../raw/code/openevolve/examples/k_module_problem/run_random_baseline.py#L125)
- `run_multiple_trials(num_trials: int, max_samples: int)` — [`L77`](../../../../../../raw/code/openevolve/examples/k_module_problem/run_random_baseline.py#L77) — Run multiple independent trials of random search.
- `run_random_search(max_samples: int)` — [`L44`](../../../../../../raw/code/openevolve/examples/k_module_problem/run_random_baseline.py#L44) — Run random search until solution found or max_samples reached.
- `score_config(config: dict)` — [`L36`](../../../../../../raw/code/openevolve/examples/k_module_problem/run_random_baseline.py#L36) — Score a configuration (number of correct modules).
- `theoretical_pass_at_k(k: int, search_space: int = 625)` — [`L118`](../../../../../../raw/code/openevolve/examples/k_module_problem/run_random_baseline.py#L118) — Calculate theoretical pass@k for uniform random search.

