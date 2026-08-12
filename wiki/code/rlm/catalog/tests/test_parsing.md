---
title: 'Module: tests/test_parsing.py'
type: catalog
provenance: extracted
module: tests/test_parsing.py
status: fresh
symbol_base: scip-python python rlm 0.0.0 `tests.test_parsing`/Test
symbols:
  TestFormatIteration.test_iteration_with_code_blocks: FormatIteration#test_iteration_with_code_blocks().
  TestFormatIteration.test_truncates_long_results: FormatIteration#test_truncates_long_results().
  TestFormatIteration.test_iteration_without_code_blocks: FormatIteration#test_iteration_without_code_blocks().
  TestAnswerDictFinalAnswer.test_answer_dict_ready_true_sets_final_answer: AnswerDictFinalAnswer#test_answer_dict_ready_true_sets_final_answer().
  TestAnswerDictFinalAnswer.test_answer_dict_unset_keeps_final_answer_none: AnswerDictFinalAnswer#test_answer_dict_unset_keeps_final_answer_none().
  TestAnswerDictFinalAnswer.test_answer_dict_rebind_with_ready: AnswerDictFinalAnswer#test_answer_dict_rebind_with_ready().
  TestAnswerDictFinalAnswer.test_answer_content_can_be_non_string: AnswerDictFinalAnswer#test_answer_content_can_be_non_string().
  TestFormatExecutionResult.test_stdout_only: FormatExecutionResult#test_stdout_only().
  TestFormatExecutionResult.test_stderr_only: FormatExecutionResult#test_stderr_only().
  TestFormatExecutionResult.test_with_locals: FormatExecutionResult#test_with_locals().
  TestFormatExecutionResult.test_excludes_private_vars: FormatExecutionResult#test_excludes_private_vars().
  TestFormatExecutionResult.test_empty_result: FormatExecutionResult#test_empty_result().
  TestFindCodeBlocks.test_single_code_block: FindCodeBlocks#test_single_code_block().
  TestFindCodeBlocks.test_multiple_code_blocks: FindCodeBlocks#test_multiple_code_blocks().
  TestFindCodeBlocks.test_no_code_blocks: FindCodeBlocks#test_no_code_blocks().
  TestFindCodeBlocks.test_non_repl_code_blocks_ignored: FindCodeBlocks#test_non_repl_code_blocks_ignored().
  TestFindCodeBlocks.test_multiline_code_block: FindCodeBlocks#test_multiline_code_block().
  TestConvertContextForRepl.test_string_context: ConvertContextForRepl#test_string_context().
  TestConvertContextForRepl.test_dict_context: ConvertContextForRepl#test_dict_context().
  TestConvertContextForRepl.test_list_of_strings: ConvertContextForRepl#test_list_of_strings().
  TestConvertContextForRepl.test_list_of_message_dicts: ConvertContextForRepl#test_list_of_message_dicts().
  TestFindCodeBlocks: FindCodeBlocks#
  TestAnswerDictFinalAnswer: AnswerDictFinalAnswer#
  TestFormatExecutionResult: FormatExecutionResult#
  TestFormatIteration: FormatIteration#
  TestConvertContextForRepl: ConvertContextForRepl#
---
# Module: [`tests/test_parsing.py`](../../../../../raw/code/rlm/tests/test_parsing.py)

