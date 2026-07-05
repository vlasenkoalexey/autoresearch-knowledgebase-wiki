---
title: 'Module: test/oai/test_embedding_and_similarity.py'
type: catalog
provenance: extracted
module: test/oai/test_embedding_and_similarity.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.oai.test_embedding_and_similarity`/TestEmbedding#
symbols:
  TestEmbedding.test_embedding: test_embedding().
  TestEmbedding.test_embedding_list: test_embedding_list().
  TestEmbedding.test_embedding_long_text_truncation: test_embedding_long_text_truncation().
  TestEmbedding.test_embedding_similarity: test_embedding_similarity().
  TestEmbedding: ''
---
# Module: [`test/oai/test_embedding_and_similarity.py`](../../../../../../raw/code/rd-agent/test/oai/test_embedding_and_similarity.py)

## Classes
### `TestEmbedding`  ·  implements/extends TestCase
- def: [`test/oai/test_embedding_and_similarity.py:9`](../../../../../../raw/code/rd-agent/test/oai/test_embedding_and_similarity.py#L9)
- signature: `class TestEmbedding(unittest.TestCase):`
- members:
  - `test_embedding(self)` — [`L10`](../../../../../../raw/code/rd-agent/test/oai/test_embedding_and_similarity.py#L10)
  - `test_embedding_list(self)` — [`L16`](../../../../../../raw/code/rd-agent/test/oai/test_embedding_and_similarity.py#L16)
  - `test_embedding_long_text_truncation(self)` — [`L29`](../../../../../../raw/code/rd-agent/test/oai/test_embedding_and_similarity.py#L29) — Test embedding with very long text that exceeds token limits
  - `test_embedding_similarity(self)` — [`L22`](../../../../../../raw/code/rd-agent/test/oai/test_embedding_and_similarity.py#L22)
- uses (calls/refs, reference-scoped): [`APIBackend`](../../rdagent/oai/llm_utils.md#APIBackend), [`create_embedding`](../../rdagent/oai/backend/base.md#APIBackend.create_embedding), [`calculate_embedding_distance_between_str_list`](../../rdagent/oai/llm_utils.md#calculate_embedding_distance_between_str_list)

