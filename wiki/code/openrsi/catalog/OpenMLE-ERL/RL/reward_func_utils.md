---
title: 'Module: OpenMLE-ERL/RL/reward_func_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/RL/reward_func_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.RL.reward_func_utils`/
symbols:
  _finite: _finite().
  score2reward: score2reward().
  hack_check_async: hack_check_async().
  logger: logger.
  apply_validation_test_gap_penalty: apply_validation_test_gap_penalty().
  get_sandbox_result: get_sandbox_result().
  score2reward_with_static_priority: score2reward_with_static_priority().
  _load_public_leaderboard: _load_public_leaderboard().
  _get_async_hack_check_runtime: _get_async_hack_check_runtime().
  hack_check: hack_check().
  VALIDATION_TEST_GAP_PENALTY_COEF: VALIDATION_TEST_GAP_PENALTY_COEF.
  VALIDATION_TEST_GAP_PENALTY_HIGH_COEF: VALIDATION_TEST_GAP_PENALTY_HIGH_COEF.
  _leaderboard_medal_for_score.score_at_position: _leaderboard_medal_for_score().score_at_position().
  VALIDATION_TEST_GAP_PENALTY_TOLERANCE: VALIDATION_TEST_GAP_PENALTY_TOLERANCE.
  _preferred_static_bounds_signed: _preferred_static_bounds_signed().
  POWER_CLIP_ALPHA: POWER_CLIP_ALPHA.
  extract_code: extract_code().
  leaderboard_medal_binary_reward: leaderboard_medal_binary_reward().
  leaderboard_rank_reward: leaderboard_rank_reward().
  _bounds_signed: _bounds_signed().
  has_static_bounds_with_priority: has_static_bounds_with_priority().
  HACK_CHECK_CONCURRENCY: HACK_CHECK_CONCURRENCY.
  _leaderboard_medal_for_score: _leaderboard_medal_for_score().
  args: args.
  validation_test_gap_info: validation_test_gap_info().
  console_handler: console_handler.
  _parse_hack_check_completion: _parse_hack_check_completion().
  _PUBLIC_LEADERBOARD_CACHE: _PUBLIC_LEADERBOARD_CACHE.
  VALIDATION_TEST_GAP_PENALTY_ENABLED: VALIDATION_TEST_GAP_PENALTY_ENABLED.
  VALIDATION_TEST_GAP_PENALTY_PIECEWISE_ENABLED: VALIDATION_TEST_GAP_PENALTY_PIECEWISE_ENABLED.
  _static_bound_limits_signed.to_signed: _static_bound_limits_signed().to_signed().
  get_bound_limits_signed: get_bound_limits_signed().
  _apply_max_range: _apply_max_range().
  _preferred_static_bounds_signed.to_signed: _preferred_static_bounds_signed().to_signed().
  choose_validation_test_gap_denominator: choose_validation_test_gap_denominator().
  test_score2reward: test_score2reward().
  signed_score: signed_score().
  GPT_API_KEY: GPT_API_KEY.
  GPT_BASE_URL: GPT_BASE_URL.
  GPU_BASE_URL: GPU_BASE_URL.
  has_final_validation_score_print: has_final_validation_score_print().
  extract_validation_score: extract_validation_score().
  format_code: format_code().
  _range_size: _range_size().
  _leaderboard_roots: _leaderboard_roots().
  _static_bound_limits_signed: _static_bound_limits_signed().
  parser: parser.
  get_clear_log: get_clear_log().
  test_score2reward.percentile_index: test_score2reward().percentile_index().
  is_valid_python_script: is_valid_python_script().
  get_proxy_sandbox_result: get_proxy_sandbox_result().
  _signed: _signed().
  test_hack_check: test_hack_check().
  SANDBOX_API_KEY: SANDBOX_API_KEY.
  _HACK_CHECK_RUNTIMES: _HACK_CHECK_RUNTIMES.
  _env_flag: _env_flag().
  _build_hack_check_messages: _build_hack_check_messages().
  _is_retryable_hack_check_error: _is_retryable_hack_check_error().
  get_sandbox_result.safe_json: get_sandbox_result().safe_json().
  get_sandbox_result.format_httpx_error: get_sandbox_result().format_httpx_error().
  _RECENT: _RECENT.
  LEADERBOARD_ROOT: LEADERBOARD_ROOT.
  _stable_sigmoid: _stable_sigmoid().
  _leaderboard_lower_is_better: _leaderboard_lower_is_better().
  HF_ENDPOINT: HF_ENDPOINT.
  _HACK_CHECK_RUNTIME_LOCK: _HACK_CHECK_RUNTIME_LOCK.
  FINAL_VALIDATION_SCORE_PRINT_RE: FINAL_VALIDATION_SCORE_PRINT_RE.
  FINAL_VALIDATION_SCORE_VALUE_RE: FINAL_VALIDATION_SCORE_VALUE_RE.
  extract_json: extract_json().
  _iter_code_candidates: _iter_code_candidates().
  _RECENT_MAXLEN: _RECENT_MAXLEN.
  _task_name_from_metadata: _task_name_from_metadata().
  _public_leaderboard_candidates: _public_leaderboard_candidates().
  _normalize_leaderboard_columns: _normalize_leaderboard_columns().
  score2reward.safe_max: score2reward().safe_max().
  score2reward.safe_min: score2reward().safe_min().
  CPU_BASE_URL: CPU_BASE_URL.
  DEFAULT_LEADERBOARD_ROOTS.DEFAULT_LEADERBOARD_ROOTS: DEFAULT_LEADERBOARD_ROOTS.DEFAULT_LEADERBOARD_ROOTS.
