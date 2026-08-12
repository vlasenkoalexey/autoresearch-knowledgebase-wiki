---
title: 'Module: OpenMLE-ERL/RL/generate_mle.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/generate_mle.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.generate_mle`/
symbols:
  reward_func: reward_func().
  generate: generate().
  logger: logger.
  _resolve_group_reward_mapping: _resolve_group_reward_mapping().
  _maybe_update_airaevo_program_metadata: _maybe_update_airaevo_program_metadata().
  compute_metric_static_base_reward: compute_metric_static_base_reward().
  MLE_CONFIGS: MLE_CONFIGS.
  _compute_task_reward_frontier: _compute_task_reward_frontier().
  compute_static_score_reward: compute_static_score_reward().
  ADAPTIVE_REWARD_BOUND_MODE: ADAPTIVE_REWARD_BOUND_MODE.
  get_program_database: get_program_database().
  _ensure_prompt_dump_dir: _ensure_prompt_dump_dir().
  get_search_algorithm: get_search_algorithm().
  _get_loop_lock: _get_loop_lock().
  _build_adaptive_bound_metadata_context: _build_adaptive_bound_metadata_context().
  _get_program_reward_views: _get_program_reward_views().
  _is_finite_number: _is_finite_number().
  ADAPTIVE_REWARD_BOUND_LOWER_SHIFT_RATIO: ADAPTIVE_REWARD_BOUND_LOWER_SHIFT_RATIO.
  _dump_prompt_to_txt: _dump_prompt_to_txt().
  _get_dynamic_bound_task_lock: _get_dynamic_bound_task_lock().
  _use_group_adaptive_reward_bounds: _use_group_adaptive_reward_bounds().
  _parent_selection_cache: _parent_selection_cache.
  console_handler: console_handler.
  _prompt_dump_dir._prompt_dump_dir: _prompt_dump_dir._prompt_dump_dir.
  SANDBOX_CONCURRENCY: SANDBOX_CONCURRENCY.
  USE_SCORE2REWARD: USE_SCORE2REWARD.
  REWARD_MAPPING_MODE: REWARD_MAPPING_MODE.
  METRIC_STATIC_BOUND_USE_CONST_FALLBACK: METRIC_STATIC_BOUND_USE_CONST_FALLBACK.
  _get_loop_semaphore: _get_loop_semaphore().
  _get_sandbox_semaphore: _get_sandbox_semaphore().
  _search_algorithm: _search_algorithm.
  _update_history_best_static_base_reward: _update_history_best_static_base_reward().
  _return_generation_abort_for_retry: _return_generation_abort_for_retry().
  SANDBOX_CONCURRENT_COUNT: SANDBOX_CONCURRENT_COUNT.
  _program_database: _program_database.
  save_db_snapshot: save_db_snapshot().
  _history_static_base_reward_cache._history_static_base_reward_cache: _history_static_base_reward_cache._history_static_base_reward_cache.
  STATIC_REWARD_MAPPING_MODE: STATIC_REWARD_MAPPING_MODE.
  ADAPTIVE_BOUND_SINGLE_FINITE_REWARD_ONE: ADAPTIVE_BOUND_SINGLE_FINITE_REWARD_ONE.
  _LOOP_PRIMITIVES_LOCK: _LOOP_PRIMITIVES_LOCK.
  _DYNAMIC_SCORE_BOUND_TASK_LOCKS: _DYNAMIC_SCORE_BOUND_TASK_LOCKS.
  EVAL_JOB_TIMEOUT: EVAL_JOB_TIMEOUT.
  EVAL_WAIT_TIMEOUT: EVAL_WAIT_TIMEOUT.
  _dynamic_bound_task_identity: _dynamic_bound_task_identity().
  GPU_BASE_URL: GPU_BASE_URL.
  ENABLE_SELF_VALIDATION: ENABLE_SELF_VALIDATION.
  METRIC_STATIC_FALLBACK_SIGNED_BEST: METRIC_STATIC_FALLBACK_SIGNED_BEST.
  METRIC_STATIC_FALLBACK_SIGNED_WORST: METRIC_STATIC_FALLBACK_SIGNED_WORST.
  EVAL_GENERATION_ABORT_MAX_RETRIES: EVAL_GENERATION_ABORT_MAX_RETRIES.
  USE_PROXY_SANDBOX: USE_PROXY_SANDBOX.
  _apply_dynamic_bound_context_metadata: _apply_dynamic_bound_context_metadata().
  _adaptive_group_reward_cache._adaptive_group_reward_cache: _adaptive_group_reward_cache._adaptive_group_reward_cache.
  IMPROVE_REWARD_STRATEGY: IMPROVE_REWARD_STRATEGY.
  IMPROVE_DELTA_BONUS_COEF: IMPROVE_DELTA_BONUS_COEF.
  DYNAMIC_SCORE_BOUND_MIN_SPAN: DYNAMIC_SCORE_BOUND_MIN_SPAN.
  _LOOP_LOCKS: _LOOP_LOCKS.
  _LOOP_SEMAPHORES: _LOOP_SEMAPHORES.
  JOB_TIMEOUT: JOB_TIMEOUT.
  WAIT_TIMEOUT: WAIT_TIMEOUT.
  EVAL_GENERATION_ABORT_RETRY_SLEEP: EVAL_GENERATION_ABORT_RETRY_SLEEP.
  compute_mode_rewards: compute_mode_rewards().
  _get_search_selection_metadata: _get_search_selection_metadata().
  _normalize_token_ids: _normalize_token_ids().
  N_SAMPLES_PER_PROMPT: N_SAMPLES_PER_PROMPT.
  GENERATION_ABORT_CODE_CATEGORIES: GENERATION_ABORT_CODE_CATEGORIES.
  GENERATION_ABORT_TRANSIENT_METADATA_KEYS: GENERATION_ABORT_TRANSIENT_METADATA_KEYS.
  ENABLE_DYNAMIC_SCORE_BOUNDS: ENABLE_DYNAMIC_SCORE_BOUNDS.
  ENABLE_PROMPT_DUMP: ENABLE_PROMPT_DUMP.
  PROMPT_DUMP_BASE_DIR: PROMPT_DUMP_BASE_DIR.
  PROMPT_DUMP_RUN_SUBDIR: PROMPT_DUMP_RUN_SUBDIR.
  AIRAEVO_RICH_MEMORY_ENABLED: AIRAEVO_RICH_MEMORY_ENABLED.
  AIRAEVO_RICH_MEMORY_MAX_TOKENS: AIRAEVO_RICH_MEMORY_MAX_TOKENS.
  AIRAEVO_RICH_MEMORY_TIMEOUT: AIRAEVO_RICH_MEMORY_TIMEOUT.
  _dynamic_bound_task_key: _dynamic_bound_task_key().
  _group_cache_key: _group_cache_key().
  _to_token_id_list: _to_token_id_list().
  _extract_llm_text: _extract_llm_text().
  CPU_BASE_URL: CPU_BASE_URL.
