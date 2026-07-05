---
title: 'Module: openevolve/database.py'
type: catalog
provenance: extracted
module: openevolve/database.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.database`/
symbols:
  Program.id: Program#id.
  ProgramDatabase.add: ProgramDatabase#add().
  Program.metrics: Program#metrics.
  Program: Program#
  ProgramDatabase.programs: ProgramDatabase#programs.
  Program.code: Program#code.
  logger: logger.
  ProgramDatabase: ProgramDatabase#
  ProgramDatabase.islands: ProgramDatabase#islands.
  Program.metadata: Program#metadata.
  Program.language: Program#language.
  ProgramDatabase.config: ProgramDatabase#config.
  ProgramDatabase.migrate_programs: ProgramDatabase#migrate_programs().
  ProgramDatabase.load: ProgramDatabase#load().
  ProgramDatabase.save: ProgramDatabase#save().
  ProgramDatabase._sample_exploration_parent: ProgramDatabase#_sample_exploration_parent().
  ProgramDatabase.feature_stats: ProgramDatabase#feature_stats.
  ProgramDatabase.sample_from_island: ProgramDatabase#sample_from_island().
  ProgramDatabase._calculate_feature_coords: ProgramDatabase#_calculate_feature_coords().
  ProgramDatabase.island_feature_maps: ProgramDatabase#island_feature_maps.
  ProgramDatabase.best_program_id: ProgramDatabase#best_program_id.
  ProgramDatabase.island_best_programs: ProgramDatabase#island_best_programs.
  ProgramDatabase.current_island: ProgramDatabase#current_island.
  ProgramDatabase._sample_inspirations: ProgramDatabase#_sample_inspirations().
  ProgramDatabase.island_generations: ProgramDatabase#island_generations.
  Program.generation: Program#generation.
  ProgramDatabase._enforce_population_limit: ProgramDatabase#_enforce_population_limit().
  Program.parent_id: Program#parent_id.
  ProgramDatabase.store_artifacts: ProgramDatabase#store_artifacts().
  ProgramDatabase.archive: ProgramDatabase#archive.
  ProgramDatabase.get_best_program: ProgramDatabase#get_best_program().
  ProgramDatabase.feature_bins: ProgramDatabase#feature_bins.
  ProgramDatabase._reconstruct_islands: ProgramDatabase#_reconstruct_islands().
  ProgramDatabase._is_novel: ProgramDatabase#_is_novel().
  ProgramDatabase._sample_from_island_weighted: ProgramDatabase#_sample_from_island_weighted().
  ProgramDatabase.get_top_programs: ProgramDatabase#get_top_programs().
  ProgramDatabase.get: ProgramDatabase#get().
  ProgramDatabase._update_archive: ProgramDatabase#_update_archive().
  ProgramDatabase.feature_bins_per_dim: ProgramDatabase#feature_bins_per_dim.
  ProgramDatabase._get_cached_diversity: ProgramDatabase#_get_cached_diversity().
  ProgramDatabase.get_island_stats: ProgramDatabase#get_island_stats().
  ProgramDatabase.get_artifacts: ProgramDatabase#get_artifacts().
  ProgramDatabase._llm_judge_novelty: ProgramDatabase#_llm_judge_novelty().
  ProgramDatabase.sample: ProgramDatabase#sample().
  ProgramDatabase.last_iteration: ProgramDatabase#last_iteration.
  Program.iteration_found: Program#iteration_found.
  ProgramDatabase._cleanup_stale_island_bests: ProgramDatabase#_cleanup_stale_island_bests().
  ProgramDatabase._scale_feature_value: ProgramDatabase#_scale_feature_value().
  ProgramDatabase._is_better: ProgramDatabase#_is_better().
  ProgramDatabase._update_best_program: ProgramDatabase#_update_best_program().
  ProgramDatabase._update_island_best_program: ProgramDatabase#_update_island_best_program().
  ProgramDatabase._sample_parent: ProgramDatabase#_sample_parent().
  ProgramDatabase._sample_exploitation_parent: ProgramDatabase#_sample_exploitation_parent().
  ProgramDatabase._sample_from_archive_for_island: ProgramDatabase#_sample_from_archive_for_island().
  ProgramDatabase._update_diversity_reference_set: ProgramDatabase#_update_diversity_reference_set().
  ProgramDatabase._validate_migration_results: ProgramDatabase#_validate_migration_results().
  ProgramDatabase._calculate_complexity_bin: ProgramDatabase#_calculate_complexity_bin().
  ProgramDatabase.diversity_cache: ProgramDatabase#diversity_cache.
  ProgramDatabase._calculate_diversity_bin: ProgramDatabase#_calculate_diversity_bin().
  ProgramDatabase._save_program: ProgramDatabase#_save_program().
  ProgramDatabase._sample_from_island_random: ProgramDatabase#_sample_from_island_random().
  ProgramDatabase.prompts_by_program: ProgramDatabase#prompts_by_program.
  ProgramDatabase.log_island_status: ProgramDatabase#log_island_status().
  ProgramDatabase.last_migration_generation: ProgramDatabase#last_migration_generation.
  ProgramDatabase.should_migrate: ProgramDatabase#should_migrate().
  ProgramDatabase._update_feature_stats: ProgramDatabase#_update_feature_stats().
  Program.changes_description: Program#changes_description.
  ProgramDatabase._distribute_programs_to_islands: ProgramDatabase#_distribute_programs_to_islands().
  ProgramDatabase._calculate_island_diversity: ProgramDatabase#_calculate_island_diversity().
  ProgramDatabase._cleanup_old_artifacts: ProgramDatabase#_cleanup_old_artifacts().
  ProgramDatabase.diversity_reference_set: ProgramDatabase#diversity_reference_set.
  ProgramDatabase._sample_random_parent: ProgramDatabase#_sample_random_parent().
  ProgramDatabase.set_current_island: ProgramDatabase#set_current_island().
  ProgramDatabase.next_island: ProgramDatabase#next_island().
  ProgramDatabase.log_prompt: ProgramDatabase#log_prompt().
  Program.artifact_dir: Program#artifact_dir.
  Program.to_dict: Program#to_dict().
  ProgramDatabase.increment_island_generation: ProgramDatabase#increment_island_generation().
  Program.artifacts_json: Program#artifacts_json.
  ProgramDatabase._invalidate_diversity_cache: ProgramDatabase#_invalidate_diversity_cache().
  ProgramDatabase.embedding_client: ProgramDatabase#embedding_client.
  ProgramDatabase._fast_code_diversity: ProgramDatabase#_fast_code_diversity().
  ProgramDatabase._deserialize_feature_stats: ProgramDatabase#_deserialize_feature_stats().
  Program.timestamp: Program#timestamp.
  Program.from_dict: Program#from_dict().
  ProgramDatabase._cache_diversity_value: ProgramDatabase#_cache_diversity_value().
  ProgramDatabase._create_artifact_dir: ProgramDatabase#_create_artifact_dir().
  ProgramDatabase._serialize_feature_stats: ProgramDatabase#_serialize_feature_stats().
  ProgramDatabase.feature_scaling_method: ProgramDatabase#feature_scaling_method.
  ProgramDatabase.novelty_llm: ProgramDatabase#novelty_llm.
  ProgramDatabase.similarity_threshold: ProgramDatabase#similarity_threshold.
  Program.complexity: Program#complexity.
  Program.diversity: Program#diversity.
  ProgramDatabase.diversity_reference_size: ProgramDatabase#diversity_reference_size.
  ProgramDatabase._feature_coords_to_key: ProgramDatabase#_feature_coords_to_key().
  ProgramDatabase._scale_feature_value_minmax: ProgramDatabase#_scale_feature_value_minmax().
  ProgramDatabase._write_artifact_file: ProgramDatabase#_write_artifact_file().
  ProgramDatabase._load_artifact_dir: ProgramDatabase#_load_artifact_dir().
  Program.embedding: Program#embedding.
  ProgramDatabase.__init__: ProgramDatabase#__init__().
  ProgramDatabase.diversity_cache_size: ProgramDatabase#diversity_cache_size.
  Program.prompts: Program#prompts.
  ProgramDatabase.migration_interval: ProgramDatabase#migration_interval.
  ProgramDatabase.migration_rate: ProgramDatabase#migration_rate.
  ProgramDatabase._cosine_similarity: ProgramDatabase#_cosine_similarity().
  ProgramDatabase._get_artifact_size: ProgramDatabase#_get_artifact_size().
  ProgramDatabase._artifact_serializer: ProgramDatabase#_artifact_serializer().
  _safe_sum_metrics: _safe_sum_metrics().
  _safe_avg_metrics: _safe_avg_metrics().
  ProgramDatabase._artifact_deserializer: ProgramDatabase#_artifact_deserializer().
---
# Module: [`openevolve/database.py`](../../../../../raw/code/openevolve/openevolve/database.py)

## Classes
### `Program`
- def: [`openevolve/database.py:44`](../../../../../raw/code/openevolve/openevolve/database.py#L44) — documented in [openevolve-api](../../concepts/openevolve-api.md)
- doc: Represents a program in the database
- signature: `class Program:`
- members:
  - `from_dict(cls, data: Dict[str, Any])` — [`L84`](../../../../../raw/code/openevolve/openevolve/database.py#L84) — Create from dictionary representation
  - `to_dict(self)` — [`L79`](../../../../../raw/code/openevolve/openevolve/database.py#L79) — Convert to dictionary representation
  - `artifact_dir` — [`L74`](../../../../../raw/code/openevolve/openevolve/database.py#L74)
  - `artifacts_json` — [`L73`](../../../../../raw/code/openevolve/openevolve/database.py#L73)
  - `changes_description` — [`L50`](../../../../../raw/code/openevolve/openevolve/database.py#L50)
  - `code` — [`L49`](../../../../../raw/code/openevolve/openevolve/database.py#L49) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `complexity` — [`L63`](../../../../../raw/code/openevolve/openevolve/database.py#L63)
  - `diversity` — [`L64`](../../../../../raw/code/openevolve/openevolve/database.py#L64)
  - `embedding` — [`L77`](../../../../../raw/code/openevolve/openevolve/database.py#L77)
  - `generation` — [`L55`](../../../../../raw/code/openevolve/openevolve/database.py#L55) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `id` — [`L48`](../../../../../raw/code/openevolve/openevolve/database.py#L48) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `iteration_found` — [`L57`](../../../../../raw/code/openevolve/openevolve/database.py#L57)
  - `language` — [`L51`](../../../../../raw/code/openevolve/openevolve/database.py#L51) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `metadata` — [`L67`](../../../../../raw/code/openevolve/openevolve/database.py#L67) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `metrics` — [`L60`](../../../../../raw/code/openevolve/openevolve/database.py#L60) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `parent_id` — [`L54`](../../../../../raw/code/openevolve/openevolve/database.py#L54) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `prompts` — [`L70`](../../../../../raw/code/openevolve/openevolve/database.py#L70)
  - `timestamp` — [`L56`](../../../../../raw/code/openevolve/openevolve/database.py#L56)
- uses (calls/refs, reference-scoped): [`logger`](database.md#logger)
- used by: [`add`](database.md#ProgramDatabase.add), [`programs`](database.md#ProgramDatabase.programs), [`run_iteration_with_shared_db`](iteration.md#run_iteration_with_shared_db), [`run`](controller.md#OpenEvolve.run), [`_run_iteration_worker`](process_parallel.md#_run_iteration_worker), [`run_evolution`](process_parallel.md#ProcessParallelController.run_evolution), [`migrate_programs`](database.md#ProgramDatabase.migrate_programs), [`load`](database.md#ProgramDatabase.load), [`save`](database.md#ProgramDatabase.save), [`_sample_exploration_parent`](database.md#ProgramDatabase._sample_exploration_parent), [`sample_from_island`](database.md#ProgramDatabase.sample_from_island), [`_warned_about_combined_score`](process_parallel.md#ProcessParallelController._warned_about_combined_score), [`_calculate_feature_coords`](database.md#ProgramDatabase._calculate_feature_coords), [`_save_checkpoint`](controller.md#OpenEvolve._save_checkpoint), [`_run_evolution_async`](api.md#_run_evolution_async), [`main_async`](cli.md#main_async), [`_save_best_program`](controller.md#OpenEvolve._save_best_program), [`_submit_iteration`](process_parallel.md#ProcessParallelController._submit_iteration), [`_sample_inspirations`](database.md#ProgramDatabase._sample_inspirations), [`_enforce_population_limit`](database.md#ProgramDatabase._enforce_population_limit), [`store_artifacts`](database.md#ProgramDatabase.store_artifacts), [`get_best_program`](database.md#ProgramDatabase.get_best_program), [`_is_novel`](database.md#ProgramDatabase._is_novel), [`_reconstruct_islands`](database.md#ProgramDatabase._reconstruct_islands), [`_sample_from_island_weighted`](database.md#ProgramDatabase._sample_from_island_weighted), [`get_top_programs`](database.md#ProgramDatabase.get_top_programs), [`_update_archive`](database.md#ProgramDatabase._update_archive), [`get`](database.md#ProgramDatabase.get), [`_create_database_snapshot`](process_parallel.md#ProcessParallelController._create_database_snapshot), [`_get_cached_diversity`](database.md#ProgramDatabase._get_cached_diversity), [`get_artifacts`](database.md#ProgramDatabase.get_artifacts), [`get_island_stats`](database.md#ProgramDatabase.get_island_stats), [`_llm_judge_novelty`](database.md#ProgramDatabase._llm_judge_novelty), [`sample`](database.md#ProgramDatabase.sample), [`_cleanup_stale_island_bests`](database.md#ProgramDatabase._cleanup_stale_island_bests), [`_is_better`](database.md#ProgramDatabase._is_better), [`_sample_exploitation_parent`](database.md#ProgramDatabase._sample_exploitation_parent), [`_sample_from_archive_for_island`](database.md#ProgramDatabase._sample_from_archive_for_island), [`_sample_parent`](database.md#ProgramDatabase._sample_parent), [`_update_best_program`](database.md#ProgramDatabase._update_best_program)  (+10 more; 112 test-only)

### `ProgramDatabase`
- def: [`openevolve/database.py:113`](../../../../../raw/code/openevolve/openevolve/database.py#L113) — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
- doc: Database for storing and sampling programs during evolution
- signature: `class ProgramDatabase:`
- members:
  - `_artifact_deserializer(self, dct)` — [`L2425`](../../../../../raw/code/openevolve/openevolve/database.py#L2425) — JSON deserializer for artifacts that handles bytes
  - `_artifact_serializer(self, obj)` — [`L2419`](../../../../../raw/code/openevolve/openevolve/database.py#L2419) — JSON serializer for artifacts that handles bytes
  - `_cache_diversity_value(self, code_hash: int, diversity: float)` — [`L2152`](../../../../../raw/code/openevolve/openevolve/database.py#L2152) — Cache a diversity value with LRU eviction
  - `_calculate_complexity_bin(self, complexity: int)` — [`L902`](../../../../../raw/code/openevolve/openevolve/database.py#L902) — Calculate the bin index for a given complexity value using feature scaling.
  - `_calculate_diversity_bin(self, diversity: float)` — [`L929`](../../../../../raw/code/openevolve/openevolve/database.py#L929) — Calculate the bin index for a given diversity value using feature scaling.
  - `_calculate_feature_coords(self, program: Program)` — [`L834`](../../../../../raw/code/openevolve/openevolve/database.py#L834) — Calculate feature coordinates for the MAP-Elites grid — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `_calculate_island_diversity(self, programs: List[Program])` — [`L2007`](../../../../../raw/code/openevolve/openevolve/database.py#L2007) — Calculate diversity within an island (deterministic version)
  - `_cleanup_old_artifacts(self, checkpoint_path: str)` — [`L2445`](../../../../../raw/code/openevolve/openevolve/database.py#L2445) — Remove artifact directories older than the configured retention period.
  - `_cleanup_stale_island_bests(self)` — [`L1923`](../../../../../raw/code/openevolve/openevolve/database.py#L1923) — Remove stale island best program references
  - `_cosine_similarity(self, vec1: List[float], vec2: List[float])` — [`L968`](../../../../../raw/code/openevolve/openevolve/database.py#L968) — Adapted from SakanaAI/ShinkaEvolve (Apache-2.0 License)
  - `_create_artifact_dir(self, program_id: str)` — [`L2431`](../../../../../raw/code/openevolve/openevolve/database.py#L2431) — Create artifact directory for a program
  - `_deserialize_feature_stats(self, stats_dict: Dict[str, Any])` — [`L2279`](../../../../../raw/code/openevolve/openevolve/database.py#L2279) — Deserialize feature_stats from loaded JSON
  - `_distribute_programs_to_islands(self)` — [`L789`](../../../../../raw/code/openevolve/openevolve/database.py#L789) — Distribute loaded programs across islands when no island metadata exists
  - `_enforce_population_limit(self, exclude_program_id: Optional[str] = None)` — [`L1678`](../../../../../raw/code/openevolve/openevolve/database.py#L1678) — Enforce the population size limit by removing worst programs if needed — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `_fast_code_diversity(self, code1: str, code2: str)` — [`L2042`](../../../../../raw/code/openevolve/openevolve/database.py#L2042) — Fast approximation of code diversity using simple metrics
  - `_feature_coords_to_key(self, coords: List[int])` — [`L956`](../../../../../raw/code/openevolve/openevolve/database.py#L956) — Convert feature coordinates to a string key
  - `_get_artifact_size(self, value: Union[str, bytes])` — [`L2410`](../../../../../raw/code/openevolve/openevolve/database.py#L2410) — Get size of an artifact value in bytes
  - `_get_cached_diversity(self, program: Program)` — [`L2070`](../../../../../raw/code/openevolve/openevolve/database.py#L2070) — Get diversity score for a program using cache and reference set
  - `_invalidate_diversity_cache(self)` — [`L2163`](../../../../../raw/code/openevolve/openevolve/database.py#L2163) — Invalidate the diversity cache when programs change significantly
  - `_is_better(self, program1: Program, program2: Program)` — [`L1101`](../../../../../raw/code/openevolve/openevolve/database.py#L1101) — Determine if program1 has better FITNESS than program2
  - `_is_novel(self, program_id: int, island_idx: int)` — [`L1058`](../../../../../raw/code/openevolve/openevolve/database.py#L1058) — Determine if a program is novel based on diversity to existing programs
  - `_llm_judge_novelty(self, program: Program, similar_program: Program)` — [`L991`](../../../../../raw/code/openevolve/openevolve/database.py#L991) — Use LLM to judge if a program is novel compared to a similar existing program
  - `_load_artifact_dir(self, artifact_dir: str)` — [`L2508`](../../../../../raw/code/openevolve/openevolve/database.py#L2508) — Load artifacts from a directory
  - `_reconstruct_islands(self, saved_islands: List[List[str]])` — [`L709`](../../../../../raw/code/openevolve/openevolve/database.py#L709) — Reconstruct island assignments from saved metadata
  - `_sample_exploitation_parent(self)` — [`L1376`](../../../../../raw/code/openevolve/openevolve/database.py#L1376) — Sample a parent for exploitation (from archive/elite programs)
  - `_sample_exploration_parent(self)` — [`L1290`](../../../../../raw/code/openevolve/openevolve/database.py#L1290) — Sample a parent for exploration (from current island) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `_sample_from_archive_for_island(self, island_id: int)` — [`L1515`](../../../../../raw/code/openevolve/openevolve/database.py#L1515) — Sample a parent from the archive, preferring programs from the specified island
  - `_sample_from_island_random(self, island_id: int)` — [`L1484`](../../../../../raw/code/openevolve/openevolve/database.py#L1484) — Sample a completely random parent from a specific island (uniform distribution)
  - `_sample_from_island_weighted(self, island_id: int)` — [`L1427`](../../../../../raw/code/openevolve/openevolve/database.py#L1427) — Sample a parent from a specific island using fitness-weighted selection
  - `_sample_inspirations(self, parent: Program, n: int = 5)` — [`L1554`](../../../../../raw/code/openevolve/openevolve/database.py#L1554) — Sample inspiration programs for the next evolution step.
  - `_sample_parent(self)` — [`L1270`](../../../../../raw/code/openevolve/openevolve/database.py#L1270) — Sample a parent program from the current island for the next evolution step
  - `_sample_random_parent(self)` — [`L1416`](../../../../../raw/code/openevolve/openevolve/database.py#L1416) — Sample a completely random parent from all programs
  - `_save_program(self, program: Program, base_path: Optional[str] = None, prompts: Optional[Dict[str, Dict[str, str]]] = None)` — [`L803`](../../../../../raw/code/openevolve/openevolve/database.py#L803) — Save a program to disk
  - `_scale_feature_value(self, feature_name: str, value: float)` — [`L2193`](../../../../../raw/code/openevolve/openevolve/database.py#L2193) — Scale a feature value according to the configured scaling method
  - `_scale_feature_value_minmax(self, feature_name: str, value: float)` — [`L2236`](../../../../../raw/code/openevolve/openevolve/database.py#L2236) — Helper for min-max scaling
  - `_serialize_feature_stats(self)` — [`L2251`](../../../../../raw/code/openevolve/openevolve/database.py#L2251) — Serialize feature_stats for JSON storage
  - `_update_archive(self, program: Program)` — [`L1131`](../../../../../raw/code/openevolve/openevolve/database.py#L1131) — Update the archive of elite programs
  - `_update_best_program(self, program: Program)` — [`L1178`](../../../../../raw/code/openevolve/openevolve/database.py#L1178) — Update the absolute best program tracking
  - `_update_diversity_reference_set(self)` — [`L2108`](../../../../../raw/code/openevolve/openevolve/database.py#L2108) — Update the reference set for diversity calculation
  - `_update_feature_stats(self, feature_name: str, value: float)` — [`L2169`](../../../../../raw/code/openevolve/openevolve/database.py#L2169) — Update statistics for a feature dimension
  - `_update_island_best_program(self, program: Program, island_idx: int)` — [`L1218`](../../../../../raw/code/openevolve/openevolve/database.py#L1218) — Update the best program tracking for a specific island
  - `_validate_migration_results(self)` — [`L1882`](../../../../../raw/code/openevolve/openevolve/database.py#L1882) — Validate migration didn't create inconsistencies
  - `_write_artifact_file(self, artifact_dir: str, key: str, value: Union[str, bytes])` — [`L2485`](../../../../../raw/code/openevolve/openevolve/database.py#L2485) — Write an artifact to a file
  - `add(self, program: Program, iteration: int = None, target_island: Optional[int] = None)` — [`L211`](../../../../../raw/code/openevolve/openevolve/database.py#L211) — Add a program to the database — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `get(self, program_id: str)` — [`L370`](../../../../../raw/code/openevolve/openevolve/database.py#L370) — Get a program by ID
  - `get_artifacts(self, program_id: str)` — [`L2379`](../../../../../raw/code/openevolve/openevolve/database.py#L2379) — Retrieve all artifacts for a program
  - `get_best_program(self, metric: Optional[str] = None)` — [`L472`](../../../../../raw/code/openevolve/openevolve/database.py#L472) — Get the best program based on a metric — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `get_island_stats(self)` — [`L1974`](../../../../../raw/code/openevolve/openevolve/database.py#L1974) — Get statistics for each island
  - `get_top_programs(self, n: int = 10, metric: Optional[str] = None, island_idx: Optional[int] = None)` — [`L538`](../../../../../raw/code/openevolve/openevolve/database.py#L538) — Get the top N programs based on a metric
  - `increment_island_generation(self, island_idx: Optional[int] = None)` — [`L1769`](../../../../../raw/code/openevolve/openevolve/database.py#L1769) — Increment generation counter for an island
  - `load(self, path: str)` — [`L639`](../../../../../raw/code/openevolve/openevolve/database.py#L639) — Load the database from disk — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `log_island_status(self)` — [`L2311`](../../../../../raw/code/openevolve/openevolve/database.py#L2311) — Log current status of all islands
  - `log_prompt(self, program_id: str, template_key: str, prompt: Dict[str, str], responses: Optional[List[str]] = None)` — [`L2533`](../../../../../raw/code/openevolve/openevolve/database.py#L2533) — Log a prompt for a program. — documented in [openevolve-evaluator](../../concepts/openevolve-evaluator.md)
  - `migrate_programs(self)` — [`L1780`](../../../../../raw/code/openevolve/openevolve/database.py#L1780) — Perform migration between islands — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `next_island(self)` — [`L1763`](../../../../../raw/code/openevolve/openevolve/database.py#L1763) — Move to the next island in round-robin fashion
  - `sample(self, num_inspirations: Optional[int] = None)` — [`L382`](../../../../../raw/code/openevolve/openevolve/database.py#L382) — Sample a program and inspirations for the next evolution step
  - `sample_from_island(self, island_id: int, num_inspirations: Optional[int] = None)` — [`L403`](../../../../../raw/code/openevolve/openevolve/database.py#L403) — Sample a program and inspirations from a specific island without modifying current_island — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `save(self, path: Optional[str] = None, iteration: int = 0)` — [`L590`](../../../../../raw/code/openevolve/openevolve/database.py#L590) — Save the database to disk — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `set_current_island(self, island_idx: int)` — [`L1758`](../../../../../raw/code/openevolve/openevolve/database.py#L1758) — Set which island is currently being evolved
  - `should_migrate(self)` — [`L1775`](../../../../../raw/code/openevolve/openevolve/database.py#L1775) — Check if migration should occur based on generation counters
  - `store_artifacts(self, program_id: str, artifacts: Dict[str, Union[str, bytes]])` — [`L2332`](../../../../../raw/code/openevolve/openevolve/database.py#L2332) — Store artifacts for a program — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `archive` — [`L152`](../../../../../raw/code/openevolve/openevolve/database.py#L152)
  - `best_program_id` — [`L155`](../../../../../raw/code/openevolve/openevolve/database.py#L155) — documented in [openevolve-api](../../concepts/openevolve-api.md)
  - `config` — [`L123`](../../../../../raw/code/openevolve/openevolve/database.py#L123) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `current_island` — [`L145`](../../../../../raw/code/openevolve/openevolve/database.py#L145) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `diversity_cache` — [`L178`](../../../../../raw/code/openevolve/openevolve/database.py#L178)
  - `diversity_cache_size` — [`L181`](../../../../../raw/code/openevolve/openevolve/database.py#L181)
  - `diversity_reference_set` — [`L182`](../../../../../raw/code/openevolve/openevolve/database.py#L182)
  - `diversity_reference_size` — [`L185`](../../../../../raw/code/openevolve/openevolve/database.py#L185)
  - `embedding_client` — [`L206`](../../../../../raw/code/openevolve/openevolve/database.py#L206)
  - `feature_bins` — [`L133`](../../../../../raw/code/openevolve/openevolve/database.py#L133)
  - `feature_bins_per_dim` — [`L193`](../../../../../raw/code/openevolve/openevolve/database.py#L193)
  - `feature_scaling_method` — [`L189`](../../../../../raw/code/openevolve/openevolve/database.py#L189)
  - `feature_stats` — [`L188`](../../../../../raw/code/openevolve/openevolve/database.py#L188)
  - `island_best_programs` — [`L158`](../../../../../raw/code/openevolve/openevolve/database.py#L158) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `island_feature_maps` — [`L129`](../../../../../raw/code/openevolve/openevolve/database.py#L129) — documented in [openevolve-controller](../../concepts/openevolve-controller.md)
  - `island_generations` — [`L146`](../../../../../raw/code/openevolve/openevolve/database.py#L146) — documented in [openevolve-process_parallel](../../concepts/openevolve-process_parallel.md)
  - `islands` — [`L142`](../../../../../raw/code/openevolve/openevolve/database.py#L142) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `last_iteration` — [`L161`](../../../../../raw/code/openevolve/openevolve/database.py#L161)
  - `last_migration_generation` — [`L147`](../../../../../raw/code/openevolve/openevolve/database.py#L147)
  - `migration_interval` — [`L148`](../../../../../raw/code/openevolve/openevolve/database.py#L148)
  - `migration_rate` — [`L149`](../../../../../raw/code/openevolve/openevolve/database.py#L149)
  - `novelty_llm` — [`L205`](../../../../../raw/code/openevolve/openevolve/database.py#L205)
  - `programs` — [`L126`](../../../../../raw/code/openevolve/openevolve/database.py#L126) — documented in [openevolve-database](../../concepts/openevolve-database.md)
  - `prompts_by_program` — [`L168`](../../../../../raw/code/openevolve/openevolve/database.py#L168)
  - `similarity_threshold` — [`L209`](../../../../../raw/code/openevolve/openevolve/database.py#L209)
- protocol/private: `__init__`[`L122`](../../../../../raw/code/openevolve/openevolve/database.py#L122)
- uses (calls/refs, reference-scoped): [`id`](database.md#Program.id), [`metrics`](database.md#Program.metrics), [`Program`](database.md#Program), [`code`](database.md#Program.code), [`logger`](database.md#logger), [`metadata`](database.md#Program.metadata), [`language`](database.md#Program.language), [`DatabaseConfig`](config.md#DatabaseConfig), [`feature_dimensions`](config.md#DatabaseConfig.feature_dimensions), [`num_islands`](config.md#DatabaseConfig.num_islands), [`generation`](database.md#Program.generation), [`parent_id`](database.md#Program.parent_id), [`get_fitness_score`](utils/metrics_utils.md#get_fitness_score), [`iteration_found`](database.md#Program.iteration_found), [`db_path`](config.md#DatabaseConfig.db_path), [`population_size`](config.md#DatabaseConfig.population_size), [`exploration_ratio`](config.md#DatabaseConfig.exploration_ratio), [`feature_bins`](config.md#DatabaseConfig.feature_bins), [`changes_description`](database.md#Program.changes_description), [`exploitation_ratio`](config.md#DatabaseConfig.exploitation_ratio), [`safe_numeric_average`](utils/metrics_utils.md#safe_numeric_average), [`artifact_dir`](database.md#Program.artifact_dir), [`to_dict`](database.md#Program.to_dict), [`get_embedding`](embedding.md#EmbeddingClient.get_embedding), [`artifacts_json`](database.md#Program.artifacts_json), [`generate_with_context`](llm/base.md#LLMInterface.generate_with_context), [`novelty_llm`](config.md#DatabaseConfig.novelty_llm), [`from_dict`](database.md#Program.from_dict), [`random_seed`](config.md#DatabaseConfig.random_seed), [`timestamp`](database.md#Program.timestamp), [`archive_size`](config.md#DatabaseConfig.archive_size), [`complexity`](database.md#Program.complexity), [`diversity`](database.md#Program.diversity), [`NOVELTY_SYSTEM_MSG`](novelty_judge.md#NOVELTY_SYSTEM_MSG), [`embedding`](database.md#Program.embedding), [`embedding_model`](config.md#DatabaseConfig.embedding_model), [`log_prompts`](config.md#DatabaseConfig.log_prompts), [`similarity_threshold`](config.md#DatabaseConfig.similarity_threshold), [`EmbeddingClient`](embedding.md#EmbeddingClient), [`NOVELTY_USER_MSG`](novelty_judge.md#NOVELTY_USER_MSG)  (+3 more)
- used by: [`run_iteration_with_shared_db`](iteration.md#run_iteration_with_shared_db), [`run`](controller.md#OpenEvolve.run), [`database`](controller.md#OpenEvolve.database), [`run_evolution`](process_parallel.md#ProcessParallelController.run_evolution), [`_warned_about_combined_score`](process_parallel.md#ProcessParallelController._warned_about_combined_score), [`_save_checkpoint`](controller.md#OpenEvolve._save_checkpoint), [`main_async`](cli.md#main_async), [`_save_best_program`](controller.md#OpenEvolve._save_best_program), [`_submit_iteration`](process_parallel.md#ProcessParallelController._submit_iteration), [`_llm_evaluate`](evaluator.md#Evaluator._llm_evaluate), [`_run_evolution_with_checkpoints`](controller.md#OpenEvolve._run_evolution_with_checkpoints), [`_create_database_snapshot`](process_parallel.md#ProcessParallelController._create_database_snapshot), [`_load_checkpoint`](controller.md#OpenEvolve._load_checkpoint), [`__init__`](evaluator.md#Evaluator.__init__), [`__init__`](process_parallel.md#ProcessParallelController.__init__)  (169 test-only)

## Functions
- `_safe_avg_metrics(metrics: Dict[str, Any])` — [`L35`](../../../../../raw/code/openevolve/openevolve/database.py#L35) — Safely calculate average of only numeric metric values
- `_safe_sum_metrics(metrics: Dict[str, Any])` — [`L27`](../../../../../raw/code/openevolve/openevolve/database.py#L27) — Safely sum only numeric metric values, ignoring strings and other types

## Module values
- `logger` — [`L24`](../../../../../raw/code/openevolve/openevolve/database.py#L24)