---
# Module: [`OpenMLE-ERL/RL/reward_func_utils.py`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py)

## Functions
- `_apply_max_range(best, worst, fallback_best=None, fallback_worst=None)` — [`L1097`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1097) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_bounds_signed(meta: dict)` — [`L1113`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1113) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_build_hack_check_messages(code: str, require_holdout_validation: bool)` — [`L131`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L131) — Shared judge prompts for sync and async hack_check paths. — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_env_flag(name: str, default: bool)` — [`L66`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L66)
- `_finite(x)` — [`L774`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L774)
- `_get_async_hack_check_runtime()` — [`L231`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L231) — Per-event-loop AsyncOpenAI client + concurrency semaphore. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `_is_retryable_hack_check_error(exc: Exception)` — [`L183`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L183) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_iter_code_candidates(code)` — [`L714`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L714)
- `_leaderboard_lower_is_better(leaderboard: pd.DataFrame)` — [`L986`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L986)
- `_leaderboard_medal_for_score(score: float, leaderboard: pd.DataFrame)` — [`L991`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L991)
- `_leaderboard_roots()` — [`L903`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L903)
- `_load_public_leaderboard(meta: dict)` — [`L940`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L940) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_normalize_leaderboard_columns(leaderboard: pd.DataFrame)` — [`L928`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L928)
- `_parse_hack_check_completion(completion, require_holdout_validation: bool)` — [`L209`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L209) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_preferred_static_bounds_signed(meta: dict, priority: str = "leaderboard", fallback_best: float | None = None, fallback_worst: float | None = None)` — [`L1137`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1137) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_public_leaderboard_candidates(root: Path, task_name: str)` — [`L921`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L921)
- `_range_size(low, high)` — [`L781`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L781)
- `_signed(score: float, meta: dict)` — [`L763`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L763) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_stable_sigmoid(x: float)` — [`L756`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L756) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_static_bound_limits_signed(meta: dict)` — [`L1063`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1063) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_task_name_from_metadata(meta: dict)` — [`L893`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L893)
- `apply_validation_test_gap_penalty(reward, relative_gap, penalty_coef: float | None = None, gap_tolerance: float | None = None, high_penalty_coef: float | None = None, enabled: bool | None = None, piecewise_enabled: bool | None = None)` — [`L846`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L846) — Penalize positive rewards by validation/test relative gap. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `choose_validation_test_gap_denominator(metadata: dict, validation_score, test_score, *, theoretical_small_range_max: float = 2, big_range_threshold: float = 100, no_range_is_big: bool = True)` — [`L788`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L788) — Choose the score scale used to normalize validation/test gap. — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `extract_code(text)` — [`L720`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L720) — Extract python code blocks from the text. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `extract_json(text: str)` — [`L97`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L97) — Extract JSON content from text, removing markdown code blocks if present. — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `extract_validation_score(text: str | None)` — [`L117`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L117) — Extract the final validation score printed by generated code.
- `format_code(code)` — [`L705`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L705) — Format Python code using Black.
- `format_httpx_error(exc: Exception, fallback_url: str)` — [`L514`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L514)
- `get_bound_limits_signed(meta: dict)` — [`L1092`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1092) — Return one-sided signed-space metadata limits: (best_limit, worst_limit).
- `get_clear_log(run_log: str | None)` — [`L408`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L408) — Extract core output from run_log using the wrapper markers:
- `get_proxy_sandbox_result(client: httpx.AsyncClient, code_str: str, data_dir: str, *, resource_type: str = "all", job_timeout: int = 3600, wait_timeout: int = 3800, poll_interval: int = 5)` — [`L659`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L659) — Proxy sandbox result for fast RL plumbing tests.
- `get_sandbox_result(client: httpx.AsyncClient, code_str: str, data_dir: str, *, resource_type: str = "gpu", priority: int = 1, job_timeout: int = 3600, wait_timeout: int = 7200, poll_interval: int = 5)` — [`L473`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L473) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `hack_check(code: str, model: str = "o3-mini", temperature: float = 0, require_holdout_validation: bool = False)` — [`L253`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L253) — Sync GPT judge for cheating/guessing code. Prefer hack_check_async in rollout. — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `hack_check_async(code: str, model: str = "o3-mini", temperature: float = 0, require_holdout_validation: bool = False)` — [`L317`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L317) — Async concurrent hack_check for rollout. Cap via HACK_CHECK_CONCURRENCY (default 64). — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `has_final_validation_score_print(code: str)` — [`L112`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L112) — Check whether the code prints a Final Validation Score via an f-string.
- `has_static_bounds_with_priority(metadata: dict, priority: str = "leaderboard", fallback_best: float | None = None, fallback_worst: float | None = None)` — [`L1176`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1176) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `is_valid_python_script(script)` — [`L695`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L695) — Check if a script is a valid Python script.
- `leaderboard_medal_binary_reward(score, metadata: dict)` — [`L1037`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1037) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `leaderboard_rank_reward(score, metadata: dict)` — [`L1044`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1044) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `percentile_index(pct: float)` — [`L1492`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1492) — Calculate index for a given percentile (0.0 to 1.0).
- `safe_json(resp: httpx.Response)` — [`L507`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L507)
- `safe_max(*vals)` — [`L1298`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1298)
- `safe_min(*vals)` — [`L1302`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1302)
- `score2reward(score, metadata, mode="logistic", power_alpha: float | None = None)` — [`L1288`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1288) — Map a metric score to a reward. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `score2reward_with_static_priority(score, metadata, mode="logistic", priority="leaderboard", fallback_best: float | None = None, fallback_worst: float | None = None, power_alpha: float | None = None)` — [`L1191`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1191) — Map score to reward using static bounds with an explicit source priority. — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `score_at_position(position: int)` — [`L998`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L998) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `signed_score(score: float, meta: dict)` — [`L769`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L769) — Public helper for converting raw score to signed score.
- `test_hack_check(code_list: list[str], labels: list[str] = None)` — [`L1542`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1542) — Test the hack_check function on a list of code samples.
- `test_score2reward(base_dir: str)` — [`L1417`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1417) — Test score2reward function for all tasks in Selected_Dojo. — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `to_signed(v)` — [`L1066`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1066)
- `to_signed(v)` — [`L1145`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1145)
- `validation_test_gap_info(validation_score, test_score, metadata: dict)` — [`L822`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L822) — Return absolute and relative validation/test gap information. — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)

