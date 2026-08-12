---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.utils.code_parsing`/
symbols:
  parse_json_output: parse_json_output().
  extract_code: extract_code().
  log: log.
  is_valid_python_script: is_valid_python_script().
  format_code: format_code().
  parse_json_output._remove_trailing_commas: parse_json_output()._remove_trailing_commas().
  parse_json_output._strip_think_blocks: parse_json_output()._strip_think_blocks().
  parse_json_output._scan_first_json_object: parse_json_output()._scan_first_json_object().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py)

## Functions
- `_remove_trailing_commas(text: str)` — [`L92`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py#L92)
- `_scan_first_json_object(text: str)` — [`L98`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py#L98)
- `_strip_think_blocks(text: str)` — [`L95`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py#L95)
- `extract_code(text: str)` — [`L54`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py#L54) — Extract Python code blocks from the given text.
- `format_code(code: str)` — [`L38`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py#L38) — Format Python code using Black.
- `is_valid_python_script(script: str)` — [`L21`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py#L21) — Check if the provided script is syntactically valid Python code.
- `parse_json_output(response_text)` — [`L87`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py#L87) — Attempts to extract and parse JSON from a string that might be wrapped in markdown/code blocks,

## Module values
- `log` — [`L18`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/utils/code_parsing.py#L18)

