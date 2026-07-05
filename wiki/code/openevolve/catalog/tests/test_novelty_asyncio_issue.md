---
title: 'Module: tests/test_novelty_asyncio_issue.py'
type: catalog
provenance: extracted
module: tests/test_novelty_asyncio_issue.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_novelty_asyncio_issue`/
symbols:
  TestNoveltyAsyncioIssue.test_novelty_check_disabled_works_fine: TestNoveltyAsyncioIssue#test_novelty_check_disabled_works_fine().
  TestNoveltyAsyncioIssue.test_novelty_check_from_async_context_works: TestNoveltyAsyncioIssue#test_novelty_check_from_async_context_works().
  TestNoveltyAsyncioIssue.test_novelty_check_from_sync_context_works: TestNoveltyAsyncioIssue#test_novelty_check_from_sync_context_works().
  TestNoveltyAsyncioIssue.setUp: TestNoveltyAsyncioIssue#setUp().
  TestNoveltyAsyncioIssue.db: TestNoveltyAsyncioIssue#db.
  TestNoveltyAsyncioIssue.async_add_programs: TestNoveltyAsyncioIssue#async_add_programs().
  MockLLM: MockLLM#
  MockLLM.generate_with_context: MockLLM#generate_with_context().
  TestNoveltyAsyncioIssue: TestNoveltyAsyncioIssue#
  TestNoveltyAsyncioIssue.mock_embedding_client_class: TestNoveltyAsyncioIssue#mock_embedding_client_class.
---
# Module: [`tests/test_novelty_asyncio_issue.py`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py)

## Classes
### `MockLLM`
- def: [`tests/test_novelty_asyncio_issue.py:17`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L17)
- doc: Mock LLM that implements the async interface
- signature: `class MockLLM:`
- members:
  - `generate_with_context(self, system_message: str, messages: list)` — [`L20`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L20) — Mock async generate method that returns NOVEL
- used by: (1 test-only callers)

### `TestNoveltyAsyncioIssue`  ·  implements/extends TestCase
- def: [`tests/test_novelty_asyncio_issue.py:25`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L25)
- doc: Test for asyncio.run() error in novelty checking (issue #313)
- signature: `class TestNoveltyAsyncioIssue(unittest.TestCase):`
- members:
  - `async_add_programs()` — [`L72`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L72) — Add programs from async context - this simulates controller.run()
  - `setUp(self, mock_embedding_client_class)` — [`L29`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L29) — Set up test database with novelty checking enabled
  - `test_novelty_check_disabled_works_fine(self)` — [`L132`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L132) — Test that when novelty checking is disabled, adding programs
  - `test_novelty_check_from_async_context_works(self)` — [`L45`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L45) — Test that novelty checking works correctly when called from within
  - `test_novelty_check_from_sync_context_works(self)` — [`L97`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L97) — Test that novelty checking also works correctly when called from
  - `db` — [`L42`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L42)
  - `mock_embedding_client_class` — [`L43`](../../../../../raw/code/openevolve/tests/test_novelty_asyncio_issue.py#L43)
- uses (calls/refs, reference-scoped): [`id`](../openevolve/database.md#Program.id), [`add`](../openevolve/database.md#ProgramDatabase.add), [`metrics`](../openevolve/database.md#Program.metrics), [`Program`](../openevolve/database.md#Program), [`programs`](../openevolve/database.md#ProgramDatabase.programs), [`code`](../openevolve/database.md#Program.code), [`Config`](../openevolve/config.md#Config), [`database`](../openevolve/config.md#Config.database), [`ProgramDatabase`](../openevolve/database.md#ProgramDatabase), [`language`](../openevolve/database.md#Program.language), [`parent_id`](../openevolve/database.md#Program.parent_id), [`in_memory`](../openevolve/config.md#DatabaseConfig.in_memory), [`novelty_llm`](../openevolve/config.md#DatabaseConfig.novelty_llm), [`embedding_model`](../openevolve/config.md#DatabaseConfig.embedding_model), [`similarity_threshold`](../openevolve/config.md#DatabaseConfig.similarity_threshold)  (1 test-only)