## Module values
- `CPU_BASE_URL` — [`L37`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L37)
- `DEFAULT_LEADERBOARD_ROOTS` — [`L751`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L751)
- `FINAL_VALIDATION_SCORE_PRINT_RE` — [`L59`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L59)
- `FINAL_VALIDATION_SCORE_VALUE_RE` — [`L63`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L63)
- `GPT_API_KEY` — [`L34`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L34) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `GPT_BASE_URL` — [`L35`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L35) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `GPU_BASE_URL` — [`L36`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L36)
- `HACK_CHECK_CONCURRENCY` — [`L43`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L43) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `HF_ENDPOINT` — [`L38`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L38)
- `LEADERBOARD_ROOT` — [`L752`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L752)
- `POWER_CLIP_ALPHA` — [`L52`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L52) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `SANDBOX_API_KEY` — [`L25`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L25)
- `VALIDATION_TEST_GAP_PENALTY_COEF` — [`L76`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L76) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `VALIDATION_TEST_GAP_PENALTY_ENABLED` — [`L73`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L73)
- `VALIDATION_TEST_GAP_PENALTY_HIGH_COEF` — [`L83`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L83) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `VALIDATION_TEST_GAP_PENALTY_PIECEWISE_ENABLED` — [`L74`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L74)
- `VALIDATION_TEST_GAP_PENALTY_TOLERANCE` — [`L90`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L90) — documented in [OpenMLE-ERL-RL-generate_mle](../../../concepts/OpenMLE-ERL-RL-generate_mle.md)
- `_HACK_CHECK_RUNTIMES` — [`L49`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L49) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_HACK_CHECK_RUNTIME_LOCK` — [`L48`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L48) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_PUBLIC_LEADERBOARD_CACHE` — [`L753`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L753) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_RECENT` — [`L749`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L749) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `_RECENT_MAXLEN` — [`L750`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L750) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `args` — [`L1603`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1603)
- `console_handler` — [`L21`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L21) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `logger` — [`L18`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L18) — documented in [OpenMLE-ERL-RL-reward_func_utils](../../../concepts/OpenMLE-ERL-RL-reward_func_utils.md)
- `parser` — [`L1601`](../../../../../../raw/code/openrsi/OpenMLE-ERL/RL/reward_func_utils.py#L1601)

