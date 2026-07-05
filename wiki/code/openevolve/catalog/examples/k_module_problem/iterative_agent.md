---
title: 'Module: examples/k_module_problem/iterative_agent.py'
type: catalog
provenance: extracted
module: examples/k_module_problem/iterative_agent.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.k_module_problem.iterative_agent`/
symbols:
  run_iterative_refinement: run_iterative_refinement().
  create_improvement_prompt: create_improvement_prompt().
  main: main().
  load_config: load_config().
  read_program: read_program().
  write_program: write_program().
  extract_code_block: extract_code_block().
  format_rich_feedback: format_rich_feedback().
  SYSTEM_PROMPT: SYSTEM_PROMPT.
---
# Module: [`examples/k_module_problem/iterative_agent.py`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py)

## Functions
- `create_improvement_prompt(current_code: str, metrics: dict, artifacts: dict, iteration: int, history: list)` — [`L87`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L87) — Create prompt asking LLM to improve the program.
- `extract_code_block(response: str)` — [`L37`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L37) — Extract Python code from LLM response.
- `format_rich_feedback(artifacts: dict)` — [`L67`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L67) — Format rich feedback if available (RICH_FEEDBACK=1).
- `load_config(config_path: str = "config.yaml")` — [`L31`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L31) — Load configuration from YAML file.
- `main()` — [`L315`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L315)
- `read_program(program_path: str)` — [`L55`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L55) — Read program from file.
- `run_iterative_refinement(initial_program: str, evaluator_path: str, config: dict, max_iterations: int = 100, output_dir: str = "iterative_output")` — [`L161`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L161) — Run iterative refinement loop.
- `write_program(program_path: str, code: str)` — [`L61`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L61) — Write program to file.

## Module values
- `SYSTEM_PROMPT` — [`L148`](../../../../../../raw/code/openevolve/examples/k_module_problem/iterative_agent.py#L148)

