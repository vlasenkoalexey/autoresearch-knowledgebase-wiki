---
title: 'Module: openevolve/evaluator.py'
type: catalog
provenance: extracted
module: openevolve/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.evaluator`/
symbols:
  Evaluator.evaluate_program: Evaluator#evaluate_program().
  Evaluator._cascade_evaluate: Evaluator#_cascade_evaluate().
  Evaluator._llm_evaluate: Evaluator#_llm_evaluate().
  Evaluator: Evaluator#
  logger: logger.
  Evaluator.config: Evaluator#config.
  Evaluator._process_evaluation_result: Evaluator#_process_evaluation_result().
  Evaluator._direct_evaluate: Evaluator#_direct_evaluate().
  Evaluator._pending_artifacts: Evaluator#_pending_artifacts.
  Evaluator.evaluate_function: Evaluator#evaluate_function.
  Evaluator.evaluation_file: Evaluator#evaluation_file.
  Evaluator._create_cascade_error_context: Evaluator#_create_cascade_error_context().
  Evaluator.get_pending_artifacts: Evaluator#get_pending_artifacts().
  Evaluator._validate_cascade_configuration: Evaluator#_validate_cascade_configuration().
  Evaluator.__init__: Evaluator#__init__().
  Evaluator.task_pool: Evaluator#task_pool.
  Evaluator.evaluate_multiple: Evaluator#evaluate_multiple().
  Evaluator._load_evaluation_function: Evaluator#_load_evaluation_function().
  Evaluator.llm_ensemble: Evaluator#llm_ensemble.
  Evaluator._passes_threshold: Evaluator#_passes_threshold().
  Evaluator.database: Evaluator#database.
  Evaluator.run_evaluation: Evaluator#run_evaluation().
  Evaluator.program_suffix: Evaluator#program_suffix.
  Evaluator.prompt_sampler: Evaluator#prompt_sampler.
  Evaluator.run_stage1: Evaluator#run_stage1().
  Evaluator.run_stage2: Evaluator#run_stage2().
  Evaluator.run_stage3: Evaluator#run_stage3().
---
# Module: [`openevolve/evaluator.py`](../../../../../raw/code/openevolve/openevolve/evaluator.py)

## Classes
### `Evaluator`
- def: [`openevolve/evaluator.py:32`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L32) — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
- doc: Evaluates programs and assigns scores
- signature: `class Evaluator:`
- members:
  - `_cascade_evaluate(self, program_path: str)` — [`L360`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L360) — Run cascade evaluation with increasingly challenging test cases — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `_create_cascade_error_context(self, stage: str, error: Exception)` — [`L644`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L644) — Create rich error context for cascade failures — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `_direct_evaluate(self, program_path: str)` — [`L331`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L331) — Directly evaluate a program using the evaluation function with timeout — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `_llm_evaluate(self, program_code: str, program_id: str = "")` — [`L550`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L550) — Use LLM to evaluate code quality — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `_load_evaluation_function(self)` — [`L67`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L67) — Load the evaluation function from the evaluation file
  - `_passes_threshold(self, metrics: Dict[str, float], threshold: float)` — [`L668`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L668) — Check if metrics pass a threshold
  - `_process_evaluation_result(self, result: Any)` — [`L298`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L298) — Process evaluation result to handle both dict and EvaluationResult returns — documented in [openevolve-evaluation_result](../../concepts/openevolve-evaluation_result.md)
  - `_validate_cascade_configuration(self, module)` — [`L101`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L101) — Validate cascade evaluation configuration and warn about potential issues
  - `evaluate_multiple(self, programs: List[Tuple[str, str]])` — [`L709`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L709) — Evaluate multiple programs in parallel
  - `evaluate_program(self, program_code: str, program_id: str = "")` — [`L132`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L132) — Evaluate a program and return scores — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `get_pending_artifacts(self, program_id: str)` — [`L319`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L319) — Get and clear pending artifacts for a program
  - `run_evaluation()` — [`L349`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L349)
  - `run_stage1()` — [`L394`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L394)
  - `run_stage2()` — [`L435`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L435)
  - `run_stage3()` — [`L497`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L497)
  - `config` — [`L49`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L49) — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `database` — [`L54`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L54)
  - `evaluate_function` — [`L92`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L92)
  - `evaluation_file` — [`L50`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L50)
  - `llm_ensemble` — [`L52`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L52)
  - `program_suffix` — [`L51`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L51)
  - `prompt_sampler` — [`L53`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L53)
  - `task_pool` — [`L57`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L57)
- protocol/private: `__init__`[`L40`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L40), `_pending_artifacts`[`L63`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L63)
- uses (calls/refs, reference-scoped): [`metrics`](evaluation_result.md#EvaluationResult.metrics), [`EvaluationResult`](evaluation_result.md#EvaluationResult), [`artifacts`](evaluation_result.md#EvaluationResult.artifacts), [`ProgramDatabase`](database.md#ProgramDatabase), [`config`](database.md#ProgramDatabase.config), [`build_prompt`](prompt/sampler.md#PromptSampler.build_prompt), [`feature_dimensions`](config.md#DatabaseConfig.feature_dimensions), [`logger`](evaluator.md#logger), [`cascade_evaluation`](config.md#EvaluatorConfig.cascade_evaluation), [`timeout`](config.md#EvaluatorConfig.timeout), [`EvaluatorConfig`](config.md#EvaluatorConfig), [`PromptSampler`](prompt/sampler.md#PromptSampler), [`LLMEnsemble`](llm/ensemble.md#LLMEnsemble), [`weights`](llm/ensemble.md#LLMEnsemble.weights), [`parallel_evaluations`](config.md#EvaluatorConfig.parallel_evaluations), [`log_prompt`](database.md#ProgramDatabase.log_prompt), [`format_metrics_safe`](utils/format_utils.md#format_metrics_safe), [`has_artifacts`](evaluation_result.md#EvaluationResult.has_artifacts), [`max_retries`](config.md#EvaluatorConfig.max_retries), [`create_task`](utils/async_utils.md#TaskPool.create_task), [`generate_all_with_context`](llm/ensemble.md#LLMEnsemble.generate_all_with_context), [`from_dict`](evaluation_result.md#EvaluationResult.from_dict), [`cascade_thresholds`](config.md#EvaluatorConfig.cascade_thresholds), [`TaskPool`](utils/async_utils.md#TaskPool), [`llm_feedback_weight`](config.md#EvaluatorConfig.llm_feedback_weight), [`use_llm_feedback`](config.md#EvaluatorConfig.use_llm_feedback)
- used by: [`run_iteration_with_shared_db`](iteration.md#run_iteration_with_shared_db), [`run`](controller.md#OpenEvolve.run), [`_run_iteration_worker`](process_parallel.md#_run_iteration_worker), [`_lazy_init_worker_components`](process_parallel.md#_lazy_init_worker_components), [`evaluator`](controller.md#OpenEvolve.evaluator)  (25 test-only)

## Module values
- `logger` — [`L29`](../../../../../raw/code/openevolve/openevolve/evaluator.py#L29)

