---
title: 'Module: examples/llm_prompt_optimization/evaluator.py'
type: catalog
provenance: extracted
module: examples/llm_prompt_optimization/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.llm_prompt_optimization.evaluator`/
symbols:
  dataset_filename: dataset_filename.
  evaluate_prompt: evaluate_prompt().
  evaluate_stage2: evaluate_stage2().
  TASK_MODEL_NAME: TASK_MODEL_NAME.
  evaluate_stage1: evaluate_stage1().
  models: models.
  MAX_TOKENS: MAX_TOKENS.
  llm_config: llm_config.
  DATASET_CONFIG_PATH: DATASET_CONFIG_PATH.
  test_model: test_model.
  MAX_RETRIES: MAX_RETRIES.
  config: config.
  prompt_file: prompt_file.
  load_prompt_config: load_prompt_config().
  calculate_prompt_features: calculate_prompt_features().
  api_base: api_base.
  evaluator_config: evaluator_config.
  basename: basename.
  evaluator_dir: evaluator_dir.
  evaluate: evaluate().
  load_hf_dataset: load_hf_dataset().
  f: f.
---
# Module: [`examples/llm_prompt_optimization/evaluator.py`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py)

## Functions
- `calculate_prompt_features(prompt)` — [`L62`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L62) — Calculate custom features for MAP-Elites
- `evaluate(prompt_path)` — [`L596`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L596) — Main evaluation function - for backwards compatibility
- `evaluate_prompt(prompt, dataset, config, num_samples)` — [`L211`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L211) — Evaluate a prompt on a subset of the dataset.
- `evaluate_stage1(prompt_path)` — [`L456`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L456) — Stage 1 evaluation: Quick evaluation with 10% of samples
- `evaluate_stage2(prompt_path)` — [`L526`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L526) — Stage 2 evaluation: Full evaluation with all samples
- `load_hf_dataset(config)` — [`L152`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L152) — Load HuggingFace dataset based on configuration.
- `load_prompt_config(prompt_path)` — [`L136`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L136) — Load the prompt from text file and dataset config from matching _dataset.yaml file.

## Module values
- `DATASET_CONFIG_PATH` — [`L50`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L50)
- `MAX_RETRIES` — [`L33`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L33)
- `MAX_TOKENS` — [`L36`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L36)
- `TASK_MODEL_NAME` — [`L26`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L26)
- `api_base` — [`L20`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L20)
- `basename` — [`L53`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L53)
- `config` — [`L16`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L16)
- `dataset_filename` — [`L54`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L54)
- `evaluator_config` — [`L32`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L32)
- `evaluator_dir` — [`L49`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L49)
- `f` — [`L15`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L15)
- `llm_config` — [`L19`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L19)
- `models` — [`L23`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L23)
- `prompt_file` — [`L46`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L46)
- `test_model` — [`L40`](../../../../../../raw/code/openevolve/examples/llm_prompt_optimization/evaluator.py#L40)

