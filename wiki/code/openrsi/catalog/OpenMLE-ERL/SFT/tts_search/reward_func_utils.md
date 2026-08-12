---
title: 'Module: OpenMLE-ERL/SFT/tts_search/reward_func_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/reward_func_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.reward_func_utils`/
symbols:
  score2reward: score2reward().
  get_sandbox_result: get_sandbox_result().
  console_handler: console_handler.
  extract_code: extract_code().
  _bounds_signed.to_signed: _bounds_signed().to_signed().
  format_sandbox_feedback: format_sandbox_feedback().
  get_clear_log: get_clear_log().
  normalize_sandbox_resource_type: normalize_sandbox_resource_type().
  logger: logger.
  resolve_sandbox_resource_type: resolve_sandbox_resource_type().
  _bounds_signed: _bounds_signed().
  _stable_sigmoid: _stable_sigmoid().
  get_sandbox_result.safe_json: get_sandbox_result().safe_json().
  get_sandbox_result.format_httpx_error: get_sandbox_result().format_httpx_error().
  format_code: format_code().
  _RECENT: _RECENT.
  is_valid_python_script: is_valid_python_script().
  _RECENT_MAXLEN: _RECENT_MAXLEN.
  _signed: _signed().
  _finite: _finite().
  score2reward.safe_max: score2reward().safe_max().
  score2reward.safe_min: score2reward().safe_min().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/reward_func_utils.py`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py)

## Functions
- `_bounds_signed(meta: dict)` — [`L321`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L321)
- `_finite(x)` — [`L314`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L314)
- `_signed(score: float, meta: dict)` — [`L308`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L308)
- `_stable_sigmoid(x: float)` — [`L301`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L301)
- `extract_code(text)` — [`L271`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L271) — Extract python code blocks from the text. — documented in [OpenMLE-ERL-SFT-tts_search-services-generator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md)
- `format_code(code)` — [`L263`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L263) — Format Python code using Black.
- `format_httpx_error(exc: Exception, fallback_url: str)` — [`L101`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L101)
- `format_sandbox_feedback(status_code: int, payload: dict)` — [`L541`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L541) — Format sandbox execution results into feedback message — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- `get_clear_log(run_log: str | None)` — [`L481`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L481) — Extract marked output sections and remove heartbeat log blocks. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- `get_sandbox_result(client: httpx.AsyncClient, code_str: str, data_dir: str, *, resource_type: str = "gpu", priority: int = 1, job_timeout: int = 3600, wait_timeout: int = 7200, poll_interval: int = 5)` — [`L53`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L53) — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- `is_valid_python_script(script)` — [`L254`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L254) — Check if a script is a valid Python script.
- `normalize_sandbox_resource_type(resource_type: str | None, default: str = "gpu")` — [`L24`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L24) — Normalize sandbox resource type to cpu/gpu with a safe default. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- `resolve_sandbox_resource_type(metadata: dict | None, override: str | None = None, default: str = "gpu")` — [`L41`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L41) — Resolve effective sandbox resource type from override or task metadata. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- `safe_json(resp: httpx.Response)` — [`L94`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L94)
- `safe_max(*vals)` — [`L361`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L361)
- `safe_min(*vals)` — [`L365`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L365)
- `score2reward(score, metadata, mode="logistic")` — [`L353`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L353) — Map a metric score to a normalized reward. — documented in [OpenMLE-ERL-SFT-tts_search-services-evaluator](../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md)
- `to_signed(v)` — [`L324`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L324)

## Module values
- `_RECENT` — [`L297`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L297)
- `_RECENT_MAXLEN` — [`L298`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L298)
- `console_handler` — [`L18`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L18)
- `logger` — [`L15`](../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/reward_func_utils.py#L15)

