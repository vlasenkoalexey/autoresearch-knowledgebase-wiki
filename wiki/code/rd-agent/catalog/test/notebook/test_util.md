---
title: 'Module: test/notebook/test_util.py'
type: catalog
provenance: extracted
module: test/notebook/test_util.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.notebook.test_util`/
symbols:
  S: S().
  TestExtractFunctionBody.test_happy_path: TestExtractFunctionBody#test_happy_path().
  TestExtractFunctionBody.test_happy_path_complex: TestExtractFunctionBody#test_happy_path_complex().
  TestExtractFunctionBody.test_missing_func: TestExtractFunctionBody#test_missing_func().
  TestSplitCodeSections.test_happy_path: TestSplitCodeSections#test_happy_path().
  TestSplitCodeSections.test_happy_path_no_header: TestSplitCodeSections#test_happy_path_no_header().
  TestSplitCodeSections.test_wrong_format: TestSplitCodeSections#test_wrong_format().
  TestSplitCodeSections.test_no_sections: TestSplitCodeSections#test_no_sections().
  TestSplitCodeSections.test_ignores_indented_calls: TestSplitCodeSections#test_ignores_indented_calls().
  TestSplitOutputSections.test_happy_path: TestSplitOutputSections#test_happy_path().
  TestSplitOutputSections.test_happy_path_no_header: TestSplitOutputSections#test_happy_path_no_header().
  TestSplitOutputSections.test_wrong_format: TestSplitOutputSections#test_wrong_format().
  TestSplitOutputSections.test_no_sections: TestSplitOutputSections#test_no_sections().
  TestSplitOutputSections.test_ignore_spaces: TestSplitOutputSections#test_ignore_spaces().
  TestSplitOutputSections.test_ignore_unknown_section: TestSplitOutputSections#test_ignore_unknown_section().
  TestExtractSectionComments.test_happy_path: TestExtractSectionComments#test_happy_path().
  TestExtractSectionComments.test_happy_path_multiline: TestExtractSectionComments#test_happy_path_multiline().
  TestExtractSectionComments.test_no_comment: TestExtractSectionComments#test_no_comment().
  TestExtractSectionComments.test_arbitrary_print_happy_path: TestExtractSectionComments#test_arbitrary_print_happy_path().
  TestExtractFirstSectionNameFromCode.test_happy_path: TestExtractFirstSectionNameFromCode#test_happy_path().
  TestExtractFirstSectionNameFromCode.test_no_section: TestExtractFirstSectionNameFromCode#test_no_section().
  TestExtractFirstSectionNameFromOutput.test_happy_path: TestExtractFirstSectionNameFromOutput#test_happy_path().
  TestExtractFirstSectionNameFromOutput.test_no_section: TestExtractFirstSectionNameFromOutput#test_no_section().
  TestIsFunctionCalled.test_happy_path: TestIsFunctionCalled#test_happy_path().
  TestIsFunctionCalled.test_happy_path_with_args: TestIsFunctionCalled#test_happy_path_with_args().
  TestIsFunctionCalled.test_happy_path_with_args_multiline: TestIsFunctionCalled#test_happy_path_with_args_multiline().
  TestIsFunctionCalled.test_not_called: TestIsFunctionCalled#test_not_called().
  TestIsFunctionCalled.test_wrong_format: TestIsFunctionCalled#test_wrong_format().
  TestRemoveFunction.test_happy_path: TestRemoveFunction#test_happy_path().
  TestRemoveFunction.test_function_does_not_exist: TestRemoveFunction#test_function_does_not_exist().
  TestRemoveFunction.test_preserves_comments: TestRemoveFunction#test_preserves_comments().
  TestRemoveMainBlock.test_happy_path: TestRemoveMainBlock#test_happy_path().
  TestRemoveMainBlock.test_one_liner: TestRemoveMainBlock#test_one_liner().
  TestRemoveMainBlock.test_happy_path_arbitrary_content: TestRemoveMainBlock#test_happy_path_arbitrary_content().
  TestRemoveMainBlock.test_block_does_not_exist: TestRemoveMainBlock#test_block_does_not_exist().
  TestExtractTopLevelFunctions.test_happy_path: TestExtractTopLevelFunctions#test_happy_path().
  TestExtractTopLevelFunctions.test_stop_at_code: TestExtractTopLevelFunctions#test_stop_at_code().
  TestExtractTopLevelFunctions.test_trailing_comment: TestExtractTopLevelFunctions#test_trailing_comment().
  TestSplitCodeAndOutputIntoSections.test_happy_path: TestSplitCodeAndOutputIntoSections#test_happy_path().
  TestSplitCodeAndOutputIntoSections.test_empty_code: TestSplitCodeAndOutputIntoSections#test_empty_code().
  TestSplitCodeAndOutputIntoSections.test_empty_outputs: TestSplitCodeAndOutputIntoSections#test_empty_outputs().
  TestSplitCodeAndOutputIntoSections.test_ignored_sections: TestSplitCodeAndOutputIntoSections#test_ignored_sections().
  TestSplitCodeAndOutputIntoSections.test_complex: TestSplitCodeAndOutputIntoSections#test_complex().
  TestExtractFunctionBody.test_empty: TestExtractFunctionBody#test_empty().
  TestSplitCodeSections.test_empty: TestSplitCodeSections#test_empty().
  TestSplitCodeSections.test_single_no_sections: TestSplitCodeSections#test_single_no_sections().
  TestSplitCodeSections.test_single_with_section: TestSplitCodeSections#test_single_with_section().
  TestSplitOutputSections.test_empty: TestSplitOutputSections#test_empty().
  TestSplitOutputSections.test_single_no_sections: TestSplitOutputSections#test_single_no_sections().
  TestSplitOutputSections.test_single_with_section: TestSplitOutputSections#test_single_with_section().
  TestExtractSectionComments.test_empty_string: TestExtractSectionComments#test_empty_string().
  TestExtractFirstSectionNameFromCode.test_empty_string: TestExtractFirstSectionNameFromCode#test_empty_string().
  TestExtractFirstSectionNameFromOutput.test_empty_string: TestExtractFirstSectionNameFromOutput#test_empty_string().
  TestIsFunctionCalled.test_empty_string: TestIsFunctionCalled#test_empty_string().
  TestRemoveFunction.test_empty: TestRemoveFunction#test_empty().
  TestRemoveMainBlock.test_empty: TestRemoveMainBlock#test_empty().
  TestExtractTopLevelFunctions.test_empty: TestExtractTopLevelFunctions#test_empty().
  test_files_dir: test_files_dir.
  TestExtractFunctionBody: TestExtractFunctionBody#
  TestSplitCodeSections: TestSplitCodeSections#
  TestSplitOutputSections: TestSplitOutputSections#
  TestExtractSectionComments: TestExtractSectionComments#
  TestExtractFirstSectionNameFromCode: TestExtractFirstSectionNameFromCode#
  TestExtractFirstSectionNameFromOutput: TestExtractFirstSectionNameFromOutput#
  TestIsFunctionCalled: TestIsFunctionCalled#
  TestRemoveFunction: TestRemoveFunction#
  TestRemoveMainBlock: TestRemoveMainBlock#
  TestExtractTopLevelFunctions: TestExtractTopLevelFunctions#
  TestSplitCodeAndOutputIntoSections: TestSplitCodeAndOutputIntoSections#
---
# Module: [`test/notebook/test_util.py`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py)

## Classes
### `TestExtractFirstSectionNameFromCode`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:627`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L627)
- signature: `class TestExtractFirstSectionNameFromCode(unittest.TestCase):`
- members:
  - `test_empty_string(self)` — [`L653`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L653)
  - `test_happy_path(self)` — [`L628`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L628)
  - `test_no_section(self)` — [`L642`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L642)
