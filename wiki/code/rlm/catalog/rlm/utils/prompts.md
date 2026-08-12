---
title: 'Module: rlm/utils/prompts.py'
type: catalog
provenance: extracted
module: rlm/utils/prompts.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.utils.prompts`/
symbols:
  build_rlm_system_prompt: build_rlm_system_prompt().
  build_user_prompt: build_user_prompt().
  RLM_SYSTEM_PROMPT: RLM_SYSTEM_PROMPT.
  USER_PROMPT: USER_PROMPT.
  ORCHESTRATOR_ADDENDUM: ORCHESTRATOR_ADDENDUM.
  _DEFAULT_MAX_ITERATIONS: _DEFAULT_MAX_ITERATIONS.
  RLM_SYSTEM_PROMPT_OLD: RLM_SYSTEM_PROMPT_OLD.
  USER_PROMPT_OLD: USER_PROMPT_OLD.
  USER_PROMPT_WITH_ROOT_OLD: USER_PROMPT_WITH_ROOT_OLD.
---
# Module: [`rlm/utils/prompts.py`](../../../../../../raw/code/rlm/rlm/utils/prompts.py)

## Functions
- `build_rlm_system_prompt(system_prompt: str, query_metadata: QueryMetadata, custom_tools: dict[str, Any] | None = None, root_prompt: str | None = None, orchestrator: bool = True)` — [`L211`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L211) — documented in [rlm-environments-base_env](../../../concepts/rlm-environments-base_env.md)
- `build_user_prompt(root_prompt: str | None = None, iteration: int = 0, context_count: int = 1, history_count: int = 0, max_iterations: int = _DEFAULT_MAX_ITERATIONS)` — [`L251`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L251)

## Module values
- `ORCHESTRATOR_ADDENDUM` — [`L147`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L147)
- `RLM_SYSTEM_PROMPT` — [`L125`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L125)
- `RLM_SYSTEM_PROMPT_OLD` — [`L9`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L9)
- `USER_PROMPT` — [`L248`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L248)
- `USER_PROMPT_OLD` — [`L121`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L121)
- `USER_PROMPT_WITH_ROOT_OLD` — [`L122`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L122)
- `_DEFAULT_MAX_ITERATIONS` — [`L208`](../../../../../../raw/code/rlm/rlm/utils/prompts.py#L208)

