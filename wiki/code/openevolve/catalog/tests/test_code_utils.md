---
title: 'Module: tests/test_code_utils.py'
type: catalog
provenance: extracted
module: tests/test_code_utils.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `tests.test_code_utils`/Test
symbols:
  TestCodeUtils.test_extract_diffs: CodeUtils#test_extract_diffs().
  TestCodeUtils.test_apply_diff: CodeUtils#test_apply_diff().
  TestFormatDiffSummary.test_single_line_changes: FormatDiffSummary#test_single_line_changes().
  TestFormatDiffSummary.test_multi_line_changes_show_actual_content: FormatDiffSummary#test_multi_line_changes_show_actual_content().
  TestFormatDiffSummary.test_multiple_diff_blocks: FormatDiffSummary#test_multiple_diff_blocks().
  TestFormatDiffSummary.test_configurable_max_line_len: FormatDiffSummary#test_configurable_max_line_len().
  TestFormatDiffSummary.test_configurable_max_lines: FormatDiffSummary#test_configurable_max_lines().
  TestFormatDiffSummary.test_block_lines_basic_formatting: FormatDiffSummary#test_block_lines_basic_formatting().
  TestFormatDiffSummary.test_block_lines_long_line_truncation: FormatDiffSummary#test_block_lines_long_line_truncation().
  TestFormatDiffSummary.test_block_lines_many_lines_truncation: FormatDiffSummary#test_block_lines_many_lines_truncation().
  TestFormatDiffSummary.test_block_lines_empty_input: FormatDiffSummary#test_block_lines_empty_input().
  TestCodeUtils: CodeUtils#
  TestFormatDiffSummary: FormatDiffSummary#
---
# Module: [`tests/test_code_utils.py`](../../../../../raw/code/openevolve/tests/test_code_utils.py)

## Classes
### `TestCodeUtils`  ·  implements/extends TestCase
- def: [`tests/test_code_utils.py:15`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L15)
- doc: Tests for code utilities
- signature: `class TestCodeUtils(unittest.TestCase):`
- members:
  - `test_apply_diff(self)` — [`L55`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L55) — Test applying diffs to code — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_extract_diffs(self)` — [`L18`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L18) — Test extracting diffs from a response — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
- uses (calls/refs, reference-scoped): [`apply_diff`](../openevolve/utils/code_utils.md#apply_diff), [`extract_diffs`](../openevolve/utils/code_utils.md#extract_diffs)

### `TestFormatDiffSummary`  ·  implements/extends TestCase
- def: [`tests/test_code_utils.py:98`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L98)
- doc: Tests for format_diff_summary showing actual diff content
- signature: `class TestFormatDiffSummary(unittest.TestCase):`
- members:
  - `test_block_lines_basic_formatting(self)` — [`L159`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L159) — Lines should be indented with 2 spaces — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_block_lines_empty_input(self)` — [`L179`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L179) — Empty input should return '(empty)' — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_block_lines_long_line_truncation(self)` — [`L165`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L165) — Lines over 100 chars should be truncated by default — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_block_lines_many_lines_truncation(self)` — [`L172`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L172) — More than 30 lines should show truncation message by default — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_configurable_max_line_len(self)` — [`L139`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L139) — max_line_len parameter should control line truncation — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_configurable_max_lines(self)` — [`L151`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L151) — max_lines parameter should control block truncation — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_multi_line_changes_show_actual_content(self)` — [`L107`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L107) — Multi-line changes should show actual SEARCH/REPLACE content — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_multiple_diff_blocks(self)` — [`L126`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L126) — Multiple diff blocks should be numbered — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
  - `test_single_line_changes(self)` — [`L101`](../../../../../raw/code/openevolve/tests/test_code_utils.py#L101) — Single-line changes should show inline format — documented in [openevolve-utils-code_utils](../../concepts/openevolve-utils-code_utils.md)
- uses (calls/refs, reference-scoped): [`format_diff_summary`](../openevolve/utils/code_utils.md#format_diff_summary), [`_format_block_lines`](../openevolve/utils/code_utils.md#_format_block_lines)

