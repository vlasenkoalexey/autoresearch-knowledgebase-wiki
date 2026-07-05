---
title: 'Module: test/oai/test_advanced.py'
type: catalog
provenance: extracted
module: test/oai/test_advanced.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.oai.test_advanced`/
symbols:
  TestAdvanced.test_chat_cache_multiprocess: TestAdvanced#test_chat_cache_multiprocess().
  TestAdvanced.test_chat_cache: TestAdvanced#test_chat_cache().
  TestAdvanced.test_chat_multi_round: TestAdvanced#test_chat_multi_round().
  _worker: _worker().
  TestAdvanced: TestAdvanced#
---
# Module: [`test/oai/test_advanced.py`](../../../../../../raw/code/rd-agent/test/oai/test_advanced.py)

## Classes
### `TestAdvanced`  ·  implements/extends TestCase
- def: [`test/oai/test_advanced.py:22`](../../../../../../raw/code/rd-agent/test/oai/test_advanced.py#L22)
- signature: `class TestAdvanced(unittest.TestCase):`
- members:
  - `test_chat_cache(self)` — [`L89`](../../../../../../raw/code/rd-agent/test/oai/test_advanced.py#L89) — Tests:
  - `test_chat_cache_multiprocess(self)` — [`L24`](../../../../../../raw/code/rd-agent/test/oai/test_advanced.py#L24) — Tests:
  - `test_chat_multi_round(self)` — [`L72`](../../../../../../raw/code/rd-agent/test/oai/test_advanced.py#L72)
- uses (calls/refs, reference-scoped): [`APIBackend`](../../rdagent/oai/llm_utils.md#APIBackend), [`LLM_SETTINGS`](../../rdagent/oai/llm_conf.md#LLM_SETTINGS), [`build_messages_and_create_chat_completion`](../../rdagent/oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`build_chat_completion`](../../rdagent/oai/backend/base.md#ChatSession.build_chat_completion), [`multiprocessing_wrapper`](../../rdagent/core/utils.md#multiprocessing_wrapper), [`build_chat_session`](../../rdagent/oai/backend/base.md#APIBackend.build_chat_session), [`LLM_CACHE_SEED_GEN`](../../rdagent/core/utils.md#LLM_CACHE_SEED_GEN), [`dump_chat_cache`](../../rdagent/oai/llm_conf.md#LLMSettings.dump_chat_cache), [`set_seed`](../../rdagent/core/utils.md#CacheSeedGen.set_seed), [`use_chat_cache`](../../rdagent/oai/llm_conf.md#LLMSettings.use_chat_cache), [`use_auto_chat_cache_seed_gen`](../../rdagent/oai/llm_conf.md#LLMSettings.use_auto_chat_cache_seed_gen)  (1 test-only)

## Functions
- `_worker(system_prompt, user_prompt)` — [`L14`](../../../../../../raw/code/rd-agent/test/oai/test_advanced.py#L14)

