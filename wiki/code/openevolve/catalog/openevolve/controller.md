---
title: 'Module: openevolve/controller.py'
type: catalog
provenance: extracted
module: openevolve/controller.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.controller`/
symbols:
  OpenEvolve.run: OpenEvolve#run().
  OpenEvolve.database: OpenEvolve#database.
  OpenEvolve._save_checkpoint: OpenEvolve#_save_checkpoint().
  OpenEvolve.config: OpenEvolve#config.
  OpenEvolve._save_best_program: OpenEvolve#_save_best_program().
  OpenEvolve: OpenEvolve#
  OpenEvolve.output_dir: OpenEvolve#output_dir.
  OpenEvolve._run_evolution_with_checkpoints: OpenEvolve#_run_evolution_with_checkpoints().
  OpenEvolve.evolution_tracer: OpenEvolve#evolution_tracer.
  logger: logger.
  OpenEvolve.evaluator_prompt_sampler: OpenEvolve#evaluator_prompt_sampler.
  OpenEvolve.evaluator: OpenEvolve#evaluator.
  OpenEvolve.evaluation_file: OpenEvolve#evaluation_file.
  OpenEvolve._setup_manual_mode_queue: OpenEvolve#_setup_manual_mode_queue().
  OpenEvolve.initial_program_code: OpenEvolve#initial_program_code.
  OpenEvolve.file_extension: OpenEvolve#file_extension.
  OpenEvolve._log_iteration: OpenEvolve#_log_iteration().
  OpenEvolve._setup_logging: OpenEvolve#_setup_logging().
  OpenEvolve.signal_handler: OpenEvolve#signal_handler().
  OpenEvolve.llm_ensemble: OpenEvolve#llm_ensemble.
  OpenEvolve.llm_evaluator_ensemble: OpenEvolve#llm_evaluator_ensemble.
  OpenEvolve.parallel_controller: OpenEvolve#parallel_controller.
  OpenEvolve._load_checkpoint: OpenEvolve#_load_checkpoint().
  OpenEvolve.prompt_sampler: OpenEvolve#prompt_sampler.
  OpenEvolve._load_initial_program: OpenEvolve#_load_initial_program().
  OpenEvolve.force_exit_handler: OpenEvolve#force_exit_handler().
  OpenEvolve.__init__: OpenEvolve#__init__().
  OpenEvolve.initial_program_path: OpenEvolve#initial_program_path.
  _format_metrics: _format_metrics().
  _format_improvement: _format_improvement().
---
# Module: [`openevolve/controller.py`](../../../../../raw/code/openevolve/openevolve/controller.py)

## Classes
### `OpenEvolve`
- def: [`openevolve/controller.py:56`](../../../../../raw/code/openevolve/openevolve/controller.py#L56) — documented in [openevolve-api](../../concepts/openevolve-api.md)
- doc: Main controller for OpenEvolve
- signature: `class OpenEvolve:`
- members:
  - `_load_checkpoint(self, checkpoint_path: str)` — [`L498`](../../../../../raw/code/openevolve/openevolve/controller.py#L498) — Load state from a checkpoint directory
  - `_load_initial_program(self)` — [`L244`](../../../../../raw/code/openevolve/openevolve/controller.py#L244) — Load the initial program from file
  - `_log_iteration(self, iteration: int, parent: Program, child: Program, elapsed_time: float)` — [`L415`](../../../../../raw/code/openevolve/openevolve/controller.py#L415) — Log iteration progress
  - `_run_evolution_with_checkpoints(self, start_iteration: int, max_iterations: int, target_score: Optional[float])` — [`L507`](../../../../../raw/code/openevolve/openevolve/controller.py#L507) — Run evolution with checkpoint saving support — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `_save_best_program(self, program: Optional[Program] = None)` — [`L534`](../../../../../raw/code/openevolve/openevolve/controller.py#L534) — Save the best program — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `_save_checkpoint(self, iteration: int)` — [`L441`](../../../../../raw/code/openevolve/openevolve/controller.py#L441) — Save a checkpoint — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `_setup_logging(self)` — [`L191`](../../../../../raw/code/openevolve/openevolve/controller.py#L191) — Set up logging
  - `_setup_manual_mode_queue(self)` — [`L215`](../../../../../raw/code/openevolve/openevolve/controller.py#L215) — Set up manual task queue directory if llm.manual_mode is enabled
  - `force_exit_handler(signum, frame)` — [`L344`](../../../../../raw/code/openevolve/openevolve/controller.py#L344)
  - `run(self, iterations: Optional[int] = None, target_score: Optional[float] = None, checkpoint_path: Optional[str] = None)` — [`L249`](../../../../../raw/code/openevolve/openevolve/controller.py#L249) — Run the evolution process with improved parallel processing — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `signal_handler(signum, frame)` — [`L339`](../../../../../raw/code/openevolve/openevolve/controller.py#L339)
  - `config` — [`L78`](../../../../../raw/code/openevolve/openevolve/controller.py#L78) — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `database` — [`L152`](../../../../../raw/code/openevolve/openevolve/controller.py#L152) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `evaluation_file` — [`L162`](../../../../../raw/code/openevolve/openevolve/controller.py#L162)
  - `evaluator` — [`L154`](../../../../../raw/code/openevolve/openevolve/controller.py#L154)
  - `evaluator_prompt_sampler` — [`L144`](../../../../../raw/code/openevolve/openevolve/controller.py#L144) — documented in [openevolve-config](../../concepts/openevolve-config.md)
  - `evolution_tracer` — [`L175`](../../../../../raw/code/openevolve/openevolve/controller.py#L175)
  - `file_extension` — [`L126`](../../../../../raw/code/openevolve/openevolve/controller.py#L126)
  - `initial_program_code` — [`L121`](../../../../../raw/code/openevolve/openevolve/controller.py#L121)
  - `initial_program_path` — [`L120`](../../../../../raw/code/openevolve/openevolve/controller.py#L120)
  - `llm_ensemble` — [`L140`](../../../../../raw/code/openevolve/openevolve/controller.py#L140) — documented in [openevolve-llm-ensemble](../../concepts/openevolve-llm-ensemble.md)
  - `llm_evaluator_ensemble` — [`L141`](../../../../../raw/code/openevolve/openevolve/controller.py#L141) — documented in [openevolve-llm-ensemble](../../concepts/openevolve-llm-ensemble.md)
  - `output_dir` — [`L81`](../../../../../raw/code/openevolve/openevolve/controller.py#L81)
  - `parallel_controller` — [`L189`](../../../../../raw/code/openevolve/openevolve/controller.py#L189)
  - `prompt_sampler` — [`L143`](../../../../../raw/code/openevolve/openevolve/controller.py#L143)
- protocol/private: `__init__`[`L70`](../../../../../raw/code/openevolve/openevolve/controller.py#L70)
- uses (calls/refs, reference-scoped): [`id`](database.md#Program.id), [`add`](database.md#ProgramDatabase.add), [`metrics`](database.md#Program.metrics), [`Program`](database.md#Program), [`programs`](database.md#ProgramDatabase.programs), [`code`](database.md#Program.code), [`Config`](config.md#Config), [`database`](config.md#Config.database), [`llm`](config.md#Config.llm), [`ProgramDatabase`](database.md#ProgramDatabase), [`language`](database.md#Program.language), [`run_evolution`](process_parallel.md#ProcessParallelController.run_evolution), [`evaluate_program`](evaluator.md#Evaluator.evaluate_program), [`load`](database.md#ProgramDatabase.load), [`evaluator`](config.md#Config.evaluator), [`models`](config.md#LLMConfig.models), [`save`](database.md#ProgramDatabase.save), [`prompt`](config.md#Config.prompt), [`best_program_id`](database.md#ProgramDatabase.best_program_id), [`close`](evolution_trace.md#EvolutionTracer.close), [`num_islands`](config.md#DatabaseConfig.num_islands), [`generation`](database.md#Program.generation), [`parent_id`](database.md#Program.parent_id), [`Evaluator`](evaluator.md#Evaluator), [`get_best_program`](database.md#ProgramDatabase.get_best_program), [`logger`](controller.md#logger), [`get`](database.md#ProgramDatabase.get), [`start`](process_parallel.md#ProcessParallelController.start), [`evolution_trace`](config.md#Config.evolution_trace), [`PromptSampler`](prompt/sampler.md#PromptSampler), [`iteration_found`](database.md#Program.iteration_found), [`last_iteration`](database.md#ProgramDatabase.last_iteration), [`ProcessParallelController`](process_parallel.md#ProcessParallelController), [`evaluator_models`](config.md#LLMConfig.evaluator_models), [`LLMEnsemble`](llm/ensemble.md#LLMEnsemble), [`max_iterations`](config.md#Config.max_iterations), [`log_island_status`](database.md#ProgramDatabase.log_island_status), [`checkpoint_interval`](config.md#Config.checkpoint_interval), [`changes_description`](database.md#Program.changes_description), [`language`](config.md#Config.language)  (+26 more)
- used by: [`_run_evolution_async`](api.md#_run_evolution_async), [`main_async`](cli.md#main_async)  (18 test-only)

## Functions
- `_format_improvement(improvement: Dict[str, Any])` — [`L42`](../../../../../raw/code/openevolve/openevolve/controller.py#L42) — Safely format improvement metrics
- `_format_metrics(metrics: Dict[str, Any])` — [`L28`](../../../../../raw/code/openevolve/openevolve/controller.py#L28) — Safely format metrics, handling both numeric and string values

## Module values
- `logger` — [`L25`](../../../../../raw/code/openevolve/openevolve/controller.py#L25)

