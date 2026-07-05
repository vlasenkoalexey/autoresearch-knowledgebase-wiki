---
title: 'Module: ai_scientist/perform_icbinb_writeup.py'
type: catalog
provenance: extracted
module: ai_scientist/perform_icbinb_writeup.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.perform_icbinb_writeup`/
symbols:
  perform_writeup: perform_writeup().
  gather_citations: gather_citations().
  parser: parser.
  get_citation_addition: get_citation_addition().
  args: args.
  success: success.
  check_page_limit: check_page_limit().
  get_reflection_page_info: get_reflection_page_info().
  compile_latex: compile_latex().
  clean_lines: clean_lines().
  load_idea_text: load_idea_text().
  load_exp_summaries: load_exp_summaries().
  filter_experiment_summaries: filter_experiment_summaries().
  detect_references_position_clean: detect_references_position_clean().
  extract_page_line_counts: extract_page_line_counts().
  remove_accents_and_clean: remove_accents_and_clean().
  is_header_or_footer: is_header_or_footer().
  writeup_system_message_template: writeup_system_message_template.
  writeup_prompt: writeup_prompt.
---
# Module: [`ai_scientist/perform_icbinb_writeup.py`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py)

## Functions
- `check_page_limit(pdf_file, page_limit=4, timeout=30)` — [`L238`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L238) — Compile the LaTeX project in a temporary folder, then determine where the — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `clean_lines(content)` — [`L111`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L111) — Given raw text content, split it into lines and remove lines that are — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `compile_latex(cwd, pdf_file, timeout=30)` — [`L45`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L45) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `detect_references_position_clean(pdf_file)` — [`L121`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L121) — Locate the first occurrence of the word "References" (or variations like — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `extract_page_line_counts(pdf_file, first_page, last_page)` — [`L186`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L186) — Extract the number of cleaned text lines for each page from first_page to last_page. — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `filter_experiment_summaries(exp_summaries, step_name)` — [`L691`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L691) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `gather_citations(base_folder, num_cite_rounds=20, small_model="gpt-4o-2024-05-13")` — [`L745`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L745) — Gather citations for a paper, with ability to resume from previous progress. — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `get_citation_addition(client, model, context, current_round, total_rounds, idea_text)` — [`L337`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L337) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `get_reflection_page_info(reflection_pdf, page_limit)` — [`L304`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L304) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `is_header_or_footer(line)` — [`L88`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L88) — Returns True if the line is likely a header or footer.
- `load_exp_summaries(base_folder)` — [`L665`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L665) — Load the experiment summaries from the base folder. — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `load_idea_text(base_folder)` — [`L648`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L648) — Load the idea text from the base folder. — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `perform_writeup(base_folder, citations_text=None, no_writing=False, num_cite_rounds=20, small_model="gpt-4o-2024-05-13", big_model="o1-2024-12-17", n_writeup_reflections=3, page_limit=4)` — [`L857`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L857) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `remove_accents_and_clean(s)` — [`L33`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L33)

## Module values
- `args` — [`L1276`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L1276) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `parser` — [`L1246`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L1246) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `success` — [`L1279`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L1279) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `writeup_prompt` — [`L602`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L602) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)
- `writeup_system_message_template` — [`L533`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_icbinb_writeup.py#L533) — documented in [ai_scientist-perform_icbinb_writeup](../../concepts/ai_scientist-perform_icbinb_writeup.md)

