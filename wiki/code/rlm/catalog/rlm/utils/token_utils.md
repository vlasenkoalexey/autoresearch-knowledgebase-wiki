---
title: 'Module: rlm/utils/token_utils.py'
type: catalog
provenance: extracted
module: rlm/utils/token_utils.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.utils.token_utils`/
symbols:
  get_context_limit: get_context_limit().
  count_tokens: count_tokens().
  DEFAULT_CONTEXT_LIMIT: DEFAULT_CONTEXT_LIMIT.
  CHARS_PER_TOKEN_ESTIMATE: CHARS_PER_TOKEN_ESTIMATE.
  MODEL_CONTEXT_LIMITS.MODEL_CONTEXT_LIMITS: MODEL_CONTEXT_LIMITS.MODEL_CONTEXT_LIMITS.
  _count_tokens_tiktoken: _count_tokens_tiktoken().
---
# Module: [`rlm/utils/token_utils.py`](../../../../../../raw/code/rlm/rlm/utils/token_utils.py)

## Functions
- `_count_tokens_tiktoken(messages: list[dict[str, Any]], model_name: str)` — [`L92`](../../../../../../raw/code/rlm/rlm/utils/token_utils.py#L92) — Count tokens with tiktoken if available. Returns None on failure.
- `count_tokens(messages: list[dict[str, Any]], model_name: str)` — [`L125`](../../../../../../raw/code/rlm/rlm/utils/token_utils.py#L125) — Count tokens in a list of message dicts (role, content).
- `get_context_limit(model_name: str)` — [`L70`](../../../../../../raw/code/rlm/rlm/utils/token_utils.py#L70) — Return max context size in tokens for a model.

## Module values
- `CHARS_PER_TOKEN_ESTIMATE` — [`L14`](../../../../../../raw/code/rlm/rlm/utils/token_utils.py#L14)
- `DEFAULT_CONTEXT_LIMIT` — [`L11`](../../../../../../raw/code/rlm/rlm/utils/token_utils.py#L11)
- `MODEL_CONTEXT_LIMITS` — [`L19`](../../../../../../raw/code/rlm/rlm/utils/token_utils.py#L19)

