---
title: 'Module: ai_scientist/treesearch/utils/response.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/utils/response.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.utils.response`/
symbols:
  wrap_code: wrap_code().
  extract_code: extract_code().
  extract_jsons: extract_jsons().
  extract_text_up_to_code: extract_text_up_to_code().
  trim_long_string: trim_long_string().
  format_code: format_code().
  is_valid_python_script: is_valid_python_script().
---
# Module: [`ai_scientist/treesearch/utils/response.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/response.py)

## Functions
- `extract_code(text)` — [`L55`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/response.py#L55) — Extract python code blocks from the text.
- `extract_jsons(text)` — [`L21`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/response.py#L21) — Extract all JSON objects from the text. Caveat: This function cannot handle nested JSON objects.
- `extract_text_up_to_code(s)` — [`L79`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/response.py#L79) — Extract (presumed) natural language text up to the start of the first code block.
- `format_code(code)` — [`L86`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/response.py#L86) — Format Python code using Black.
- `is_valid_python_script(script)` — [`L12`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/response.py#L12) — Check if a script is a valid Python script.
- `trim_long_string(string, threshold=5100, k=2500)` — [`L41`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/response.py#L41)
- `wrap_code(code: str, lang="python")` — [`L7`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/response.py#L7) — Wraps code with three backticks.

