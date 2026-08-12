---
title: 'Module: OpenMLE-Evo/tts_search/reward_func_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/tts_search/reward_func_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.tts_search.reward_func_utils`/
symbols:
  logger: logger.
  score2reward: score2reward().
  get_sandbox_result: get_sandbox_result().
  get_sandbox_result_deprecated: get_sandbox_result_deprecated().
  console_handler: console_handler.
  _bounds_signed.to_signed: _bounds_signed().to_signed().
  test_score2reward: test_score2reward().
  get_sandbox_result_deprecated.safe_json: get_sandbox_result_deprecated().safe_json().
  extract_code: extract_code().
  _bounds_signed: _bounds_signed().
  format_sandbox_feedback: format_sandbox_feedback().
  _build_retryable_sandbox_payload: _build_retryable_sandbox_payload().
  test_score2reward.percentile_index: test_score2reward().percentile_index().
  get_sandbox_result.retry_after_seconds: get_sandbox_result().retry_after_seconds().
  API_KEY: API_KEY.
  get_sandbox_result.safe_json: get_sandbox_result().safe_json().
  _stable_sigmoid: _stable_sigmoid().
  get_clear_log: get_clear_log().
  RETRYABLE_SANDBOX_STATUS_CODES: RETRYABLE_SANDBOX_STATUS_CODES.
  get_sandbox_result.format_httpx_error: get_sandbox_result().format_httpx_error().
  format_code: format_code().
  _RECENT: _RECENT.
  parse_final_validation_score: parse_final_validation_score().
  is_valid_python_script: is_valid_python_script().
  _RECENT_MAXLEN: _RECENT_MAXLEN.
  _signed: _signed().
  _finite: _finite().
  score2reward.safe_max: score2reward().safe_max().
  score2reward.safe_min: score2reward().safe_min().
  BASE_URL: BASE_URL.
---
# Module: [`OpenMLE-Evo/tts_search/reward_func_utils.py`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py)

## Functions
- `_bounds_signed(meta: dict)` — [`L527`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L527)
- `_build_retryable_sandbox_payload(*, error: str, detail: str, status_code: int | None = None, job_id: str | None = None, data: dict | None = None, error_type: str | None = None)` — [`L34`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L34)
- `_finite(x)` — [`L521`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L521)
- `_signed(score: float, meta: dict)` — [`L515`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L515)
- `_stable_sigmoid(x: float)` — [`L508`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L508)
- `extract_code(text)` — [`L479`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L479) — Extract python code blocks from the text.
- `format_code(code)` — [`L472`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L472) — Format Python code using Black.
- `format_httpx_error(exc: Exception, fallback_url: str)` — [`L246`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L246)
- `format_sandbox_feedback(status_code: int, payload: dict)` — [`L903`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L903) — Format sandbox execution results into feedback message
- `get_clear_log(run_log: str | None)` — [`L822`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L822) — 从 run_log 中提取核心输出，基于新的包裹标记：
- `get_sandbox_result(client: httpx.AsyncClient, code_str: str, data_dir: str, *, resource_type: str = "gpu", priority: int = 1, job_timeout: int = 3600, wait_timeout: int = 86400, poll_interval: int = 10, eval_split: str | None = None)` — [`L203`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L203)
- `get_sandbox_result_deprecated(client: httpx.AsyncClient, code_str: str, data_dir: str, *, resource_type: str, eval_split=None, priority: int = 1, job_timeout: int = 3600, wait_timeout: int = 86400, poll_interval: int = 5)` — [`L58`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L58)
- `is_valid_python_script(script)` — [`L464`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L464) — Check if a script is a valid Python script.
- `parse_final_validation_score(run_log: str | None)` — [`L887`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L887)
- `percentile_index(pct: float)` — [`L773`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L773) — Calculate index for a given percentile (0.0 to 1.0).
- `retry_after_seconds(resp: httpx.Response, fallback: float)` — [`L269`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L269)
- `safe_json(resp: httpx.Response)` — [`L93`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L93)
- `safe_json(resp: httpx.Response)` — [`L239`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L239)
- `safe_max(*vals)` — [`L568`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L568)
- `safe_min(*vals)` — [`L572`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L572)
- `score2reward(score, metadata, mode="logistic")` — [`L558`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L558) — 将 metric 的 score 映射为 reward。
- `test_score2reward(base_dir: str = "./Selected_Dojo")` — [`L698`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L698) — Test score2reward function for all tasks in Selected_Dojo.
- `to_signed(v)` — [`L530`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L530)

## Module values
- `API_KEY` — [`L29`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L29)
- `BASE_URL` — [`L28`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L28)
- `RETRYABLE_SANDBOX_STATUS_CODES` — [`L31`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L31)
- `_RECENT` — [`L505`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L505)
- `_RECENT_MAXLEN` — [`L506`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L506)
- `console_handler` — [`L22`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L22)
- `logger` — [`L19`](../../../../../../raw/code/openrsi/OpenMLE-Evo/tts_search/reward_func_utils.py#L19)