---
# Module: [`OpenMLE-ERL/RL/generate_mle.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py)

## Functions
- `_apply_dynamic_bound_context_metadata(sample: Sample, context: dict, expected_group_count: int)` — [`L579`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L579)
- `_build_adaptive_bound_metadata_context(*, task_key: str, group_index: int | None, history_count: int, group_count: int, best_signed: float | None, worst_signed: float | None, group_generation_aborted: bool = False)` — [`L344`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L344) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `_compute_task_reward_frontier(db: ProgramDatabase, *, task_name: str, metadata_fallback: dict)` — [`L765`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L765) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `_dump_prompt_to_txt(*, task_name: str, task_id: str, group_index: int | None, mode: str, parent_program: Program | None, secondary_parent_program: Program | None, system_prompt: str, user_prompt: str)` — [`L256`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L256)
- `_dynamic_bound_task_identity(metadata: dict)` — [`L307`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L307)
- `_dynamic_bound_task_key(metadata: dict)` — [`L299`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L299)
- `_ensure_prompt_dump_dir()` — [`L241`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L241)
- `_extract_llm_text(output: dict)` — [`L892`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L892)
- `_get_dynamic_bound_task_lock(task_key: str)` — [`L314`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L314)
- `_get_loop_lock(name: str)` — [`L169`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L169) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `_get_loop_semaphore(name: str, value: int)` — [`L183`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L183)
- `_get_program_reward_views(program: Program | None)` — [`L747`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L747) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `_get_sandbox_semaphore()` — [`L197`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L197)
- `_get_search_selection_metadata(search_algo)` — [`L887`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L887)
- `_group_cache_key(task_key: str, group_index: int | None)` — [`L334`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L334)
- `_is_finite_number(value)` — [`L292`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L292)
- `_maybe_update_airaevo_program_metadata(args, db: ProgramDatabase, program: Program)` — [`L911`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L911) — documented in [OpenMLE-ERL-RL-airaevo_experience](../../../concepts/OpenMLE-ERL-RL-airaevo_experience.md)
- `_normalize_token_ids(token_ids)` — [`L961`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L961) — Normalize tokenizer/SGLang token containers to a plain list[int].
- `_resolve_group_reward_mapping(metadata: dict, *, group_index: int | None, group_size: int, sample_key: str, score: float | None, base_reward: float)` — [`L370`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L370) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `_return_generation_abort_for_retry(sample: Sample, *, task_name: str, group_index: int | None)` — [`L593`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L593)
- `_to_token_id_list(tokenized)` — [`L870`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L870) — Normalize tokenizer output to a flat list[int] for Sample.tokens.
- `_update_history_best_static_base_reward(task_name: str, best_before: float, current_value: float | None)` — [`L808`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L808)
- `_use_group_adaptive_reward_bounds()` — [`L340`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L340)
- `compute_metric_static_base_reward(score: float | None, metadata: dict)` — [`L698`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L698) — Metric-only static base reward: — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `compute_mode_rewards(*, generation_mode: str, effective_base_reward: float, parent_base_reward: float | None, parent_reward: float | None, parent_code: str, code: str, crossover_parent_base_reward: float | None = None, crossover_parent_reward: float | None = None, crossover_parent_code: str = "", improve_reward_strategy: str = "base", improve_delta_bonus_coef: float = 0.5)` — [`L614`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L614) — Compute shaped base reward and final reward for draft/improve/debug/crossover.
- `compute_static_score_reward(score: float | None, metadata: dict)` — [`L667`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L667) — Map score to the original static bounds reward, independent of dynamic reward mode. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `generate(args, sample: Sample, sampling_params, evaluation)` — [`L986`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L986) — Single-turn generation with draft/improve mode support. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `get_program_database()` — [`L825`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L825) — Get or create the global program database instance. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `get_search_algorithm()` — [`L837`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L837) — Get or create the global search algorithm instance. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `reward_func(args, sample, **kwargs)` — [`L1351`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L1351) — The reward function for code generation tasks. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `save_db_snapshot(snapshot_path: str)` — [`L2013`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L2013) — Save a snapshot of the program database.

