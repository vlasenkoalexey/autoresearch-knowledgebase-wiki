---
title: 'Module: openevolve/utils/code_utils.py'
type: catalog
provenance: extracted
module: openevolve/utils/code_utils.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `openevolve.utils.code_utils`/
symbols:
  format_diff_summary: format_diff_summary().
  apply_diff: apply_diff().
  extract_diffs: extract_diffs().
  _format_block_lines: _format_block_lines().
  split_diffs_by_target: split_diffs_by_target().
  apply_diff_blocks: apply_diff_blocks().
  parse_full_rewrite: parse_full_rewrite().
  extract_code_language: extract_code_language().
  calculate_edit_distance: calculate_edit_distance().
  _can_apply_linewise: _can_apply_linewise().
  parse_evolve_blocks: parse_evolve_blocks().
---
# Module: [`openevolve/utils/code_utils.py`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py)

## Functions
- `_can_apply_linewise(haystack_lines: List[str], needle_lines: List[str])` — [`L232`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L232)
- `_format_block_lines(lines: List[str], max_line_len: int = 100, max_lines: int = 30)` — [`L123`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L123) — Format a block of lines for diff summary: show all lines (truncated per line, optional cap). — documented in [openevolve-utils-code_utils](../../../concepts/openevolve-utils-code_utils.md)
- `apply_diff(original_code: str, diff_text: str, diff_pattern: str = r"<<<<<<< SEARCH\n(.*?)=======\n(.*?)>>>>>>> REPLACE")` — [`L40`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L40) — Apply a diff to the original code — documented in [openevolve-utils-code_utils](../../../concepts/openevolve-utils-code_utils.md)
- `apply_diff_blocks(original_text: str, diff_blocks: List[Tuple[str, str]])` — [`L243`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L243) — Apply diff blocks line-wise and return (new_text, applied_count)
- `calculate_edit_distance(code1: str, code2: str)` — [`L169`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L169) — Calculate the Levenshtein edit distance between two code snippets
- `extract_code_language(code: str)` — [`L205`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L205) — Try to determine the language of a code snippet
- `extract_diffs(diff_text: str, diff_pattern: str = r"<<<<<<< SEARCH\n(.*?)=======\n(.*?)>>>>>>> REPLACE")` — [`L78`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L78) — Extract diff blocks from the diff text — documented in [openevolve-utils-code_utils](../../../concepts/openevolve-utils-code_utils.md)
- `format_diff_summary(diff_blocks: List[Tuple[str, str]], max_line_len: int = 100, max_lines: int = 30)` — [`L136`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L136) — Create a human-readable summary of the diff. — documented in [openevolve-utils-code_utils](../../../concepts/openevolve-utils-code_utils.md)
- `parse_evolve_blocks(code: str)` — [`L9`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L9) — Parse evolve blocks from code
- `parse_full_rewrite(llm_response: str, language: str = "python")` — [`L95`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L95) — Extract a full rewrite from an LLM response
- `split_diffs_by_target(diff_blocks: List[Tuple[str, str]], *, code_text: str, changes_description_text: str)` — [`L263`](../../../../../../raw/code/openevolve/openevolve/utils/code_utils.py#L263) — Route diff blocks to either code or changes_description based on exact line-wise match

