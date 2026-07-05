---
title: 'Module: rdagent/components/coder/data_science/share/util.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/share/util.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.share.util`/
symbols:
  split_code_and_output_into_sections: split_code_and_output_into_sections().
  split_output_sections: split_output_sections().
  split_code_sections: split_code_sections().
  extract_top_level_functions_with_decorators_and_comments: extract_top_level_functions_with_decorators_and_comments().
  extract_function_body: extract_function_body().
  is_function_called: is_function_called().
  extract_comment_under_first_print: extract_comment_under_first_print().
  extract_first_section_name_from_code: extract_first_section_name_from_code().
  remove_main_block: remove_main_block().
  remove_function: remove_function().
  extract_first_section_name_from_output: extract_first_section_name_from_output().
  extract_top_level_functions_with_decorators_and_comments._max_lineno: extract_top_level_functions_with_decorators_and_comments()._max_lineno().
  CodeSection: CodeSection#
  CodeSection.name: CodeSection#name.
  CodeSection.code: CodeSection#code.
  CodeSection.comments: CodeSection#comments.
  CodeSection.output: CodeSection#output.
  split_sections: split_sections().
---
# Module: [`rdagent/components/coder/data_science/share/util.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py)

## Classes
### `CodeSection`  ·  implements/extends _TypedDict
- def: [`rdagent/components/coder/data_science/share/util.py:9`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L9)
- doc: Represents a section of the original Python source code, to be converted to a notebook cell.
- signature: `class CodeSection(TypedDict):`
- members:
  - `code` — [`L15`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L15)
  - `comments` — [`L16`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L16)
  - `name` — [`L14`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L14)
  - `output` — [`L17`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L17)
- used by: [`split_code_and_output_into_sections`](util.md#split_code_and_output_into_sections)

## Functions
- `_max_lineno(n)` — [`L283`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L283)
- `extract_comment_under_first_print(source_code)` — [`L94`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L94) — Extract comments from the source code after the first print statement.
- `extract_first_section_name_from_code(source_code)` — [`L133`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L133) — Extract the first section name from the source code.
- `extract_first_section_name_from_output(stdout: str)` — [`L151`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L151) — Extract the first section name from the output string.
- `extract_function_body(source_code: str, function_name: str)` — [`L20`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L20) — Extracts the body of a function from the source code.
- `extract_top_level_functions_with_decorators_and_comments(code: str)` — [`L224`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L224) — Returns list of (function_name, source_segment) for top-level functions (excluding "main"),
- `is_function_called(source_code: str, func_name: str)` — [`L161`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L161) — Returns True if the function named `func_name` is called in `source_code`.
- `remove_function(source_code: str, function_name: str)` — [`L178`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L178) — Remove a function definition from the source code.
- `remove_main_block(source_code: str)` — [`L194`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L194) — Remove the if __name__ == "__main__": block from the source code.
- `split_code_and_output_into_sections(code: str, stdout: str)` — [`L300`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L300) — Converts a Python script and its output into a list of CodeSections.
- `split_code_sections(source_code: str)` — [`L79`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L79) — Split code into sections based on the section headers.
- `split_output_sections(stdout: str, known_sections: list[str])` — [`L86`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L86) — Split output into sections based on the section headers.
- `split_sections(text: str, section_header_regex: str, known_sections: Optional[list[str]] = None)` — [`L39`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/util.py#L39) — Split text into sections based on the section headers.

