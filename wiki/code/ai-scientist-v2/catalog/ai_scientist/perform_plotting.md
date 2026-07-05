---
title: 'Module: ai_scientist/perform_plotting.py'
type: catalog
provenance: extracted
module: ai_scientist/perform_plotting.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.perform_plotting`/
symbols:
  aggregate_plots: aggregate_plots().
  AGGREGATOR_SYSTEM_MSG: AGGREGATOR_SYSTEM_MSG.
  main: main().
  MAX_FIGURES: MAX_FIGURES.
  extract_code_snippet: extract_code_snippet().
  run_aggregator_script: run_aggregator_script().
  build_aggregator_prompt: build_aggregator_prompt().
---
# Module: [`ai_scientist/perform_plotting.py`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_plotting.py)

## Functions
- `aggregate_plots(base_folder: str, model: str = "o1-2024-12-17", n_reflections: int = 5)` — [`L136`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_plotting.py#L136) — documented in [ai_scientist-llm](../../concepts/ai_scientist-llm.md)
- `build_aggregator_prompt(combined_summaries_str, idea_text)` — [`L52`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_plotting.py#L52)
- `extract_code_snippet(text: str)` — [`L89`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_plotting.py#L89) — Look for a Python code block in triple backticks in the LLM response.
- `main()` — [`L257`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_plotting.py#L257)
- `run_aggregator_script(aggregator_code, aggregator_script_path, base_folder, script_name)` — [`L99`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_plotting.py#L99)

## Module values
- `AGGREGATOR_SYSTEM_MSG` — [`L21`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_plotting.py#L21)
- `MAX_FIGURES` — [`L19`](../../../../../raw/code/ai-scientist-v2/ai_scientist/perform_plotting.py#L19)

