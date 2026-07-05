---
title: 'Module: rdagent/oai/utils/embedding.py'
type: catalog
provenance: extracted
module: rdagent/oai/utils/embedding.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.oai.utils.embedding`/
symbols:
  get_embedding_max_tokens: get_embedding_max_tokens().
  trim_text_for_embedding: trim_text_for_embedding().
  truncate_content_list: truncate_content_list().
  EMBEDDING_MODEL_LIMITS: EMBEDDING_MODEL_LIMITS.
---
# Module: [`rdagent/oai/utils/embedding.py`](../../../../../../../raw/code/rd-agent/rdagent/oai/utils/embedding.py)

## Functions
- `get_embedding_max_tokens(model: str)` — [`L27`](../../../../../../../raw/code/rd-agent/rdagent/oai/utils/embedding.py#L27) — Get maximum token limit for embedding model.
- `trim_text_for_embedding(text: str, model: str, max_tokens: Optional[int] = None)` — [`L63`](../../../../../../../raw/code/rd-agent/rdagent/oai/utils/embedding.py#L63) — Truncate text for embedding model using encode/decode approach.
- `truncate_content_list(content_list: list[str], model: str)` — [`L118`](../../../../../../../raw/code/rd-agent/rdagent/oai/utils/embedding.py#L118) — Truncate a list of content strings.

## Module values
- `EMBEDDING_MODEL_LIMITS` — [`L13`](../../../../../../../raw/code/rd-agent/rdagent/oai/utils/embedding.py#L13)

