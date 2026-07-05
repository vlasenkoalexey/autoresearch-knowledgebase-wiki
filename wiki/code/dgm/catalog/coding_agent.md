---
title: 'Module: coding_agent.py'
type: catalog
provenance: extracted
module: coding_agent.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 coding_agent/
symbols:
  AgenticSystem.run_regression_tests: AgenticSystem#run_regression_tests().
  AgenticSystem.forward: AgenticSystem#forward().
  AgenticSystem.get_regression_tests: AgenticSystem#get_regression_tests().
  AgenticSystem.get_current_edits: AgenticSystem#get_current_edits().
  main: main().
  AgenticSystem.git_tempdir: AgenticSystem#git_tempdir.
  AgenticSystem.code_model: AgenticSystem#code_model.
  safe_log: safe_log().
  get_thread_logger: get_thread_logger().
  set_thread_logger: set_thread_logger().
  setup_logger: setup_logger().
  AgenticSystem.problem_statement: AgenticSystem#problem_statement.
  AgenticSystem.test_description: AgenticSystem#test_description.
  AgenticSystem.logger: AgenticSystem#logger.
  thread_local: thread_local.
  AgenticSystem: AgenticSystem#
  AgenticSystem.base_commit: AgenticSystem#base_commit.
  AgenticSystem.instance_id: AgenticSystem#instance_id.
  AgenticSystem.__init__: AgenticSystem#__init__().
  AgenticSystem.chat_history_file: AgenticSystem#chat_history_file.
  AgenticSystem.self_improve: AgenticSystem#self_improve.
---
# Module: [`coding_agent.py`](../../../../raw/code/dgm/coding_agent.py)

## Classes
### `AgenticSystem`
- def: [`coding_agent.py:67`](../../../../raw/code/dgm/coding_agent.py#L67)
- signature: `class AgenticSystem:`
- members:
  - `forward(self)` — [`L153`](../../../../raw/code/dgm/coding_agent.py#L153) — The forward function for the AgenticSystem. — documented in [coding_agent](../concepts/coding_agent.md)
  - `get_current_edits(self)` — [`L94`](../../../../raw/code/dgm/coding_agent.py#L94) — documented in [coding_agent](../concepts/coding_agent.md)
  - `get_regression_tests(self)` — [`L98`](../../../../raw/code/dgm/coding_agent.py#L98) — Get the regression tests from the repository. — documented in [coding_agent](../concepts/coding_agent.md)
  - `run_regression_tests(self, regression_tests_summary)` — [`L124`](../../../../raw/code/dgm/coding_agent.py#L124) — Run the regression tests and get the test report. — documented in [coding_agent](../concepts/coding_agent.md)
  - `base_commit` — [`L80`](../../../../raw/code/dgm/coding_agent.py#L80) — documented in [coding_agent](../concepts/coding_agent.md)
  - `chat_history_file` — [`L81`](../../../../raw/code/dgm/coding_agent.py#L81)
  - `code_model` — [`L85`](../../../../raw/code/dgm/coding_agent.py#L85) — documented in [coding_agent](../concepts/coding_agent.md)
  - `git_tempdir` — [`L79`](../../../../raw/code/dgm/coding_agent.py#L79) — documented in [coding_agent](../concepts/coding_agent.md)
  - `instance_id` — [`L84`](../../../../raw/code/dgm/coding_agent.py#L84) — documented in [coding_agent](../concepts/coding_agent.md)
  - `logger` — [`L88`](../../../../raw/code/dgm/coding_agent.py#L88)
  - `problem_statement` — [`L78`](../../../../raw/code/dgm/coding_agent.py#L78) — documented in [coding_agent](../concepts/coding_agent.md)
  - `self_improve` — [`L83`](../../../../raw/code/dgm/coding_agent.py#L83)
  - `test_description` — [`L82`](../../../../raw/code/dgm/coding_agent.py#L82) — documented in [coding_agent](../concepts/coding_agent.md)
- protocol/private: `__init__`[`L68`](../../../../raw/code/dgm/coding_agent.py#L68)
- uses (calls/refs, reference-scoped): [`chat_with_agent`](llm_withtools.md#chat_with_agent), [`diff_versus_commit`](utils/git_utils.md#diff_versus_commit), [`msg_history_to_report`](utils/eval_utils.md#msg_history_to_report), [`safe_log`](coding_agent.md#safe_log), [`CLAUDE_MODEL`](llm_withtools.md#CLAUDE_MODEL), [`setup_logger`](coding_agent.md#setup_logger)
- used by: [`main`](coding_agent.md#main)

## Functions
- `get_thread_logger()` — [`L16`](../../../../raw/code/dgm/coding_agent.py#L16) — Get the logger instance specific to the current thread. — documented in [coding_agent](../concepts/coding_agent.md)
- `main()` — [`L171`](../../../../raw/code/dgm/coding_agent.py#L171) — documented in [coding_agent](../concepts/coding_agent.md)
- `safe_log(message, level=logging.INFO)` — [`L57`](../../../../raw/code/dgm/coding_agent.py#L57) — Thread-safe logging function that ensures messages go to the correct logger. — documented in [coding_agent](../concepts/coding_agent.md)
- `set_thread_logger(logger)` — [`L23`](../../../../raw/code/dgm/coding_agent.py#L23) — Set the logger instance for the current thread.
- `setup_logger(log_file='./chat_history.md', level=logging.INFO)` — [`L29`](../../../../raw/code/dgm/coding_agent.py#L29) — Set up a logger with both file and console handlers.

## Module values
- `thread_local` — [`L14`](../../../../raw/code/dgm/coding_agent.py#L14) — documented in [coding_agent](../concepts/coding_agent.md)

