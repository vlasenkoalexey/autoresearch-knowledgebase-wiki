---
title: 'Module: examples/llm_prompt_optimization/evaluate_prompts.py'
type: catalog
provenance: extracted
module: examples/llm_prompt_optimization/evaluate_prompts.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.llm_prompt_optimization.evaluate_prompts`/
symbols:
  main: main().
  get_client: get_client().
  load_prompt: load_prompt().
  evaluate_ifeval: evaluate_ifeval().
  evaluate_hover: evaluate_hover().
  evaluate_hotpotqa: evaluate_hotpotqa().
  load_dataset_config: load_dataset_config().
---
# Module: [`examples/llm_prompt_optimization/evaluate_prompts.py`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluate_prompts.py)

## Functions
- `evaluate_hotpotqa(client, prompt_template, num_samples, model)` — [`L213`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluate_prompts.py#L213) — Evaluate HotpotQA dataset.
- `evaluate_hover(client, prompt_template, num_samples, model)` — [`L122`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluate_prompts.py#L122) — Evaluate HoVer dataset.
- `evaluate_ifeval(client, prompt_template, num_samples, model)` — [`L49`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluate_prompts.py#L49) — Evaluate IFEval dataset.
- `get_client()` — [`L19`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluate_prompts.py#L19)
- `load_dataset_config(dataset_name)` — [`L41`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluate_prompts.py#L41) — Load dataset configuration.
- `load_prompt(dataset_name, prompt_type="baseline")` — [`L27`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluate_prompts.py#L27) — Load prompt template for a dataset.
- `main()` — [`L301`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluate_prompts.py#L301)

