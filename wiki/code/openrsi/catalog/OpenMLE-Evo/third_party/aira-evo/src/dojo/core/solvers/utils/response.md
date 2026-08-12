---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.core.solvers.utils.response`/
symbols:
  sanitize_execution_output_for_prompt: sanitize_execution_output_for_prompt().
  wrap_code: wrap_code().
  extract_code: extract_code().
  prompt_score_sanitization_enabled: prompt_score_sanitization_enabled().
  parse_thinking_tags: parse_thinking_tags().
  sanitize_execution_output_for_prompt.insert_redaction: sanitize_execution_output_for_prompt().insert_redaction().
  _config_get: _config_get().
  extract_jsons: extract_jsons().
  trim_long_string: trim_long_string().
  extract_text_up_to_code: extract_text_up_to_code().
  format_code: format_code().
  OFFICIAL_SCORE_REDACTION: OFFICIAL_SCORE_REDACTION.
  _OFFICIAL_FINAL_SCORE_RE: _OFFICIAL_FINAL_SCORE_RE.
  _OFFICIAL_SCORE_MARKER_RE: _OFFICIAL_SCORE_MARKER_RE.
  _GRADER_MARKDOWN_SCORE_RE: _GRADER_MARKDOWN_SCORE_RE.
  _GRADER_PLAIN_SCORE_RE: _GRADER_PLAIN_SCORE_RE.
  is_valid_python_script: is_valid_python_script().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py)

## Functions
- `_config_get(config, key: str, default=None)` — [`L40`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L40)
- `extract_code(text)` — [`L163`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L163) — Extract python code blocks from the text.
- `extract_jsons(text)` — [`L129`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L129) — Extract all JSON objects from the text. Caveat: This function cannot handle nested JSON objects.
- `extract_text_up_to_code(s)` — [`L187`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L187) — Extract (presumed) natural language text up to the start of the first code block.
- `format_code(code)` — [`L194`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L194) — Format Python code using Black.
- `insert_redaction(newline: str)` — [`L88`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L88)
- `is_valid_python_script(script)` — [`L120`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L120) — Check if a script is a valid Python script.
- `parse_thinking_tags(text)` — [`L202`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L202) — Extracts the thinking information from text enclosed within <think>...</think> tags.
- `prompt_score_sanitization_enabled(cfg)` — [`L48`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L48) — Return whether prompt logs should hide official sandbox scores.
- `sanitize_execution_output_for_prompt(output, *, enabled: bool = True)` — [`L64`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L64) — Remove official sandbox scores from execution output before prompting.
- `trim_long_string(string, threshold=5100, k=2500)` — [`L149`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L149)
- `wrap_code(code: str, lang="python")` — [`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L35) — Wraps code with three backticks.

## Module values
- `OFFICIAL_SCORE_REDACTION` — [`L17`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L17)
- `_GRADER_MARKDOWN_SCORE_RE` — [`L27`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L27)
- `_GRADER_PLAIN_SCORE_RE` — [`L30`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L30)
- `_OFFICIAL_FINAL_SCORE_RE` — [`L21`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L21)
- `_OFFICIAL_SCORE_MARKER_RE` — [`L24`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/core/solvers/utils/response.py#L24)

