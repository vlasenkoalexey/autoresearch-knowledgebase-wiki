---
title: 'Module: openevolve/embedding.py'
type: catalog
provenance: extracted
module: openevolve/embedding.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.embedding`/
symbols:
  EmbeddingClient.get_embedding: EmbeddingClient#get_embedding().
  EmbeddingClient._get_client_model: EmbeddingClient#_get_client_model().
  EmbeddingClient.model: EmbeddingClient#model.
  OPENAI_EMBEDDING_COSTS: OPENAI_EMBEDDING_COSTS.
  M: M.
  EmbeddingClient: EmbeddingClient#
  logger: logger.
  OPENAI_EMBEDDING_MODELS: OPENAI_EMBEDDING_MODELS.
  AZURE_EMBEDDING_MODELS: AZURE_EMBEDDING_MODELS.
  EmbeddingClient.client: EmbeddingClient#client.
  EmbeddingClient.__init__: EmbeddingClient#__init__().
---
# Module: [`openevolve/embedding.py`](../../../../../raw/code/openevolve/openevolve/embedding.py)

## Classes
### `EmbeddingClient`
- def: [`openevolve/embedding.py:31`](../../../../../raw/code/openevolve/openevolve/embedding.py#L31)
- signature: `class EmbeddingClient:`
- members:
  - `__init__(self, model_name: str = "text-embedding-3-small")` — [`L32`](../../../../../raw/code/openevolve/openevolve/embedding.py#L32) — Initialize the EmbeddingClient.
  - `get_embedding(self, code: Union[str, List[str]])` — [`L61`](../../../../../raw/code/openevolve/openevolve/embedding.py#L61) — Computes the text embedding for a code string.
  - `client` — [`L39`](../../../../../raw/code/openevolve/openevolve/embedding.py#L39)
  - `model` — [`L39`](../../../../../raw/code/openevolve/openevolve/embedding.py#L39)
- protocol/private: `_get_client_model`[`L41`](../../../../../raw/code/openevolve/openevolve/embedding.py#L41)
- uses (calls/refs, reference-scoped): [`AZURE_EMBEDDING_MODELS`](embedding.md#AZURE_EMBEDDING_MODELS), [`OPENAI_EMBEDDING_MODELS`](embedding.md#OPENAI_EMBEDDING_MODELS), [`logger`](embedding.md#logger)
- used by: [`_is_novel`](database.md#ProgramDatabase._is_novel), [`feature_bins_per_dim`](database.md#ProgramDatabase.feature_bins_per_dim), [`embedding_client`](database.md#ProgramDatabase.embedding_client)

## Module values
- `AZURE_EMBEDDING_MODELS` — [`L20`](../../../../../raw/code/openevolve/openevolve/embedding.py#L20)
- `M` — [`L13`](../../../../../raw/code/openevolve/openevolve/embedding.py#L13)
- `OPENAI_EMBEDDING_COSTS` — [`L25`](../../../../../raw/code/openevolve/openevolve/embedding.py#L25)
- `OPENAI_EMBEDDING_MODELS` — [`L15`](../../../../../raw/code/openevolve/openevolve/embedding.py#L15)
- `logger` — [`L11`](../../../../../raw/code/openevolve/openevolve/embedding.py#L11)

