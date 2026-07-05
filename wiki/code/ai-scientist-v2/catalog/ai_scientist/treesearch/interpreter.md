---
title: 'Module: ai_scientist/treesearch/interpreter.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/interpreter.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.interpreter`/
symbols:
  Interpreter.run: Interpreter#run().
  Interpreter.event_outq: Interpreter#event_outq.
  Interpreter.process: Interpreter#process.
  Interpreter.cleanup_session: Interpreter#cleanup_session().
  Interpreter._run_session: Interpreter#_run_session().
  Interpreter.working_dir: Interpreter#working_dir.
  Interpreter._drain_queues: Interpreter#_drain_queues().
  Interpreter.result_outq: Interpreter#result_outq.
  Interpreter.child_proc_setup: Interpreter#child_proc_setup().
  ExecutionResult: ExecutionResult#
  logger: logger.
  Interpreter.timeout: Interpreter#timeout.
  ExecutionResult.term_out: ExecutionResult#term_out.
  ExecutionResult.exc_type: ExecutionResult#exc_type.
  ExecutionResult.exc_info: ExecutionResult#exc_info.
  Interpreter: Interpreter#
  Interpreter.code_inq: Interpreter#code_inq.
  ExecutionResult.exc_stack: ExecutionResult#exc_stack.
  Interpreter.agent_file_name: Interpreter#agent_file_name.
  RedirectQueue.write: RedirectQueue#write().
  ExecutionResult.exec_time: ExecutionResult#exec_time.
  exception_summary: exception_summary().
  RedirectQueue: RedirectQueue#
  RedirectQueue.queue: RedirectQueue#queue.
  Interpreter.format_tb_ipython: Interpreter#format_tb_ipython.
  Interpreter.env_vars: Interpreter#env_vars.
  Interpreter.create_process: Interpreter#create_process().
  RedirectQueue.__init__: RedirectQueue#__init__().
  RedirectQueue.flush: RedirectQueue#flush().
  Interpreter.__init__: Interpreter#__init__().
---
# Module: [`ai_scientist/treesearch/interpreter.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py)

## Classes
### `ExecutionResult`
- def: [`ai_scientist/treesearch/interpreter.py:27`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L27) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
- doc: Result of executing a code snippet in the interpreter.
- signature: `class ExecutionResult(DataClassJsonMixin):`
- members:
  - `exc_info` — [`L36`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L36)
  - `exc_stack` — [`L37`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L37)
  - `exc_type` — [`L35`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L35)
  - `exec_time` — [`L34`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L34)
  - `term_out` — [`L33`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L33)
- used by: [`_process_node_wrapper`](parallel_agent.md#ParallelAgent._process_node_wrapper), [`parse_exec_result`](parallel_agent.md#MinimalAgent.parse_exec_result), [`absorb_exec_result`](journal.md#Node.absorb_exec_result), [`absorb_plot_exec_result`](journal.md#Node.absorb_plot_exec_result), [`run`](interpreter.md#Interpreter.run), [`ExecCallbackType`](parallel_agent.md#ExecCallbackType)

### `Interpreter`
- def: [`ai_scientist/treesearch/interpreter.py:81`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L81)
- signature: `class Interpreter:`
- members:
  - `__init__(self, working_dir: Path | str, timeout: int = 3600, format_tb_ipython: bool = False, agent_file_name: str = "runfile.py", env_vars: dict[str, str] = {})` — [`L82`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L82) — Simulates a standalone Python REPL with an execution time limit.
  - `_drain_queues(self)` — [`L176`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L176) — Quickly drain all in-flight messages to prevent blocking. — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `child_proc_setup(self, result_outq: Queue)` — [`L111`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L111) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `cleanup_session(self)` — [`L196`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L196) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `create_process(self)` — [`L163`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L163) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `run(self, code: str, reset_session=True)` — [`L213`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L213) — Execute the provided Python command in a separate process and return its output. — documented in [ai_scientist-treesearch-agent_manager](../../../concepts/ai_scientist-treesearch-agent_manager.md)
  - `agent_file_name` — [`L107`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L107) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `code_inq` — [`L169`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L169) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `env_vars` — [`L109`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L109) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `event_outq` — [`L169`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L169) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `format_tb_ipython` — [`L106`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L106) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `process` — [`L108`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L108) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `result_outq` — [`L169`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L169) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `timeout` — [`L105`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L105) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
  - `working_dir` — [`L101`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L101) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
- protocol/private: `_run_session`[`L130`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L130)
- uses (calls/refs, reference-scoped): [`ExecutionResult`](interpreter.md#ExecutionResult), [`logger`](interpreter.md#logger), [`RedirectQueue`](interpreter.md#RedirectQueue), [`exception_summary`](interpreter.md#exception_summary)
- used by: [`_process_node_wrapper`](parallel_agent.md#ParallelAgent._process_node_wrapper), [`_run_plot_aggregation`](parallel_agent.md#ParallelAgent._run_plot_aggregation)

### `RedirectQueue`
- def: [`ai_scientist/treesearch/interpreter.py:70`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L70) — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)
- signature: `class RedirectQueue:`
- members:
  - `flush(self)` — [`L77`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L77)
  - `write(self, msg)` — [`L74`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L74)
  - `queue` — [`L72`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L72)
- protocol/private: `__init__`[`L71`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L71)
- used by: [`child_proc_setup`](interpreter.md#Interpreter.child_proc_setup)

## Functions
- `exception_summary(e, working_dir, exec_file_name, format_tb_ipython)` — [`L40`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L40) — Generates a string that summarizes an exception and its stack trace (either in standard python repl or in IPython format). — documented in [ai_scientist-treesearch-interpreter](../../../concepts/ai_scientist-treesearch-interpreter.md)

## Module values
- `logger` — [`L23`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/interpreter.py#L23)

