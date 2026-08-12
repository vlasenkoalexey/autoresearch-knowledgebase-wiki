---
title: 'Module: utils/llm_provider_ui.py'
type: catalog
provenance: extracted
module: utils/llm_provider_ui.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.llm_provider_ui`/
symbols:
  infer_llm_provider_family: infer_llm_provider_family().
  _family_from_openrouter_model: _family_from_openrouter_model().
  _family_from_model_heuristic: _family_from_model_heuristic().
---
# Module: [`utils/llm_provider_ui.py`](../../../../../raw/code/continual-harness/utils/llm_provider_ui.py)

## Functions
- `_family_from_model_heuristic(model_lower: str)` — [`L8`](../../../../../raw/code/continual-harness/utils/llm_provider_ui.py#L8)
- `_family_from_openrouter_model(model_lower: str)` — [`L18`](../../../../../raw/code/continual-harness/utils/llm_provider_ui.py#L18)
- `infer_llm_provider_family(interaction_type: str, model: str = "", metadata_backend: str | None = None)` — [`L30`](../../../../../raw/code/continual-harness/utils/llm_provider_ui.py#L30) — Return one of: ``gemini``, ``openai``, ``anthropic``, ``other``.

