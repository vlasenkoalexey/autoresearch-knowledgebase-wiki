---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.solvers.evo.evo`/
symbols:
  Evolutionary.search: Evolutionary#search().
  Evolutionary.parse_eval_result: Evolutionary#parse_eval_result().
  Evolutionary._draft: Evolutionary#_draft().
  Evolutionary._improve: Evolutionary#_improve().
  SolutionsDatabase.add_nodes_to_islands: SolutionsDatabase#add_nodes_to_islands().
  Evolutionary._debug: Evolutionary#_debug().
  Evolutionary._crossover: Evolutionary#_crossover().
  SolutionsDatabase.sample_in_context: SolutionsDatabase#sample_in_context().
  Evolutionary.create_root_node: Evolutionary#create_root_node().
  Evolutionary.debug_cycle: Evolutionary#debug_cycle().
  Evolutionary._build_solution_database_from_journal: Evolutionary#_build_solution_database_from_journal().
  Evolutionary.__call__: Evolutionary#__call__().
  Island.register_node_in_island: Island#register_node_in_island().
  SolutionsDatabase._islands: SolutionsDatabase#_islands.
  SolutionsDatabase.reset_islands: SolutionsDatabase#reset_islands().
  Evolutionary.state: Evolutionary#state.
  Island.only_keep_best: Island#only_keep_best().
  SolutionsDatabase.logger: SolutionsDatabase#logger.
  Island.remove_lowest: Island#remove_lowest().
  Island.remove_node: Island#remove_node().
  Evolutionary.load_checkpoint: Evolutionary#load_checkpoint().
  SolutionsDatabase.seed_islands_with_nodes: SolutionsDatabase#seed_islands_with_nodes().
  SolutionsDatabase.global_max_fitness: SolutionsDatabase#global_max_fitness.
  Evolutionary.journal: Evolutionary#journal.
  Evolutionary.log_journal: Evolutionary#log_journal().
  Island.migrate_node: Island#migrate_node().
  SolutionsDatabase.state_dict: SolutionsDatabase#state_dict().
  Island.nodes: Island#nodes.
  SolutionsDatabase._update_global_fitness_range: SolutionsDatabase#_update_global_fitness_range().
  Evolutionary.save_checkpoint: Evolutionary#save_checkpoint().
  Evolutionary._analyze: Evolutionary#_analyze().
  Island.fitness_scores: Island#fitness_scores().
  Island.size: Island#size().
  Island.fittest_individual: Island#fittest_individual().
  Evolutionary.draft_fn: Evolutionary#draft_fn.
  Evolutionary.improve_fn: Evolutionary#improve_fn.
  Evolutionary.debug_fn: Evolutionary#debug_fn.
  Evolutionary.crossover_fn: Evolutionary#crossover_fn.
  Evolutionary.update_data_preview: Evolutionary#update_data_preview().
  SolutionsDatabase.get_normalized_score: SolutionsDatabase#get_normalized_score().
  Evolutionary.memory_op: Evolutionary#memory_op.
  SolutionsDatabase.global_min_fitness: SolutionsDatabase#global_min_fitness.
  Evolutionary.lower_is_better: Evolutionary#lower_is_better.
  Evolutionary.task_desc: Evolutionary#task_desc.
  Evolutionary.setup_operators: Evolutionary#setup_operators().
  Evolutionary.debug_memory_op: Evolutionary#debug_memory_op.
  Island.average_fitness_score: Island#average_fitness_score().
  SolutionsDatabase.lower_is_better: SolutionsDatabase#lower_is_better.
  Evolutionary.data_preview: Evolutionary#data_preview.
  Island.island_id: Island#island_id.
  Island.lower_is_better: Island#lower_is_better.
  Island.logger: Island#logger.
  Evolutionary.prompt_context: Evolutionary#prompt_context.
  Island.best_fitness_score: Island#best_fitness_score().
  Evolutionary.analyze_fn: Evolutionary#analyze_fn.
  Evolutionary.root_node: Evolutionary#root_node.
  Evolutionary: Evolutionary#
  Island.__init__: Island#__init__().
  Island.solution_nodes: Island#solution_nodes().
  Evolutionary.__init__: Evolutionary#__init__().
  SolutionsDatabase.num_islands: SolutionsDatabase#num_islands.
  SolutionsDatabase.max_size: SolutionsDatabase#max_size.
  Evolutionary.linear_decay: Evolutionary#linear_decay().
  SolutionsDatabase.__init__: SolutionsDatabase#__init__().
  Island: Island#
  SolutionsDatabase: SolutionsDatabase#
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py)

## Classes
### `Evolutionary`  ·  implements/extends Solver
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py:584`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L584)
- signature: `class Evolutionary(Solver):`
- members:
  - `_analyze(self, node: Node)` — [`L747`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L747) — Analyze a node's execution results using the analyze LLM operator.
  - `_debug(self, parent_node: Node)` — [`L719`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L719) — Debug a buggy solution using the debug LLM operator.
  - `_draft(self)` — [`L660`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L660) — Generate a new solution from scratch using the draft LLM operator.
  - `_improve(self, parent_node: Node)` — [`L688`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L688) — Improve an existing solution using the improve LLM operator.
  - `create_root_node(self)` — [`L972`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L972)
  - `debug_cycle(self, state, task, buggy_node: Node)` — [`L827`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L827)
  - `linear_decay(self, iteration: int)` — [`L820`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L820) — defines a temperature schedule for sampling of islands and individuals
  - `load_checkpoint(self)` — [`L615`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L615)
  - `log_journal(self)` — [`L1135`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1135)
  - `parse_eval_result(self, node: Node, eval_result: Dict[str, Any])` — [`L874`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L874) — Parse evaluation results and update the node accordingly.
  - `save_checkpoint(self)` — [`L604`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L604)
  - `search(self, task, state)` — [`L1016`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1016)
  - `setup_operators(self)` — [`L631`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L631) — Setup operator LLMs.
  - `update_data_preview(self, state)` — [`L789`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L789) — Generate a data preview to provide context for the LLM operators.
  - `analyze_fn` — [`L655`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L655)
  - `crossover_fn` — [`L656`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L656)
  - `data_preview` — [`L588`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L588)
  - `debug_fn` — [`L652`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L652)
  - `debug_memory_op` — [`L643`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L643)
  - `draft_fn` — [`L646`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L646)
  - `improve_fn` — [`L649`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L649)
  - `journal` — [`L587`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L587)
  - `lower_is_better` — [`L597`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L597)
  - `memory_op` — [`L642`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L642)
  - `prompt_context` — [`L591`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L591)
  - `root_node` — [`L973`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L973)
  - `state` — [`L602`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L602)
  - `task_desc` — [`L590`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L590)
