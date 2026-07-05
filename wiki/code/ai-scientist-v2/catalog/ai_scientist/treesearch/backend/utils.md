---
title: 'Module: ai_scientist/treesearch/backend/utils.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/backend/utils.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.backend.utils`/
symbols:
  FunctionSpec: FunctionSpec#
  compile_prompt_to_md: compile_prompt_to_md().
  logger: logger.
  FunctionSpec.name: FunctionSpec#name.
  FunctionSpec.json_schema: FunctionSpec#json_schema.
  FunctionSpec.description: FunctionSpec#description.
  OutputType: OutputType.
  FunctionSpec.as_openai_tool_dict: FunctionSpec#as_openai_tool_dict().
  backoff_create: backoff_create().
  PromptType: PromptType.
  opt_messages_to_list: opt_messages_to_list().
  FunctionSpec.openai_tool_choice_dict: FunctionSpec#openai_tool_choice_dict().
  FunctionSpec.__post_init__: FunctionSpec#__post_init__().
  FunctionCallType: FunctionCallType.
---
# Module: [`ai_scientist/treesearch/backend/utils.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py)

## Classes
### `FunctionSpec`
- def: [`ai_scientist/treesearch/backend/utils.py:106`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L106) — documented in [ai_scientist-treesearch-backend-utils](../../../../concepts/ai_scientist-treesearch-backend-utils.md)
- signature: `class FunctionSpec(DataClassJsonMixin):`
- members:
  - `as_openai_tool_dict(self)` — [`L116`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L116) — documented in [ai_scientist-treesearch-backend-utils](../../../../concepts/ai_scientist-treesearch-backend-utils.md)
  - `openai_tool_choice_dict(self)` — [`L127`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L127) — documented in [ai_scientist-treesearch-backend-utils](../../../../concepts/ai_scientist-treesearch-backend-utils.md)
  - `description` — [`L109`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L109)
  - `json_schema` — [`L108`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L108)
  - `name` — [`L107`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L107) — documented in [ai_scientist-treesearch-backend-utils](../../../../concepts/ai_scientist-treesearch-backend-utils.md)
- protocol/private: `__post_init__`[`L111`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L111)
- used by: [`query`](__init__.md#query), [`_generate_substage_goal`](../agent_manager.md#AgentManager._generate_substage_goal), [`query`](backend_openai.md#query), [`query`](backend_anthropic.md#query), [`stage_completion_eval_spec`](../agent_manager.md#stage_completion_eval_spec), [`metric_parse_spec`](../parallel_agent.md#metric_parse_spec), [`node_selection_spec`](../journal.md#node_selection_spec), [`plot_selection_spec`](../parallel_agent.md#plot_selection_spec), [`review_func_spec`](../parallel_agent.md#review_func_spec), [`stage_progress_eval_spec`](../agent_manager.md#stage_progress_eval_spec), [`vlm_feedback_spec`](../parallel_agent.md#vlm_feedback_spec), [`stage_config_spec`](../agent_manager.md#stage_config_spec)

## Functions
- `backoff_create(create_fn: Callable, retry_exceptions: list[Exception], *args, **kwargs)` — [`L23`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L23) — documented in [ai_scientist-treesearch-backend-utils](../../../../concepts/ai_scientist-treesearch-backend-utils.md)
- `compile_prompt_to_md(prompt: PromptType, _header_depth: int = 1)` — [`L44`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L44) — Convert a prompt into markdown format — documented in [ai_scientist-treesearch-backend-utils](../../../../concepts/ai_scientist-treesearch-backend-utils.md)
- `opt_messages_to_list(system_message: str | None, user_message: str | None)` — [`L33`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L33)

## Module values
- `FunctionCallType` — [`L7`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L7)
- `OutputType` — [`L8`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L8)
- `PromptType` — [`L6`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L6) — documented in [ai_scientist-treesearch-backend-utils](../../../../concepts/ai_scientist-treesearch-backend-utils.md)
- `logger` — [`L15`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/utils.py#L15) — documented in [ai_scientist-treesearch-backend-utils](../../../../concepts/ai_scientist-treesearch-backend-utils.md)