## Classes
### `TestAnswerDictFinalAnswer`
- def: [`tests/test_parsing.py:78`](../../../../../raw/code/rlm/tests/test_parsing.py#L78)
- doc: Tests for the `answer` dict completion signal surfaced via REPLResult.final_answer.
- signature: `class TestAnswerDictFinalAnswer:`
- members:
  - `test_answer_content_can_be_non_string(self)` — [`L108`](../../../../../raw/code/rlm/tests/test_parsing.py#L108) — Any ``str()``-able content (numbers, lists) should be coerced to a string final answer.
  - `test_answer_dict_ready_true_sets_final_answer(self)` — [`L81`](../../../../../raw/code/rlm/tests/test_parsing.py#L81) — Setting ``answer['ready'] = True`` must populate REPLResult.final_answer.
  - `test_answer_dict_rebind_with_ready(self)` — [`L99`](../../../../../raw/code/rlm/tests/test_parsing.py#L99) — Plain-dict rebind with ``ready=True`` must still be captured.
  - `test_answer_dict_unset_keeps_final_answer_none(self)` — [`L90`](../../../../../raw/code/rlm/tests/test_parsing.py#L90) — If ``ready`` stays False, the REPL must not surface a final answer.
- uses (calls/refs, reference-scoped): [`execute_code`](../rlm/environments/local_repl.md#LocalREPL.execute_code), [`LocalREPL`](../rlm/environments/local_repl.md#LocalREPL), [`cleanup`](../rlm/environments/local_repl.md#LocalREPL.cleanup), [`final_answer`](../rlm/core/types.md#REPLResult.final_answer)

### `TestConvertContextForRepl`
- def: [`tests/test_parsing.py:190`](../../../../../raw/code/rlm/tests/test_parsing.py#L190)
- doc: Tests for convert_context_for_repl function.
- signature: `class TestConvertContextForRepl:`
- members:
  - `test_dict_context(self)` — [`L198`](../../../../../raw/code/rlm/tests/test_parsing.py#L198)
  - `test_list_of_message_dicts(self)` — [`L208`](../../../../../raw/code/rlm/tests/test_parsing.py#L208)
  - `test_list_of_strings(self)` — [`L203`](../../../../../raw/code/rlm/tests/test_parsing.py#L203)
  - `test_string_context(self)` — [`L193`](../../../../../raw/code/rlm/tests/test_parsing.py#L193)
- uses (calls/refs, reference-scoped): [`convert_context_for_repl`](../rlm/utils/parsing.md#convert_context_for_repl)

### `TestFindCodeBlocks`
- def: [`tests/test_parsing.py:13`](../../../../../raw/code/rlm/tests/test_parsing.py#L13)
- doc: Tests for find_code_blocks function.
- signature: `class TestFindCodeBlocks:`
- members:
  - `test_multiline_code_block(self)` — [`L62`](../../../../../raw/code/rlm/tests/test_parsing.py#L62)
  - `test_multiple_code_blocks(self)` — [`L28`](../../../../../raw/code/rlm/tests/test_parsing.py#L28)
  - `test_no_code_blocks(self)` — [`L43`](../../../../../raw/code/rlm/tests/test_parsing.py#L43)
  - `test_non_repl_code_blocks_ignored(self)` — [`L48`](../../../../../raw/code/rlm/tests/test_parsing.py#L48)
  - `test_single_code_block(self)` — [`L16`](../../../../../raw/code/rlm/tests/test_parsing.py#L16)
- uses (calls/refs, reference-scoped): [`find_code_blocks`](../rlm/utils/parsing.md#find_code_blocks)

### `TestFormatExecutionResult`
- def: [`tests/test_parsing.py:118`](../../../../../raw/code/rlm/tests/test_parsing.py#L118)
- doc: Tests for format_execution_result function.
- signature: `class TestFormatExecutionResult:`
- members:
  - `test_empty_result(self)` — [`L144`](../../../../../raw/code/rlm/tests/test_parsing.py#L144)
  - `test_excludes_private_vars(self)` — [`L137`](../../../../../raw/code/rlm/tests/test_parsing.py#L137)
  - `test_stderr_only(self)` — [`L126`](../../../../../raw/code/rlm/tests/test_parsing.py#L126)
  - `test_stdout_only(self)` — [`L121`](../../../../../raw/code/rlm/tests/test_parsing.py#L121)
  - `test_with_locals(self)` — [`L131`](../../../../../raw/code/rlm/tests/test_parsing.py#L131)
- uses (calls/refs, reference-scoped): [`REPLResult`](../rlm/core/types.md#REPLResult), [`format_execution_result`](../rlm/utils/parsing.md#format_execution_result)

### `TestFormatIteration`
- def: [`tests/test_parsing.py:150`](../../../../../raw/code/rlm/tests/test_parsing.py#L150)
- doc: Tests for format_iteration function.
- signature: `class TestFormatIteration:`
- members:
  - `test_iteration_with_code_blocks(self)` — [`L153`](../../../../../raw/code/rlm/tests/test_parsing.py#L153)
  - `test_iteration_without_code_blocks(self)` — [`L167`](../../../../../raw/code/rlm/tests/test_parsing.py#L167)
  - `test_truncates_long_results(self)` — [`L177`](../../../../../raw/code/rlm/tests/test_parsing.py#L177)
- uses (calls/refs, reference-scoped): [`REPLResult`](../rlm/core/types.md#REPLResult), [`RLMIteration`](../rlm/core/types.md#RLMIteration), [`code_blocks`](../rlm/core/types.md#RLMIteration.code_blocks), [`format_iteration`](../rlm/utils/parsing.md#format_iteration), [`result`](../rlm/core/types.md#CodeBlock.result), [`response`](../rlm/core/types.md#RLMIteration.response), [`CodeBlock`](../rlm/core/types.md#CodeBlock), [`prompt`](../rlm/core/types.md#RLMIteration.prompt), [`code`](../rlm/core/types.md#CodeBlock.code)