- uses (calls/refs, reference-scoped): [`extract_first_section_name_from_code`](../../rdagent/components/coder/data_science/share/util.md#extract_first_section_name_from_code)  (1 test-only)

### `TestExtractFirstSectionNameFromOutput`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:659`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L659)
- signature: `class TestExtractFirstSectionNameFromOutput(unittest.TestCase):`
- members:
  - `test_empty_string(self)` — [`L684`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L684)
  - `test_happy_path(self)` — [`L660`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L660)
  - `test_no_section(self)` — [`L673`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L673)
- uses (calls/refs, reference-scoped): [`extract_first_section_name_from_output`](../../rdagent/components/coder/data_science/share/util.md#extract_first_section_name_from_output)  (1 test-only)

### `TestExtractFunctionBody`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:21`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L21)
- signature: `class TestExtractFunctionBody(unittest.TestCase):`
- members:
  - `test_empty(self)` — [`L78`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L78)
  - `test_happy_path(self)` — [`L22`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L22)
  - `test_happy_path_complex(self)` — [`L42`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L42)
  - `test_missing_func(self)` — [`L83`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L83)
- uses (calls/refs, reference-scoped): [`extract_function_body`](../../rdagent/components/coder/data_science/share/util.md#extract_function_body)  (1 test-only)

### `TestExtractSectionComments`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:521`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L521)
- signature: `class TestExtractSectionComments(unittest.TestCase):`
- members:
  - `test_arbitrary_print_happy_path(self)` — [`L600`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L600)
  - `test_empty_string(self)` — [`L620`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L620)
  - `test_happy_path(self)` — [`L522`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L522)
  - `test_happy_path_multiline(self)` — [`L548`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L548)
  - `test_no_comment(self)` — [`L575`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L575)
- uses (calls/refs, reference-scoped): [`extract_comment_under_first_print`](../../rdagent/components/coder/data_science/share/util.md#extract_comment_under_first_print)  (1 test-only)

### `TestExtractTopLevelFunctions`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:843`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L843)
- signature: `class TestExtractTopLevelFunctions(unittest.TestCase):`
- members:
  - `test_empty(self)` — [`L889`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L889)
  - `test_happy_path(self)` — [`L844`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L844)
  - `test_stop_at_code(self)` — [`L894`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L894)
  - `test_trailing_comment(self)` — [`L937`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L937)
- uses (calls/refs, reference-scoped): [`extract_top_level_functions_with_decorators_and_comments`](../../rdagent/components/coder/data_science/share/util.md#extract_top_level_functions_with_decorators_and_comments)  (1 test-only)

### `TestIsFunctionCalled`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:690`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L690)
- signature: `class TestIsFunctionCalled(unittest.TestCase):`
- members:
  - `test_empty_string(self)` — [`L728`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L728)
  - `test_happy_path(self)` — [`L691`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L691)
  - `test_happy_path_with_args(self)` — [`L695`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L695)
  - `test_happy_path_with_args_multiline(self)` — [`L703`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L703)
  - `test_not_called(self)` — [`L714`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L714)
  - `test_wrong_format(self)` — [`L724`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L724)
- uses (calls/refs, reference-scoped): [`is_function_called`](../../rdagent/components/coder/data_science/share/util.md#is_function_called)  (1 test-only)

### `TestRemoveFunction`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:733`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L733)
- signature: `class TestRemoveFunction(unittest.TestCase):`
- members:
  - `test_empty(self)` — [`L746`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L746)
  - `test_function_does_not_exist(self)` — [`L740`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L740)
  - `test_happy_path(self)` — [`L734`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L734)
  - `test_preserves_comments(self)` — [`L752`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L752)
- uses (calls/refs, reference-scoped): [`remove_function`](../../rdagent/components/coder/data_science/share/util.md#remove_function)  (1 test-only)

### `TestRemoveMainBlock`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:785`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L785)
- signature: `class TestRemoveMainBlock(unittest.TestCase):`
- members:
  - `test_block_does_not_exist(self)` — [`L820`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L820)
  - `test_empty(self)` — [`L836`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L836)
  - `test_happy_path(self)` — [`L786`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L786)
  - `test_happy_path_arbitrary_content(self)` — [`L807`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L807)
  - `test_one_liner(self)` — [`L797`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L797)
- uses (calls/refs, reference-scoped): [`remove_main_block`](../../rdagent/components/coder/data_science/share/util.md#remove_main_block)  (1 test-only)

### `TestSplitCodeAndOutputIntoSections`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:983`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L983)
- signature: `class TestSplitCodeAndOutputIntoSections(unittest.TestCase):`
- members:
  - `test_complex(self)` — [`L1347`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L1347)
  - `test_empty_code(self)` — [`L1087`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L1087)
  - `test_empty_outputs(self)` — [`L1142`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L1142)
  - `test_happy_path(self)` — [`L984`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L984)
  - `test_ignored_sections(self)` — [`L1227`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L1227)
- uses (calls/refs, reference-scoped): [`split_code_and_output_into_sections`](../../rdagent/components/coder/data_science/share/util.md#split_code_and_output_into_sections)  (2 test-only)

### `TestSplitCodeSections`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:98`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L98)
- signature: `class TestSplitCodeSections(unittest.TestCase):`
- members:
  - `test_empty(self)` — [`L219`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L219)
  - `test_happy_path(self)` — [`L99`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L99)
  - `test_happy_path_no_header(self)` — [`L143`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L143)
  - `test_ignores_indented_calls(self)` — [`L268`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L268)
  - `test_no_sections(self)` — [`L240`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L240)
  - `test_single_no_sections(self)` — [`L226`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L226)
  - `test_single_with_section(self)` — [`L233`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L233)
  - `test_wrong_format(self)` — [`L187`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L187)
- uses (calls/refs, reference-scoped): [`split_code_sections`](../../rdagent/components/coder/data_science/share/util.md#split_code_sections)  (1 test-only)

### `TestSplitOutputSections`  ·  implements/extends TestCase
- def: [`test/notebook/test_util.py:323`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L323)
- signature: `class TestSplitOutputSections(unittest.TestCase):`
- members:
  - `test_empty(self)` — [`L413`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L413)
  - `test_happy_path(self)` — [`L324`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L324)
  - `test_happy_path_no_header(self)` — [`L356`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L356)
  - `test_ignore_spaces(self)` — [`L452`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L452)
  - `test_ignore_unknown_section(self)` — [`L477`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L477)
  - `test_no_sections(self)` — [`L431`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L431)
  - `test_single_no_sections(self)` — [`L419`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L419)
  - `test_single_with_section(self)` — [`L425`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L425)
  - `test_wrong_format(self)` — [`L388`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L388)
- uses (calls/refs, reference-scoped): [`split_output_sections`](../../rdagent/components/coder/data_science/share/util.md#split_output_sections)  (1 test-only)

## Functions
- `S(s_arr)` — [`L1916`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L1916)

## Module values
- `test_files_dir` — [`L18`](../../../../../../raw/code/rd-agent/test/notebook/test_util.py#L18)

