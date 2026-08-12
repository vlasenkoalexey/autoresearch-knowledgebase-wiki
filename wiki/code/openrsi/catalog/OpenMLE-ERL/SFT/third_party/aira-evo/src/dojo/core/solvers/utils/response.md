---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.solvers.utils.response`/
symbols:
  wrap_code: wrap_code().
  extract_code: extract_code().
  parse_thinking_tags: parse_thinking_tags().
  extract_jsons: extract_jsons().
  trim_long_string: trim_long_string().
  extract_text_up_to_code: extract_text_up_to_code().
  format_code: format_code().
  is_valid_python_script: is_valid_python_script().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py)

## Functions
- `extract_code(text)` — [`L66`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L66) — Extract python code blocks from the text.
- `extract_jsons(text)` — [`L32`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L32) — Extract all JSON objects from the text. Caveat: This function cannot handle nested JSON objects.
- `extract_text_up_to_code(s)` — [`L88`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L88) — Extract (presumed) natural language text up to the start of the first code block.
- `format_code(code)` — [`L95`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L95) — Format Python code using Black.
- `is_valid_python_script(script)` — [`L23`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L23) — Check if a script is a valid Python script.
- `parse_thinking_tags(text)` — [`L103`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L103) — Extracts the thinking information from text enclosed within <think>...</think> tags.
- `trim_long_string(string, threshold=5100, k=2500)` — [`L52`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L52)
- `wrap_code(code: str, lang="python")` — [`L18`](../../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L18) — Wraps code with three backticks.

