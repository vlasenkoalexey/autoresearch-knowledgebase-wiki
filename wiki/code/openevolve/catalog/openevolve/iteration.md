---
title: 'Module: openevolve/iteration.py'
type: catalog
provenance: extracted
module: openevolve/iteration.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.iteration`/
symbols:
  run_iteration_with_shared_db: run_iteration_with_shared_db().
  Result.child_metrics: Result#child_metrics.
  Result: Result#
  Result.child_program: Result#child_program.
  Result.parent: Result#parent.
  Result.iteration_time: Result#iteration_time.
  Result.prompt: Result#prompt.
  Result.llm_response: Result#llm_response.
  Result.artifacts: Result#artifacts.
---
# Module: [`openevolve/iteration.py`](../../../../../raw/code/openevolve/openevolve/iteration.py)

## Classes
### `Result`
- def: [`openevolve/iteration.py:24`](../../../../../raw/code/openevolve/openevolve/iteration.py#L24)
- doc: Resulting program and metrics from an iteration of OpenEvolve
- signature: `class Result:`
- members:
  - `artifacts` — [`L33`](../../../../../raw/code/openevolve/openevolve/iteration.py#L33)
  - `child_metrics` — [`L29`](../../../../../raw/code/openevolve/openevolve/iteration.py#L29)
  - `child_program` — [`L27`](../../../../../raw/code/openevolve/openevolve/iteration.py#L27)
  - `iteration_time` — [`L30`](../../../../../raw/code/openevolve/openevolve/iteration.py#L30)
  - `llm_response` — [`L32`](../../../../../raw/code/openevolve/openevolve/iteration.py#L32)
  - `parent` — [`L28`](../../../../../raw/code/openevolve/openevolve/iteration.py#L28)
  - `prompt` — [`L31`](../../../../../raw/code/openevolve/openevolve/iteration.py#L31)
- used by: [`run_iteration_with_shared_db`](iteration.md#run_iteration_with_shared_db)

## Functions
- `run_iteration_with_shared_db(iteration: int, config: Config, database: ProgramDatabase, evaluator: Evaluator, llm_ensemble: LLMEnsemble, prompt_sampler: PromptSampler)` — [`L36`](../../../../../raw/code/openevolve/openevolve/iteration.py#L36) — Run a single iteration using shared memory database — documented in [openevolve-config](../../concepts/openevolve-config.md)

