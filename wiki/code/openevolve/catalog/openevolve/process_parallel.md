---
title: 'Module: openevolve/process_parallel.py'
type: catalog
provenance: extracted
module: openevolve/process_parallel.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.process_parallel`/
symbols:
  _run_iteration_worker: _run_iteration_worker().
  ProcessParallelController.run_evolution: ProcessParallelController#run_evolution().
  ProcessParallelController._serialize_config: ProcessParallelController#_serialize_config().
  ProcessParallelController._warned_about_combined_score: ProcessParallelController#_warned_about_combined_score.
  ProcessParallelController._submit_iteration: ProcessParallelController#_submit_iteration().
  logger: logger.
  _worker_init: _worker_init().
  _lazy_init_worker_components: _lazy_init_worker_components().
  ProcessParallelController._create_database_snapshot: ProcessParallelController#_create_database_snapshot().
  ProcessParallelController.config: ProcessParallelController#config.
  ProcessParallelController.start: ProcessParallelController#start().
  ProcessParallelController.database: ProcessParallelController#database.
  ProcessParallelController: ProcessParallelController#
  SerializableResult: SerializableResult#
  ProcessParallelController.num_islands: ProcessParallelController#num_islands.
  SerializableResult.iteration: SerializableResult#iteration.
  ProcessParallelController.executor: ProcessParallelController#executor.
  SerializableResult.error: SerializableResult#error.
  ProcessParallelController.stop: ProcessParallelController#stop().
  ProcessParallelController.shutdown_event: ProcessParallelController#shutdown_event.
  ProcessParallelController.num_workers: ProcessParallelController#num_workers.
  ProcessParallelController.request_shutdown: ProcessParallelController#request_shutdown().
  SerializableResult.child_program_dict: SerializableResult#child_program_dict.
  ProcessParallelController.__init__: ProcessParallelController#__init__().
  ProcessParallelController.early_stopping_triggered: ProcessParallelController#early_stopping_triggered.
  SerializableResult.parent_id: SerializableResult#parent_id.
  SerializableResult.iteration_time: SerializableResult#iteration_time.
  ProcessParallelController.evolution_tracer: ProcessParallelController#evolution_tracer.
  ProcessParallelController.file_suffix: ProcessParallelController#file_suffix.
  SerializableResult.prompt: SerializableResult#prompt.
  SerializableResult.llm_response: SerializableResult#llm_response.
  SerializableResult.artifacts: SerializableResult#artifacts.
  SerializableResult.target_island: SerializableResult#target_island.
  ProcessParallelController.evaluation_file: ProcessParallelController#evaluation_file.
---
# Module: [`openevolve/process_parallel.py`](../../../../../raw/code/openevolve/openevolve/process_parallel.py)

## Classes
### `ProcessParallelController`
- def: [`openevolve/process_parallel.py:335`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L335)
- doc: Controller for process-based parallel evolution
- signature: `class ProcessParallelController:`
- members:
  - `_create_database_snapshot(self)` — [`L442`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L442) — Create a serializable snapshot of the database state
  - `_serialize_config(self, config: Config)` — [`L362`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L362) — Serialize config object to a dictionary that can be pickled — documented in [openevolve-config](../../concepts/openevolve-config.md)
  - `_submit_iteration(self, iteration: int, island_id: Optional[int] = None)` — [`L796`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L796) — Submit an iteration to the process pool, optionally pinned to a specific island — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `request_shutdown(self)` — [`L437`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L437) — Request graceful shutdown
  - `run_evolution(self, start_iteration: int, max_iterations: int, target_score: Optional[float] = None, checkpoint_callback=None)` — [`L472`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L472) — Run evolution with process-based parallelism — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `start(self)` — [`L396`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L396) — Start the process pool — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `stop(self)` — [`L427`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L427) — Stop the process pool
  - `config` — [`L346`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L346)
  - `database` — [`L348`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L348) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `early_stopping_triggered` — [`L354`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L354)
  - `evaluation_file` — [`L347`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L347)
  - `evolution_tracer` — [`L349`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L349)
  - `executor` — [`L352`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L352)
  - `file_suffix` — [`L350`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L350)
  - `num_islands` — [`L358`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L358)
  - `num_workers` — [`L357`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L357)
  - `shutdown_event` — [`L353`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L353)
- protocol/private: `__init__`[`L338`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L338), `_warned_about_combined_score`[`L645`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L645)
- uses (calls/refs, reference-scoped): [`id`](database.md#Program.id), [`add`](database.md#ProgramDatabase.add), [`metrics`](database.md#Program.metrics), [`Program`](database.md#Program), [`programs`](database.md#ProgramDatabase.programs), [`Config`](config.md#Config), [`database`](config.md#Config.database), [`llm`](config.md#Config.llm), [`_run_iteration_worker`](process_parallel.md#_run_iteration_worker), [`ProgramDatabase`](database.md#ProgramDatabase), [`islands`](database.md#ProgramDatabase.islands), [`metadata`](database.md#Program.metadata), [`config`](database.md#ProgramDatabase.config), [`migrate_programs`](database.md#ProgramDatabase.migrate_programs), [`evaluator`](config.md#Config.evaluator), [`models`](config.md#LLMConfig.models), [`sample_from_island`](database.md#ProgramDatabase.sample_from_island), [`prompt`](config.md#Config.prompt), [`best_program_id`](database.md#ProgramDatabase.best_program_id), [`current_island`](database.md#ProgramDatabase.current_island), [`feature_dimensions`](config.md#DatabaseConfig.feature_dimensions), [`num_islands`](config.md#DatabaseConfig.num_islands), [`store_artifacts`](database.md#ProgramDatabase.store_artifacts), [`logger`](process_parallel.md#logger), [`get_best_program`](database.md#ProgramDatabase.get_best_program), [`api_key`](config.md#LLMModelConfig.api_key), [`_worker_init`](process_parallel.md#_worker_init), [`get`](database.md#ProgramDatabase.get), [`timeout`](config.md#EvaluatorConfig.timeout), [`get_artifacts`](database.md#ProgramDatabase.get_artifacts), [`evaluator_models`](config.md#LLMConfig.evaluator_models), [`max_iterations`](config.md#Config.max_iterations), [`log_island_status`](database.md#ProgramDatabase.log_island_status), [`checkpoint_interval`](config.md#Config.checkpoint_interval), [`max_snapshot_artifacts`](config.md#DatabaseConfig.max_snapshot_artifacts), [`should_migrate`](database.md#ProgramDatabase.should_migrate), [`early_stopping_patience`](config.md#Config.early_stopping_patience), [`language`](config.md#Config.language), [`safe_numeric_average`](utils/metrics_utils.md#safe_numeric_average), [`parallel_evaluations`](config.md#EvaluatorConfig.parallel_evaluations)  (+20 more)
- used by: [`run`](controller.md#OpenEvolve.run), [`_run_evolution_with_checkpoints`](controller.md#OpenEvolve._run_evolution_with_checkpoints), [`signal_handler`](controller.md#OpenEvolve.signal_handler)  (12 test-only)

### `SerializableResult`
- def: [`openevolve/process_parallel.py:25`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L25)
- doc: Result that can be pickled and sent between processes
- signature: `class SerializableResult:`
- members:
  - `artifacts` — [`L33`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L33)
  - `child_program_dict` — [`L28`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L28)
  - `error` — [`L35`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L35)
  - `iteration` — [`L34`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L34)
  - `iteration_time` — [`L30`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L30)
  - `llm_response` — [`L32`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L32)
  - `parent_id` — [`L29`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L29)
  - `prompt` — [`L31`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L31)
  - `target_island` — [`L36`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L36)
- used by: [`_run_iteration_worker`](process_parallel.md#_run_iteration_worker)  (2 test-only)

## Functions
- `_lazy_init_worker_components()` — [`L98`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L98) — Lazily initialize expensive components on first use — documented in [openevolve-config](../../concepts/openevolve-config.md)
- `_run_iteration_worker(iteration: int, db_snapshot: Dict[str, Any], parent_id: str, inspiration_ids: List[str])` — [`L134`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L134) — Run a single iteration in a worker process — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
- `_worker_init(config_dict: dict, evaluation_file: str, parent_env: dict = None)` — [`L39`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L39) — Initialize worker process with necessary components — documented in [openevolve-config](../../concepts/openevolve-config.md)

## Module values
- `logger` — [`L21`](../../../../../raw/code/openevolve/openevolve/process_parallel.py#L21)