- protocol/private: `__call__`[`L1146`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L1146), `__init__`[`L585`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L585), `_build_solution_database_from_journal`[`L985`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L985), `_crossover`[`L766`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L766)
- uses (calls/refs, reference-scoped): [`logger`](../../core/solvers/base.md#Solver.logger), [`cfg`](../../core/solvers/base.md#Solver.cfg), [`Node`](../../core/solvers/utils/journal.md#Node), [`LogEvent`](../../utils/logger.md#LogEvent), [`metric`](../../core/solvers/utils/journal.md#Node.metric), [`from_export_data`](../../core/solvers/utils/journal.md#Journal.from_export_data), [`get_node_data`](../../core/solvers/utils/journal.md#Journal.get_node_data), [`id`](../../core/solvers/utils/journal.md#Node.id), [`value`](../../core/solvers/utils/metric.md#MetricValue.value), [`parents`](../../core/solvers/utils/journal.md#Node.parents), [`code`](../../core/solvers/utils/journal.md#Node.code), [`Journal`](../../core/solvers/utils/journal.md#Journal), [`add_nodes_to_islands`](evo.md#SolutionsDatabase.add_nodes_to_islands), [`sample_in_context`](evo.md#SolutionsDatabase.sample_in_context), [`SOLVER`](../../utils/logger.md#LogEvent.SOLVER), [`nodes`](../../core/solvers/utils/journal.md#Journal.nodes), [`is_buggy`](../../core/solvers/utils/journal.md#Node.is_buggy), [`export_search_results`](../../core/solvers/utils/search_exporter.md#export_search_results), [`plan`](../../core/solvers/utils/journal.md#Node.plan), [`GenericLLM`](../../core/solvers/llm_helpers/generic_llm.md#GenericLLM), [`create_memory_op`](../../core/solvers/operators/memory.md#create_memory_op), [`absorb_exec_result`](../../core/solvers/utils/journal.md#Node.absorb_exec_result), [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`append`](../../core/solvers/utils/journal.md#Journal.append), [`step`](../../core/solvers/utils/journal.md#Node.step), [`generate`](../../core/solvers/utils/data_preview.md#generate), [`get_complextiy_level`](../utils.md#get_complextiy_level), [`is_root_node`](../../core/solvers/utils/journal.md#Journal.is_root_node), [`analyze_op`](../../core/solvers/operators/analyze.md#analyze_op), [`get_best_node`](../../core/solvers/utils/journal.md#Journal.get_best_node), [`improve_op`](../../core/solvers/operators/improve.md#improve_op), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`MetricValue`](../../core/solvers/utils/metric.md#MetricValue), [`info`](../../core/solvers/utils/metric.md#MetricValue.info), [`seed_islands_with_nodes`](evo.md#SolutionsDatabase.seed_islands_with_nodes), [`analysis`](../../core/solvers/utils/journal.md#Node.analysis), [`debug_op`](../../core/solvers/operators/debug.md#debug_op), [`execute_op_plan_code`](../../core/solvers/operators/core.md#execute_op_plan_code), [`maximize`](../../core/solvers/utils/metric.md#MetricValue.maximize), [`parse_json_output`](../../utils/code_parsing.md#parse_json_output)  (+34 more)
- used by: [`load_checkpoint`](../../core/solvers/base.md#Solver.load_checkpoint), [`save_checkpoint`](../../core/solvers/base.md#Solver.save_checkpoint), [`Solver`](../../core/solvers/base.md#Solver), [`_materialize`](../../config_dataclasses/solver/__init__.md#_LazySolverMap._materialize)

### `Island`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py:58`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L58)
- doc: A population of solutions (Nodes) in an island.
- signature: `class Island:`
- members:
  - `average_fitness_score(self)` — [`L101`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L101) — Returns the average fitness score.
  - `best_fitness_score(self)` — [`L91`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L91) — Returns the best fitness score in the island.
  - `fitness_scores(self)` — [`L78`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L78) — Returns fitness scores, using +/- inf for None metrics.
  - `fittest_individual(self)` — [`L118`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L118) — Returns the node with the best fitness score.
  - `migrate_node(self, founder_node: Node)` — [`L191`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L191) — Migrate a node from a founder island to this island.
  - `only_keep_best(self)` — [`L175`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L175) — Remove all nodes except the single best one.
  - `register_node_in_island(self, solution_node: Node)` — [`L131`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L131) — Add a solution Node to the island population.
  - `remove_lowest(self)` — [`L145`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L145) — Removes the node with the worst fitness score in the island.
  - `remove_node(self, to_remove_node: Node)` — [`L161`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L161) — Remove a specific node from the island.
  - `size(self)` — [`L74`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L74)
  - `solution_nodes(self)` — [`L128`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L128)
  - `island_id` — [`L68`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L68)
  - `logger` — [`L70`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L70)
  - `lower_is_better` — [`L69`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L69)
  - `nodes` — [`L71`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L71)
- protocol/private: `__init__`[`L61`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L61)
- uses (calls/refs, reference-scoped): [`Node`](../../core/solvers/utils/journal.md#Node), [`LogEvent`](../../utils/logger.md#LogEvent), [`metric`](../../core/solvers/utils/journal.md#Node.metric), [`id`](../../core/solvers/utils/journal.md#Node.id), [`value`](../../core/solvers/utils/metric.md#MetricValue.value), [`SOLVER`](../../utils/logger.md#LogEvent.SOLVER), [`info`](../../utils/logger.md#CollectiveLogger.info), [`warning`](../../utils/logger.md#CollectiveLogger.warning), [`CollectiveLogger`](../../utils/logger.md#CollectiveLogger)
- used by: [`add_nodes_to_islands`](evo.md#SolutionsDatabase.add_nodes_to_islands), [`sample_in_context`](evo.md#SolutionsDatabase.sample_in_context), [`_islands`](evo.md#SolutionsDatabase._islands), [`reset_islands`](evo.md#SolutionsDatabase.reset_islands), [`seed_islands_with_nodes`](evo.md#SolutionsDatabase.seed_islands_with_nodes), [`global_max_fitness`](evo.md#SolutionsDatabase.global_max_fitness), [`state_dict`](evo.md#SolutionsDatabase.state_dict)

### `SolutionsDatabase`
- def: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py:202`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L202)
- doc: Maintains and updates a Database of all solutions (Nodes).
- signature: `class SolutionsDatabase:`
- members:
  - `_update_global_fitness_range(self, score: float)` — [`L266`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L266) — Updates the global min and max fitness scores seen so far.
  - `add_nodes_to_islands(self, solution_nodes: List[Node], island_ids: List[int], migration_prob: float)` — [`L307`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L307) — Add evaluated Nodes to appropriate islands based on fitness improvement.
  - `get_normalized_score(self, score: Optional[float])` — [`L276`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L276) — Normalizes a raw fitness score to the range [0, 1], where 1.0 is always best.
  - `reset_islands(self)` — [`L365`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L365) — Resets the weaker half of islands and seeds them
  - `sample_in_context(self, num_samples: Dict, temperature: float, crossover_prob: float)` — [`L467`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L467) — Samples nodes for the next generation, selecting islands and then nodes based on fitness.
  - `seed_islands_with_nodes(self, solution_nodes: List[Node], island_ids: List[int])` — [`L243`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L243) — Initialize islands with the first generation of Nodes.
  - `state_dict(self)` — [`L230`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L230)
  - `global_max_fitness` — [`L223`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L223)
  - `global_min_fitness` — [`L222`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L222)
  - `logger` — [`L220`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L220)
  - `lower_is_better` — [`L219`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L219)
  - `max_size` — [`L218`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L218)
  - `num_islands` — [`L217`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L217)
- protocol/private: `__init__`[`L210`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L210), `_islands`[`L221`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/solvers/evo/evo.py#L221)
- uses (calls/refs, reference-scoped): [`Node`](../../core/solvers/utils/journal.md#Node), [`LogEvent`](../../utils/logger.md#LogEvent), [`metric`](../../core/solvers/utils/journal.md#Node.metric), [`id`](../../core/solvers/utils/journal.md#Node.id), [`value`](../../core/solvers/utils/metric.md#MetricValue.value), [`SOLVER`](../../utils/logger.md#LogEvent.SOLVER), [`register_node_in_island`](evo.md#Island.register_node_in_island), [`remove_lowest`](evo.md#Island.remove_lowest), [`info`](../../utils/logger.md#CollectiveLogger.info), [`nodes`](evo.md#Island.nodes), [`fitness_scores`](evo.md#Island.fitness_scores), [`size`](evo.md#Island.size), [`warning`](../../utils/logger.md#CollectiveLogger.warning), [`CollectiveLogger`](../../utils/logger.md#CollectiveLogger), [`average_fitness_score`](evo.md#Island.average_fitness_score), [`error`](../../utils/logger.md#CollectiveLogger.error), [`debug`](../../utils/logger.md#CollectiveLogger.debug), [`best_fitness_score`](evo.md#Island.best_fitness_score), [`normalized`](../../core/solvers/utils/search_utils.md#normalized), [`Island`](evo.md#Island)
- used by: [`search`](evo.md#Evolutionary.search), [`_build_solution_database_from_journal`](evo.md#Evolutionary._build_solution_database_from_journal)

