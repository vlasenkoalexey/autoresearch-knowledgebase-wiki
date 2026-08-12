---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.solvers.evo.evo`/
symbols:
  Evolutionary.search: Evolutionary#search().
  Evolutionary.parse_eval_result: Evolutionary#parse_eval_result().
  Evolutionary._draft: Evolutionary#_draft().
  Evolutionary._improve: Evolutionary#_improve().
  Evolutionary._debug_cycle_async: Evolutionary#_debug_cycle_async().
  SolutionsDatabase.sample_in_context: SolutionsDatabase#sample_in_context().
  Evolutionary._async_worker_loop: Evolutionary#_async_worker_loop().
  Evolutionary.root_node: Evolutionary#root_node.
  Evolutionary._debug: Evolutionary#_debug().
  Evolutionary._crossover: Evolutionary#_crossover().
  Evolutionary._next_async_work_item: Evolutionary#_next_async_work_item().
  SolutionsDatabase.add_nodes_to_islands: SolutionsDatabase#add_nodes_to_islands().
  Evolutionary.create_root_node: Evolutionary#create_root_node().
  Evolutionary.debug_cycle: Evolutionary#debug_cycle().
  Evolutionary._create_node_from_work_item: Evolutionary#_create_node_from_work_item().
  Evolutionary._commit_async_node: Evolutionary#_commit_async_node().
  Evolutionary.state: Evolutionary#state.
  SolutionsDatabase._islands: SolutionsDatabase#_islands.
  Evolutionary.journal: Evolutionary#journal.
  Evolutionary.__call__: Evolutionary#__call__().
  Evolutionary._ensure_node_rich_summary_unlocked: Evolutionary#_ensure_node_rich_summary_unlocked().
  Island.register_node_in_island: Island#register_node_in_island().
  Evolutionary._prepare_operator_rich_memory: Evolutionary#_prepare_operator_rich_memory().
  SolutionsDatabase.logger: SolutionsDatabase#logger.
  Evolutionary._should_stop_async_search: Evolutionary#_should_stop_async_search().
  SolutionsDatabase.reset_islands: SolutionsDatabase#reset_islands().
  Island.only_keep_best: Island#only_keep_best().
  Island.remove_lowest: Island#remove_lowest().
  Island.remove_node: Island#remove_node().
  Evolutionary.load_checkpoint: Evolutionary#load_checkpoint().
  Evolutionary._append_evaluated_node: Evolutionary#_append_evaluated_node().
  SolutionsDatabase.seed_islands_with_nodes: SolutionsDatabase#seed_islands_with_nodes().
  SolutionsDatabase.global_max_fitness: SolutionsDatabase#global_max_fitness.
  Island.migrate_node: Island#migrate_node().
  Island.nodes: Island#nodes.
  Evolutionary.log_journal: Evolutionary#log_journal().
  Evolutionary.save_checkpoint: Evolutionary#save_checkpoint().
  SolutionsDatabase._update_global_fitness_range: SolutionsDatabase#_update_global_fitness_range().
  Island.size: Island#size().
  Evolutionary._analyze: Evolutionary#_analyze().
  Evolutionary._seed_solution_database_from_journal: Evolutionary#_seed_solution_database_from_journal().
  Island.fitness_scores: Island#fitness_scores().
  Evolutionary._store_rich_summary: Evolutionary#_store_rich_summary().
  Evolutionary.lower_is_better: Evolutionary#lower_is_better.
  Evolutionary.task_desc: Evolutionary#task_desc.
  Island.fittest_individual: Island#fittest_individual().
  Evolutionary.setup_operators: Evolutionary#setup_operators().
  Evolutionary.draft_fn: Evolutionary#draft_fn.
  Evolutionary.improve_fn: Evolutionary#improve_fn.
  Evolutionary.debug_fn: Evolutionary#debug_fn.
  Evolutionary.crossover_fn: Evolutionary#crossover_fn.
  Evolutionary.update_data_preview: Evolutionary#update_data_preview().
  Evolutionary._new_solution_database: Evolutionary#_new_solution_database().
  SolutionsDatabase.get_normalized_score: SolutionsDatabase#get_normalized_score().
  Evolutionary.memory_op: Evolutionary#memory_op.
  AsyncWorkItem.worker: AsyncWorkItem#worker.
  Evolutionary._rich_memory_cache_path: Evolutionary#_rich_memory_cache_path().
  Evolutionary.run_legacy_analyze: Evolutionary#run_legacy_analyze().
  SolutionsDatabase.last_parent_selection: SolutionsDatabase#last_parent_selection.
  SolutionsDatabase.sample_in_context_with_trace: SolutionsDatabase#sample_in_context_with_trace().
  Evolutionary.debug_memory_op: Evolutionary#debug_memory_op.
  Evolutionary._rich_summary_lock_for_node: Evolutionary#_rich_summary_lock_for_node().
  Evolutionary._ensure_node_rich_summary: Evolutionary#_ensure_node_rich_summary().
  Island.average_fitness_score: Island#average_fitness_score().
  SolutionsDatabase: SolutionsDatabase#
  SolutionsDatabase.lower_is_better: SolutionsDatabase#lower_is_better.
  SolutionsDatabase.global_min_fitness: SolutionsDatabase#global_min_fitness.
  Evolutionary.data_preview: Evolutionary#data_preview.
  AsyncWorkItem.parent_nodes: AsyncWorkItem#parent_nodes.
  Island.island_id: Island#island_id.
  Island.lower_is_better: Island#lower_is_better.
  Island.logger: Island#logger.
  SolutionsDatabase.num_islands: SolutionsDatabase#num_islands.
  Evolutionary.rich_memory_summary_fn: Evolutionary#rich_memory_summary_fn.
  Evolutionary._repeated_debug_failure_reason: Evolutionary#_repeated_debug_failure_reason().
  Evolutionary._restore_solution_database_from_journal: Evolutionary#_restore_solution_database_from_journal().
  Evolutionary._experience_enabled: Evolutionary#_experience_enabled().
  AsyncWorkItem: AsyncWorkItem#
  Island.best_fitness_score: Island#best_fitness_score().
  SolutionsDatabase.has_nodes: SolutionsDatabase#has_nodes().
  SolutionsDatabase.has_island_with_size: SolutionsDatabase#has_island_with_size().
  Evolutionary.analyze_fn: Evolutionary#analyze_fn.
  Evolutionary._rich_memory_cache_dir: Evolutionary#_rich_memory_cache_dir().
  Evolutionary._load_cached_rich_summary: Evolutionary#_load_cached_rich_summary().
  Evolutionary._async_worker_count: Evolutionary#_async_worker_count().
  Evolutionary._execution_mode: Evolutionary#_execution_mode().
  Evolutionary._async_sandbox_urls: Evolutionary#_async_sandbox_urls().
  Evolutionary.search_async_steady_state: Evolutionary#search_async_steady_state().
  AsyncWorkItem.attempt_id: AsyncWorkItem#attempt_id.
  Island.__init__: Island#__init__().
  Island.solution_nodes: Island#solution_nodes().
  Evolutionary.__init__: Evolutionary#__init__().
  Evolutionary.prompt_context: Evolutionary#prompt_context.
  Evolutionary: Evolutionary#
  Evolutionary.linear_decay: Evolutionary#linear_decay().
  Evolutionary.failure_signature: Evolutionary#failure_signature().
  AsyncWorkItem.generation_id: AsyncWorkItem#generation_id.
  AsyncWorkItem.operator: AsyncWorkItem#operator.
  AsyncWorkItem.parent_selection_trace: AsyncWorkItem#parent_selection_trace.
  Evolutionary._normalize_rich_summary: Evolutionary#_normalize_rich_summary().
  Evolutionary._async_attempt_limit: Evolutionary#_async_attempt_limit().
  AsyncWorkItem.temperature: AsyncWorkItem#temperature.
  AsyncWorkItem.island_id: AsyncWorkItem#island_id.
  SolutionsDatabase.max_size: SolutionsDatabase#max_size.
  Evolutionary._task_budget_exempt_seconds: Evolutionary#_task_budget_exempt_seconds().
  SolutionsDatabase.__init__: SolutionsDatabase#__init__().
  Evolutionary.solution_database: Evolutionary#solution_database.
  Island: Island#
  SolutionsDatabase.experience_config: SolutionsDatabase#experience_config.
  SolutionsDatabase.request_fresh_draft: SolutionsDatabase#request_fresh_draft().
  Evolutionary._rich_summary_locks: Evolutionary#_rich_summary_locks.
  Evolutionary._step_task_async: Evolutionary#_step_task_async().
  SolutionsDatabase._forced_fresh_draft_reason: SolutionsDatabase#_forced_fresh_draft_reason.
  Evolutionary._rich_summary_locks_guard: Evolutionary#_rich_summary_locks_guard.
  Evolutionary.coerce_float: Evolutionary#coerce_float().
  Evolutionary.deterministic_failure: Evolutionary#deterministic_failure().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py)

## Classes
### `AsyncWorkItem`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py:82`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L82)
- signature: `class AsyncWorkItem:`
- members:
  - `attempt_id` — [`L83`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L83)
  - `generation_id` — [`L84`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L84)
  - `island_id` — [`L86`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L86)
  - `operator` — [`L87`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L87)
  - `parent_nodes` — [`L88`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L88)
  - `parent_selection_trace` — [`L89`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L89)
  - `temperature` — [`L85`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L85)
  - `worker` — [`L90`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L90) — documented in [OpenMLE-Evo-tts_search-airaevo_async_resources](../../../../../../../../concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md)
