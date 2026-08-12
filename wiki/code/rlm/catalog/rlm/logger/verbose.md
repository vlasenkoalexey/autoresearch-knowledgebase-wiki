---
title: 'Module: rlm/logger/verbose.py'
type: catalog
provenance: extracted
module: rlm/logger/verbose.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.logger.verbose`/
symbols:
  VerbosePrinter.print_iteration: VerbosePrinter#print_iteration().
  VerbosePrinter.print_code_execution: VerbosePrinter#print_code_execution().
  COLORS: COLORS.
  STYLE_MUTED: STYLE_MUTED.
  VerbosePrinter.console: VerbosePrinter#console.
  VerbosePrinter.print_metadata: VerbosePrinter#print_metadata().
  VerbosePrinter.print_subcall: VerbosePrinter#print_subcall().
  VerbosePrinter.print_header: VerbosePrinter#print_header().
  VerbosePrinter.print_completion: VerbosePrinter#print_completion().
  VerbosePrinter.print_final_answer: VerbosePrinter#print_final_answer().
  VerbosePrinter.print_compaction_status: VerbosePrinter#print_compaction_status().
  VerbosePrinter.print_compaction: VerbosePrinter#print_compaction().
  VerbosePrinter.print_summary: VerbosePrinter#print_summary().
  VerbosePrinter.print_limit_exceeded: VerbosePrinter#print_limit_exceeded().
  VerbosePrinter.print_iteration_start: VerbosePrinter#print_iteration_start().
  VerbosePrinter.print_budget_exceeded: VerbosePrinter#print_budget_exceeded().
  VerbosePrinter.enabled: VerbosePrinter#enabled.
  STYLE_SECONDARY: STYLE_SECONDARY.
  STYLE_TEXT: STYLE_TEXT.
  _to_str: _to_str().
  STYLE_WARNING: STYLE_WARNING.
  STYLE_ACCENT: STYLE_ACCENT.
  STYLE_ERROR: STYLE_ERROR.
  VerbosePrinter: VerbosePrinter#
  STYLE_PRIMARY: STYLE_PRIMARY.
  STYLE_SUCCESS: STYLE_SUCCESS.
  VerbosePrinter._iteration_count: VerbosePrinter#_iteration_count.
  VerbosePrinter.__init__: VerbosePrinter#__init__().
---
# Module: [`rlm/logger/verbose.py`](../../../../../../raw/code/rlm/rlm/logger/verbose.py)

## Classes
### `VerbosePrinter`
- def: [`rlm/logger/verbose.py:55`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L55)
- doc: Rich console printer for RLM verbose output.
- signature: `class VerbosePrinter:`
- members:
  - `__init__(self, enabled: bool = True)` — [`L66`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L66) — Initialize the verbose printer.
  - `print_budget_exceeded(self, spent: float, budget: float)` — [`L366`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L366) — Print a budget exceeded warning.
  - `print_code_execution(self, code_block: CodeBlock)` — [`L211`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L211) — Print code execution details. — documented in [rlm-core-types](../../../concepts/rlm-core-types.md)
  - `print_compaction(self)` — [`L447`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L447) — Print that context compaction (summarization) is running.
  - `print_compaction_status(self, current_tokens: int, threshold_tokens: int, max_tokens: int)` — [`L426`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L426) — Print how close root context is to compaction threshold (before next turn).
  - `print_completion(self, response: Any, iteration_time: float | None = None)` — [`L182`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L182) — Print a completion response.
  - `print_final_answer(self, answer: Any)` — [`L469`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L469) — Print the final answer.
  - `print_header(self, backend: str, model: str, environment: str, max_iterations: int, max_depth: int, other_backends: list[str] | None = None)` — [`L77`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L77) — Print the initial RLM configuration header.
  - `print_iteration(self, iteration: RLMIteration, iteration_num: int)` — [`L338`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L338) — Print a complete iteration including response and code executions. — documented in [rlm-logger-verbose](../../../concepts/rlm-logger-verbose.md)
  - `print_iteration_start(self, iteration: int)` — [`L168`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L168) — Print the start of a new iteration.
  - `print_limit_exceeded(self, limit_type: str, details: str)` — [`L393`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L393) — Print a limit exceeded warning (timeout, tokens, errors, cancellation).
  - `print_metadata(self, metadata: RLMMetadata)` — [`L151`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L151) — Print RLM metadata as header.
  - `print_subcall(self, model: str, prompt_preview: str, response_preview: str, execution_time: float | None = None, metadata: dict | None = None)` — [`L265`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L265) — Print a sub-call to another model.
  - `print_summary(self, total_iterations: int, total_time: float, usage_summary: dict[str, Any] | None = None)` — [`L494`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L494) — Print a summary at the end of execution.
  - `console` — [`L74`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L74)
  - `enabled` — [`L73`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L73)
- protocol/private: `_iteration_count`[`L75`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L75)
- uses (calls/refs, reference-scoped): [`stderr`](../core/types.md#REPLResult.stderr), [`stdout`](../core/types.md#REPLResult.stdout), [`response`](../core/types.md#RLMChatCompletion.response), [`rlm_calls`](../core/types.md#REPLResult.rlm_calls), [`RLMIteration`](../core/types.md#RLMIteration), [`metadata`](../core/types.md#RLMChatCompletion.metadata), [`execution_time`](../core/types.md#RLMChatCompletion.execution_time), [`COLORS`](verbose.md#COLORS), [`prompt`](../core/types.md#RLMChatCompletion.prompt), [`root_model`](../core/types.md#RLMChatCompletion.root_model), [`STYLE_MUTED`](verbose.md#STYLE_MUTED), [`code_blocks`](../core/types.md#RLMIteration.code_blocks), [`result`](../core/types.md#CodeBlock.result), [`response`](../core/types.md#RLMIteration.response), [`CodeBlock`](../core/types.md#CodeBlock), [`STYLE_SECONDARY`](verbose.md#STYLE_SECONDARY), [`STYLE_TEXT`](verbose.md#STYLE_TEXT), [`RLMMetadata`](../core/types.md#RLMMetadata), [`_to_str`](verbose.md#_to_str), [`code`](../core/types.md#CodeBlock.code), [`STYLE_ACCENT`](verbose.md#STYLE_ACCENT), [`STYLE_WARNING`](verbose.md#STYLE_WARNING), [`STYLE_ERROR`](verbose.md#STYLE_ERROR), [`execution_time`](../core/types.md#REPLResult.execution_time), [`STYLE_PRIMARY`](verbose.md#STYLE_PRIMARY), [`STYLE_SUCCESS`](verbose.md#STYLE_SUCCESS), [`backend`](../core/types.md#RLMMetadata.backend), [`backend_kwargs`](../core/types.md#RLMMetadata.backend_kwargs), [`environment_type`](../core/types.md#RLMMetadata.environment_type), [`iteration_time`](../core/types.md#RLMIteration.iteration_time), [`max_depth`](../core/types.md#RLMMetadata.max_depth), [`max_iterations`](../core/types.md#RLMMetadata.max_iterations), [`other_backends`](../core/types.md#RLMMetadata.other_backends)
- used by: [`completion`](../core/rlm.md#RLM.completion), [`_persistent_env`](../core/rlm.md#RLM._persistent_env), [`_check_iteration_limits`](../core/rlm.md#RLM._check_iteration_limits), [`_check_timeout`](../core/rlm.md#RLM._check_timeout), [`verbose`](../core/rlm.md#RLM.verbose)  (1 test-only)

## Functions
- `_to_str(value: Any)` — [`L48`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L48) — Convert any value to string safely.

## Module values
- `COLORS` — [`L23`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L23)
- `STYLE_ACCENT` — [`L45`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L45)
- `STYLE_ERROR` — [`L42`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L42)
- `STYLE_MUTED` — [`L44`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L44)
- `STYLE_PRIMARY` — [`L38`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L38)
- `STYLE_SECONDARY` — [`L39`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L39)
- `STYLE_SUCCESS` — [`L40`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L40)
- `STYLE_TEXT` — [`L43`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L43)
- `STYLE_WARNING` — [`L41`](../../../../../../raw/code/rlm/rlm/logger/verbose.py#L41)

