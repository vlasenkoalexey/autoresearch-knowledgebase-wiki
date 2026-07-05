---
title: 'Module: examples/web_scraper_optillm/evaluator.py'
type: catalog
provenance: extracted
module: examples/web_scraper_optillm/evaluator.py
status: fresh
symbol_base: scip-python python openevolve 0.0.0 `examples.web_scraper_optillm.evaluator`/
symbols:
  evaluate: evaluate().
  get_test_cases: get_test_cases().
  evaluate_extraction: evaluate_extraction().
  generate_feedback: generate_feedback().
---
# Module: [`examples/web_scraper_optillm/evaluator.py`](../../../../../../raw/code/openevolve/examples/web_scraper_optillm/evaluator.py)

## Functions
- `evaluate(program_path: str)` — [`L18`](../../../../../../raw/code/openevolve/examples/web_scraper_optillm/evaluator.py#L18) — Evaluate the web scraper program.
- `evaluate_extraction(docs: List[Dict[str, Any]], expected: List[Dict[str, Any]])` — [`L260`](../../../../../../raw/code/openevolve/examples/web_scraper_optillm/evaluator.py#L260) — Evaluate the accuracy of extracted documentation.
- `generate_feedback(metrics: Dict[str, float], artifacts: Dict[str, Any])` — [`L301`](../../../../../../raw/code/openevolve/examples/web_scraper_optillm/evaluator.py#L301) — Generate detailed feedback for the LLM to improve the scraper.
- `get_test_cases()` — [`L114`](../../../../../../raw/code/openevolve/examples/web_scraper_optillm/evaluator.py#L114) — Get test cases with HTML content and expected results.

