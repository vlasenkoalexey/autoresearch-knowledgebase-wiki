---
title: 'Module: ai_scientist/perform_writeup.py'
type: catalog
provenance: extracted
module: ai_scientist/perform_writeup.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.perform_writeup`/
symbols:
  perform_writeup: perform_writeup().
  parser: parser.
  get_citation_addition: get_citation_addition().
  args: args.
  success: success.
  compile_latex: compile_latex().
  remove_accents_and_clean: remove_accents_and_clean().
  detect_pages_before_impact: detect_pages_before_impact().
  writeup_system_message_template: writeup_system_message_template.
  writeup_prompt: writeup_prompt.
---
# Module: [`ai_scientist/perform_writeup.py`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py)

## Functions
- `compile_latex(cwd, pdf_file, timeout=30)` — [`L39`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L39)
- `detect_pages_before_impact(latex_folder, timeout=30)` — [`L82`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L82) — Temporarily copy the latex folder, compile, and detect on which page
- `get_citation_addition(client, model, context, current_round, total_rounds, idea_text)` — [`L149`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L149) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `perform_writeup(base_folder, no_writing=False, num_cite_rounds=20, small_model="gpt-4o-2024-05-13", big_model="o1-2024-12-17", n_writeup_reflections=3, page_limit=8)` — [`L455`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L455) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `remove_accents_and_clean(s)` — [`L25`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L25)

## Module values
- `args` — [`L794`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L794)
- `parser` — [`L764`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L764)
- `success` — [`L797`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L797)
- `writeup_prompt` — [`L410`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L410)
- `writeup_system_message_template` — [`L345`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_writeup.py#L345)