## Module values
- `ADAPTIVE_BOUND_SINGLE_FINITE_REWARD_ONE` — [`L125`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L125)
- `ADAPTIVE_REWARD_BOUND_LOWER_SHIFT_RATIO` — [`L119`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L119)
- `ADAPTIVE_REWARD_BOUND_MODE` — [`L109`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L109) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `AIRAEVO_RICH_MEMORY_ENABLED` — [`L218`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L218)
- `AIRAEVO_RICH_MEMORY_MAX_TOKENS` — [`L219`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L219)
- `AIRAEVO_RICH_MEMORY_TIMEOUT` — [`L220`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L220)
- `CPU_BASE_URL` — [`L77`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L77)
- `DYNAMIC_SCORE_BOUND_MIN_SPAN` — [`L117`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L117)
- `ENABLE_DYNAMIC_SCORE_BOUNDS` — [`L103`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L103)
- `ENABLE_PROMPT_DUMP` — [`L212`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L212)
- `ENABLE_SELF_VALIDATION` — [`L89`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L89)
- `EVAL_GENERATION_ABORT_MAX_RETRIES` — [`L209`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L209)
- `EVAL_GENERATION_ABORT_RETRY_SLEEP` — [`L210`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L210)
- `EVAL_JOB_TIMEOUT` — [`L207`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L207)
- `EVAL_WAIT_TIMEOUT` — [`L208`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L208)
- `GENERATION_ABORT_CODE_CATEGORIES` — [`L68`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L68)
- `GENERATION_ABORT_TRANSIENT_METADATA_KEYS` — [`L69`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L69)
- `GPU_BASE_URL` — [`L76`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L76)
- `IMPROVE_DELTA_BONUS_COEF` — [`L102`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L102)
- `IMPROVE_REWARD_STRATEGY` — [`L101`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L101)
- `JOB_TIMEOUT` — [`L205`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L205)
- `METRIC_STATIC_BOUND_USE_CONST_FALLBACK` — [`L131`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L131)
- `METRIC_STATIC_FALLBACK_SIGNED_BEST` — [`L137`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L137)
- `METRIC_STATIC_FALLBACK_SIGNED_WORST` — [`L138`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L138)
- `MLE_CONFIGS` — [`L140`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L140) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `N_SAMPLES_PER_PROMPT` — [`L67`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L67)
- `PROMPT_DUMP_BASE_DIR` — [`L213`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L213)
- `PROMPT_DUMP_RUN_SUBDIR` — [`L217`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L217)
- `REWARD_MAPPING_MODE` — [`L87`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L87)
- `SANDBOX_CONCURRENCY` — [`L79`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L79)
- `SANDBOX_CONCURRENT_COUNT` — [`L202`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L202)
- `STATIC_REWARD_MAPPING_MODE` — [`L88`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L88)
- `USE_PROXY_SANDBOX` — [`L211`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L211)
- `USE_SCORE2REWARD` — [`L86`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L86)
- `WAIT_TIMEOUT` — [`L206`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L206)
- `_DYNAMIC_SCORE_BOUND_TASK_LOCKS` — [`L166`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L166)
- `_LOOP_LOCKS` — [`L164`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L164)
- `_LOOP_PRIMITIVES_LOCK` — [`L163`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L163)
- `_LOOP_SEMAPHORES` — [`L165`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L165)
- `_adaptive_group_reward_cache` — [`L238`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L238)
- `_history_static_base_reward_cache` — [`L236`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L236)
- `_parent_selection_cache` — [`L234`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L234)
- `_program_database` — [`L223`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L223)
- `_prompt_dump_dir` — [`L237`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L237)
- `_search_algorithm` — [`L226`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L226)
- `console_handler` — [`L62`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L62)
- `logger` — [`L59`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/generate_mle.py#L59)

