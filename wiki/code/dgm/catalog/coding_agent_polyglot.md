---
title: 'Module: coding_agent_polyglot.py'
type: catalog
provenance: extracted
module: coding_agent_polyglot.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 coding_agent_polyglot/
symbols:
  AgenticSystem.forward: AgenticSystem#forward().
  main: main().
  AgenticSystem.get_current_edits: AgenticSystem#get_current_edits().
  AgenticSystem.code_model: AgenticSystem#code_model.
  TEST_COMMANDS: TEST_COMMANDS.
  get_thread_logger: get_thread_logger().
  set_thread_logger: set_thread_logger().
  setup_logger: setup_logger().
  safe_log: safe_log().
  AgenticSystem.git_tempdir: AgenticSystem#git_tempdir.
  AgenticSystem.logger: AgenticSystem#logger.
  thread_local: thread_local.
  NPM_TEST_COMMANDS: NPM_TEST_COMMANDS.
  CPP_TEST_COMMANDS: CPP_TEST_COMMANDS.
  AgenticSystem: AgenticSystem#
  AgenticSystem.problem_statement: AgenticSystem#problem_statement.
  AgenticSystem.base_commit: AgenticSystem#base_commit.
  AgenticSystem.__init__: AgenticSystem#__init__().
  AgenticSystem.chat_history_file: AgenticSystem#chat_history_file.
  AgenticSystem.test_description: AgenticSystem#test_description.
  AgenticSystem.self_improve: AgenticSystem#self_improve.
  AgenticSystem.language: AgenticSystem#language.
---
# Module: [`coding_agent_polyglot.py`](../../../../raw/code/dgm/coding_agent_polyglot.py)

## Classes
### `AgenticSystem`
- def: [`coding_agent_polyglot.py:96`](../../../../raw/code/dgm/coding_agent_polyglot.py#L96)
- signature: `class AgenticSystem:`
- members:
  - `forward(self)` — [`L140`](../../../../raw/code/dgm/coding_agent_polyglot.py#L140) — The forward function for the AgenticSystem. — documented in [llm_withtools](../concepts/llm_withtools.md)
  - `get_current_edits(self)` — [`L125`](../../../../raw/code/dgm/coding_agent_polyglot.py#L125)
  - `base_commit` — [`L109`](../../../../raw/code/dgm/coding_agent_polyglot.py#L109)
  - `chat_history_file` — [`L110`](../../../../raw/code/dgm/coding_agent_polyglot.py#L110)
  - `code_model` — [`L116`](../../../../raw/code/dgm/coding_agent_polyglot.py#L116)
  - `git_tempdir` — [`L108`](../../../../raw/code/dgm/coding_agent_polyglot.py#L108)
  - `language` — [`L113`](../../../../raw/code/dgm/coding_agent_polyglot.py#L113)
  - `logger` — [`L119`](../../../../raw/code/dgm/coding_agent_polyglot.py#L119)
  - `problem_statement` — [`L107`](../../../../raw/code/dgm/coding_agent_polyglot.py#L107)
  - `self_improve` — [`L112`](../../../../raw/code/dgm/coding_agent_polyglot.py#L112)
  - `test_description` — [`L111`](../../../../raw/code/dgm/coding_agent_polyglot.py#L111)
- protocol/private: `__init__`[`L97`](../../../../raw/code/dgm/coding_agent_polyglot.py#L97)
- uses (calls/refs, reference-scoped): [`chat_with_agent`](llm_withtools.md#chat_with_agent), [`diff_versus_commit`](utils/git_utils.md#diff_versus_commit), [`CLAUDE_MODEL`](llm_withtools.md#CLAUDE_MODEL), [`safe_log`](coding_agent_polyglot.md#safe_log), [`setup_logger`](coding_agent_polyglot.md#setup_logger), [`OPENAI_MODEL`](llm_withtools.md#OPENAI_MODEL)
- used by: [`main`](coding_agent_polyglot.md#main)

## Functions
- `get_thread_logger()` — [`L45`](../../../../raw/code/dgm/coding_agent_polyglot.py#L45) — Get the logger instance specific to the current thread.
- `main()` — [`L155`](../../../../raw/code/dgm/coding_agent_polyglot.py#L155)
- `safe_log(message, level=logging.INFO)` — [`L86`](../../../../raw/code/dgm/coding_agent_polyglot.py#L86) — Thread-safe logging function that ensures messages go to the correct logger.
- `set_thread_logger(logger)` — [`L52`](../../../../raw/code/dgm/coding_agent_polyglot.py#L52) — Set the logger instance for the current thread.
- `setup_logger(log_file='./chat_history.md', level=logging.INFO)` — [`L58`](../../../../raw/code/dgm/coding_agent_polyglot.py#L58) — Set up a logger with both file and console handlers.

## Module values
- `CPP_TEST_COMMANDS` — [`L24`](../../../../raw/code/dgm/coding_agent_polyglot.py#L24)
- `NPM_TEST_COMMANDS` — [`L16`](../../../../raw/code/dgm/coding_agent_polyglot.py#L16)
- `TEST_COMMANDS` — [`L33`](../../../../raw/code/dgm/coding_agent_polyglot.py#L33)
- `thread_local` — [`L43`](../../../../raw/code/dgm/coding_agent_polyglot.py#L43)

