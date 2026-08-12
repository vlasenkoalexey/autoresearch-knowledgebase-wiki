---
title: 'Module: rlm/utils/parsing.py'
type: catalog
provenance: extracted
module: rlm/utils/parsing.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `rlm.utils.parsing`/
symbols:
  format_iteration: format_iteration().
  format_execution_result: format_execution_result().
  find_code_blocks: find_code_blocks().
  convert_context_for_repl: convert_context_for_repl().
---
# Module: [`rlm/utils/parsing.py`](../../../../../../raw/code/rlm/rlm/utils/parsing.py)

## Functions
- `convert_context_for_repl(context)` — [`L110`](../../../../../../raw/code/rlm/rlm/utils/parsing.py#L110) — Convert REPL context to either some
- `find_code_blocks(text: str)` — [`L10`](../../../../../../raw/code/rlm/rlm/utils/parsing.py#L10) — Find REPL code blocks in text wrapped in triple backticks and return List of content(s).
- `format_execution_result(result: REPLResult)` — [`L77`](../../../../../../raw/code/rlm/rlm/utils/parsing.py#L77) — Format the execution result as a string for display.
- `format_iteration(iteration: RLMIteration, max_character_length: int = 20000)` — [`L25`](../../../../../../raw/code/rlm/rlm/utils/parsing.py#L25) — Format an RLM iteration (including all code blocks) to append to the message history for — documented in [rlm-core-rlm](../../../concepts/rlm-core-rlm.md)

