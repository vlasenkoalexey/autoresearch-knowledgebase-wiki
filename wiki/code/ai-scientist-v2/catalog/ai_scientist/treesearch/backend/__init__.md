---
title: 'Module: ai_scientist/treesearch/backend/__init__.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/backend/__init__.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.backend`/
symbols:
  query: query().
  get_ai_client: get_ai_client().
---
# Module: [`ai_scientist/treesearch/backend/__init__.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/__init__.py)

## Functions
- `get_ai_client(model: str, **model_kwargs)` — [`L4`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/__init__.py#L4) — Get the appropriate AI client based on the model string. — documented in [ai_scientist-treesearch-log_summarization](../../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `query(system_message: PromptType | None, user_message: PromptType | None, model: str, temperature: float | None = None, max_tokens: int | None = None, func_spec: FunctionSpec | None = None, **model_kwargs)` — [`L19`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/backend/__init__.py#L19) — General LLM query for various backends with a single system and user message. — documented in [ai_scientist-treesearch-agent_manager](../../../../concepts/ai_scientist-treesearch-agent_manager.md)