- uses (calls/refs, reference-scoped): [`Node`](../../core/solvers/utils/journal.md#Node), [`WorkerSpec`](../../../../../../tts_search/airaevo_async_resources.md#WorkerSpec)
- used by: [`_debug_cycle_async`](evo.md#Evolutionary._debug_cycle_async), [`_async_worker_loop`](evo.md#Evolutionary._async_worker_loop), [`_next_async_work_item`](evo.md#Evolutionary._next_async_work_item), [`_create_node_from_work_item`](evo.md#Evolutionary._create_node_from_work_item), [`_commit_async_node`](evo.md#Evolutionary._commit_async_node)

### `Evolutionary`  ·  implements/extends Solver
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py:749`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L749)
- signature: `class Evolutionary(Solver):`
- members:
  - `_analyze(self, node: Node)` — [`L1112`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1112) — Analyze a node's execution results using the analyze LLM operator.
  - `_append_evaluated_node(self, node: Node)` — [`L1206`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1206) — Append an evaluated node and immediately mirror/log it if not already present.
  - `_debug(self, parent_node: Node)` — [`L1083`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1083) — Debug a buggy solution using the debug LLM operator.
  - `_draft(self)` — [`L1023`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1023) — Generate a new solution from scratch using the draft LLM operator.
  - `_improve(self, parent_node: Node)` — [`L1051`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1051) — Improve an existing solution using the improve LLM operator.
  - `_repeated_debug_failure_reason(debug_path: List[Node])` — [`L1227`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1227) — Identify repeated failures where another repair is unlikely to add information.
  - `_restore_solution_database_from_journal(self)` — [`L1333`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1333) — Create the islands database and restore all resumable journal nodes.
  - `coerce_float(value)` — [`L1776`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1776)
  - `create_root_node(self)` — [`L1897`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1897)
  - `debug_cycle(self, state, task, buggy_node: Node)` — [`L1259`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1259)
  - `deterministic_failure()` — [`L1785`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1785)
  - `failure_signature(node: Node)` — [`L1232`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1232)
  - `linear_decay(self, iteration: int)` — [`L1186`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1186) — defines a temperature schedule for sampling of islands and individuals
  - `load_checkpoint(self)` — [`L795`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L795)
  - `log_journal(self)` — [`L2064`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L2064)
  - `parse_eval_result(self, node: Node, eval_result: Dict[str, Any])` — [`L1747`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1747) — Parse evaluation results and update the node accordingly.
  - `run_legacy_analyze()` — [`L1807`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1807)
  - `save_checkpoint(self)` — [`L784`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L784)
  - `search(self, task, state)` — [`L1910`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1910)
  - `search_async_steady_state(self, task, state, *, worker_count: int)` — [`L1685`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1685)
  - `setup_operators(self)` — [`L811`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L811) — Setup operator LLMs.
  - `update_data_preview(self, state)` — [`L1155`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1155) — Generate a data preview to provide context for the LLM operators.
  - `analyze_fn` — [`L841`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L841)
  - `crossover_fn` — [`L847`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L847)
  - `data_preview` — [`L753`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L753)
  - `debug_fn` — [`L838`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L838)
  - `debug_memory_op` — [`L829`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L829)
  - `draft_fn` — [`L832`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L832)
  - `improve_fn` — [`L835`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L835)
  - `journal` — [`L752`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L752)
  - `lower_is_better` — [`L774`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L774)
  - `memory_op` — [`L828`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L828)
  - `prompt_context` — [`L765`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L765)
  - `rich_memory_summary_fn` — [`L842`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L842)
  - `root_node` — [`L1687`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1687)
  - `solution_database` — [`L1336`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1336)
  - `state` — [`L780`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L780)
  - `task_desc` — [`L755`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L755)
- protocol/private: `__call__`[`L2075`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L2075), `__init__`[`L750`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L750), `_async_attempt_limit`[`L1346`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1346), `_async_sandbox_urls`[`L1353`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1353), `_async_worker_count`[`L1340`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1340), `_async_worker_loop`[`L1587`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1587), `_commit_async_node`[`L1476`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1476), `_create_node_from_work_item`[`L1447`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1447), `_crossover`[`L1131`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1131), `_debug_cycle_async`[`L1512`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1512), `_ensure_node_rich_summary`[`L918`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L918), `_ensure_node_rich_summary_unlocked`[`L924`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L924), `_execution_mode`[`L1343`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1343), `_experience_enabled`[`L1200`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1200), `_load_cached_rich_summary`[`L867`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L867), `_new_solution_database`[`L1310`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1310), `_next_async_work_item`[`L1386`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1386), `_normalize_rich_summary`[`L905`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L905), `_prepare_operator_rich_memory`[`L970`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L970), `_rich_memory_cache_dir`[`L851`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L851), `_rich_memory_cache_path`[`L855`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L855), `_rich_summary_lock_for_node`[`L858`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L858), `_rich_summary_locks`[`L781`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L781), `_rich_summary_locks_guard`[`L782`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L782), `_seed_solution_database_from_journal`[`L1319`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1319), `_should_stop_async_search`[`L1361`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1361), `_step_task_async`[`L1467`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1467), `_store_rich_summary`[`L883`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L883), `_task_budget_exempt_seconds`[`L1216`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1216)
- uses (calls/refs, reference-scoped): [`cfg`](../../core/solvers/base.md#Solver.cfg), [`logger`](../../core/solvers/base.md#Solver.logger), [`Node`](../../core/solvers/utils/journal.md#Node), [`LogEvent`](../../utils/logger.md#LogEvent), [`metric`](../../core/solvers/utils/journal.md#Node.metric), [`from_export_data`](../../core/solvers/utils/journal.md#Journal.from_export_data), [`id`](../../core/solvers/utils/journal.md#Node.id), [`get_node_data`](../../core/solvers/utils/journal.md#Journal.get_node_data), [`code`](../../core/solvers/utils/journal.md#Node.code), [`sample_in_context`](evo.md#SolutionsDatabase.sample_in_context), [`parents`](../../core/solvers/utils/journal.md#Node.parents), [`value`](../../core/solvers/utils/metric.md#MetricValue.value), [`SOLVER`](../../utils/logger.md#LogEvent.SOLVER), [`improve_op`](../../core/solvers/operators/improve.md#improve_op), [`add_nodes_to_islands`](evo.md#SolutionsDatabase.add_nodes_to_islands), [`Journal`](../../core/solvers/utils/journal.md#Journal), [`debug_op`](../../core/solvers/operators/debug.md#debug_op), [`crossover_op`](../../core/solvers/operators/crossover.md#crossover_op), [`nodes`](../../core/solvers/utils/journal.md#Journal.nodes), [`is_buggy`](../../core/solvers/utils/journal.md#Node.is_buggy), [`GenericLLM`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM), [`export_search_results`](../../core/solvers/utils/search_exporter.md#export_search_results), [`plan`](../../core/solvers/utils/journal.md#Node.plan), [`analyze_op`](../../core/solvers/operators/analyze.md#analyze_op), [`step`](../../core/solvers/utils/journal.md#Node.step), [`sanitize_execution_output_for_prompt`](../../core/solvers/utils/response.md#sanitize_execution_output_for_prompt), [`create_memory_op`](../../core/solvers/operators/memory.md#create_memory_op), [`absorb_exec_result`](../../core/solvers/utils/journal.md#Node.absorb_exec_result), [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`build_worker_specs`](../../../../../../tts_search/airaevo_async_resources.md#build_worker_specs), [`get_best_node`](../../core/solvers/utils/journal.md#Journal.get_best_node), [`rich_memory_summary_op`](../../core/solvers/operators/rich_memory_summary.md#rich_memory_summary_op), [`append`](../../core/solvers/utils/journal.md#Journal.append), [`generate`](../../core/solvers/utils/data_preview.md#generate), [`get_complextiy_level`](../utils.md#get_complextiy_level), [`is_root_node`](../../core/solvers/utils/journal.md#Journal.is_root_node), [`collect_operator_memory_nodes`](experience.md#collect_operator_memory_nodes), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`MetricValue`](../../core/solvers/utils/metric.md#MetricValue), [`info`](../../core/solvers/utils/metric.md#MetricValue.info)  (+66 more)
- used by: [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`Solver`](../../core/solvers/base.md#Solver), [`__getattr__`](__init__.md#__getattr__)

### `Island`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py:93`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L93)
- doc: A population of solutions (Nodes) in an island.
- signature: `class Island:`
- members:
  - `average_fitness_score(self)` — [`L136`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L136) — Returns the average fitness score.
  - `best_fitness_score(self)` — [`L126`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L126) — Returns the best fitness score in the island.
  - `fitness_scores(self)` — [`L113`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L113) — Returns fitness scores, using +/- inf for None metrics.
  - `fittest_individual(self)` — [`L153`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L153) — Returns the node with the best fitness score.
  - `migrate_node(self, founder_node: Node)` — [`L226`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L226) — Migrate a node from a founder island to this island.
  - `only_keep_best(self)` — [`L210`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L210) — Remove all nodes except the single best one.
  - `register_node_in_island(self, solution_node: Node)` — [`L166`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L166) — Add a solution Node to the island population.
  - `remove_lowest(self)` — [`L180`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L180) — Removes the node with the worst fitness score in the island.
  - `remove_node(self, to_remove_node: Node)` — [`L196`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L196) — Remove a specific node from the island.
  - `size(self)` — [`L109`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L109)
  - `solution_nodes(self)` — [`L163`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L163)
  - `island_id` — [`L103`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L103)
  - `logger` — [`L105`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L105)
  - `lower_is_better` — [`L104`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L104)
  - `nodes` — [`L106`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L106)
- protocol/private: `__init__`[`L96`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L96)
- uses (calls/refs, reference-scoped): [`Node`](../../core/solvers/utils/journal.md#Node), [`LogEvent`](../../utils/logger.md#LogEvent), [`metric`](../../core/solvers/utils/journal.md#Node.metric), [`id`](../../core/solvers/utils/journal.md#Node.id), [`value`](../../core/solvers/utils/metric.md#MetricValue.value), [`SOLVER`](../../utils/logger.md#LogEvent.SOLVER), [`info`](../../utils/logger.md#CollectiveLogger.info), [`warning`](../../utils/logger.md#CollectiveLogger.warning), [`CollectiveLogger`](../../utils/logger.md#CollectiveLogger)
- used by: [`sample_in_context`](evo.md#SolutionsDatabase.sample_in_context), [`add_nodes_to_islands`](evo.md#SolutionsDatabase.add_nodes_to_islands), [`_islands`](evo.md#SolutionsDatabase._islands), [`reset_islands`](evo.md#SolutionsDatabase.reset_islands), [`seed_islands_with_nodes`](evo.md#SolutionsDatabase.seed_islands_with_nodes), [`global_max_fitness`](evo.md#SolutionsDatabase.global_max_fitness), [`has_island_with_size`](evo.md#SolutionsDatabase.has_island_with_size), [`has_nodes`](evo.md#SolutionsDatabase.has_nodes)

### `SolutionsDatabase`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py:237`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L237)
- doc: Maintains and updates a Database of all solutions (Nodes).
- signature: `class SolutionsDatabase:`
- members:
  - `_update_global_fitness_range(self, score: float)` — [`L298`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L298) — Updates the global min and max fitness scores seen so far.
  - `add_nodes_to_islands(self, solution_nodes: List[Node], island_ids: List[int], migration_prob: float)` — [`L339`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L339) — Add evaluated Nodes to appropriate islands based on fitness improvement.
  - `get_normalized_score(self, score: Optional[float])` — [`L308`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L308) — Normalizes a raw fitness score to the range [0, 1], where 1.0 is always best.
  - `has_island_with_size(self, size: int)` — [`L272`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L272)
  - `has_nodes(self)` — [`L269`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L269)
  - `request_fresh_draft(self, reason: str)` — [`L499`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L499) — Make the next non-initial generation explore a clean candidate.
  - `reset_islands(self)` — [`L397`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L397) — Resets the weaker half of islands and seeds them
  - `sample_in_context(self, num_samples: Dict, temperature: float, crossover_prob: float, fresh_draft_prob: float = 0)` — [`L503`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L503) — Samples nodes for the next generation, selecting islands and then nodes based on fitness.
  - `sample_in_context_with_trace(self, num_samples: Dict, temperature: float, crossover_prob: float, fresh_draft_prob: float = 0)` — [`L733`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L733)
  - `seed_islands_with_nodes(self, solution_nodes: List[Node], island_ids: List[int])` — [`L275`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L275) — Initialize islands with the first generation of Nodes.
  - `experience_config` — [`L257`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L257)
  - `global_max_fitness` — [`L261`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L261)
  - `global_min_fitness` — [`L260`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L260)
  - `last_parent_selection` — [`L258`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L258)
  - `logger` — [`L256`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L256)
  - `lower_is_better` — [`L255`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L255)
  - `max_size` — [`L254`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L254)
  - `num_islands` — [`L253`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L253)
- protocol/private: `__init__`[`L245`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L245), `_forced_fresh_draft_reason`[`L501`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L501), `_islands`[`L259`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L259)
- uses (calls/refs, reference-scoped): [`Node`](../../core/solvers/utils/journal.md#Node), [`LogEvent`](../../utils/logger.md#LogEvent), [`metric`](../../core/solvers/utils/journal.md#Node.metric), [`id`](../../core/solvers/utils/journal.md#Node.id), [`value`](../../core/solvers/utils/metric.md#MetricValue.value), [`SOLVER`](../../utils/logger.md#LogEvent.SOLVER), [`compute_parent_utilities`](experience.md#compute_parent_utilities), [`register_node_in_island`](evo.md#Island.register_node_in_island), [`info`](../../utils/logger.md#CollectiveLogger.info), [`remove_lowest`](evo.md#Island.remove_lowest), [`nodes`](evo.md#Island.nodes), [`size`](evo.md#Island.size), [`fitness_scores`](evo.md#Island.fitness_scores), [`warning`](../../utils/logger.md#CollectiveLogger.warning), [`CollectiveLogger`](../../utils/logger.md#CollectiveLogger), [`average_fitness_score`](evo.md#Island.average_fitness_score), [`debug`](../../utils/logger.md#CollectiveLogger.debug), [`error`](../../utils/logger.md#CollectiveLogger.error), [`best_fitness_score`](evo.md#Island.best_fitness_score), [`normalized`](../../core/solvers/utils/search_utils.md#normalized), [`Island`](evo.md#Island)
- used by: [`search`](evo.md#Evolutionary.search), [`_debug_cycle_async`](evo.md#Evolutionary._debug_cycle_async), [`_async_worker_loop`](evo.md#Evolutionary._async_worker_loop), [`_next_async_work_item`](evo.md#Evolutionary._next_async_work_item), [`_commit_async_node`](evo.md#Evolutionary._commit_async_node), [`_seed_solution_database_from_journal`](evo.md#Evolutionary._seed_solution_database_from_journal), [`_new_solution_database`](evo.md#Evolutionary._new_solution_database), [`_restore_solution_database_from_journal`](evo.md#Evolutionary._restore_solution_database_from_journal)

