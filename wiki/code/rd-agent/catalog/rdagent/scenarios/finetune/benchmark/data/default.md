---
title: 'Module: rdagent/scenarios/finetune/benchmark/data/default.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/benchmark/data/default.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.benchmark.data.default`/
symbols:
  extract_error_samples: extract_error_samples().
  _to_bool: _to_bool().
  _format_value: _format_value().
  _get_question: _get_question().
  _is_correct: _is_correct().
  _get_gold: _get_gold().
  _get_prediction: _get_prediction().
  _format_prompt: _format_prompt().
  _extract_tag_content: _extract_tag_content().
---
# Module: [`rdagent/scenarios/finetune/benchmark/data/default.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py)

## Functions
- `_extract_tag_content(prompt: Any, tag_name: str)` — [`L111`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L111) — Extract content from <tag_name Begin>...<tag_name End> in prompt.
- `_format_prompt(prompt: Any)` — [`L71`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L71) — Format prompt to readable string (matches model input format).
- `_format_value(value: Any)` — [`L62`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L62) — Format value to string, handling list/dict/None.
- `_get_gold(sample: Dict, pred_entry: Dict)` — [`L160`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L160) — Extract gold/reference answer - prioritize predictions.
- `_get_prediction(sample: Dict, pred_entry: Dict)` — [`L182`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L182) — Extract model prediction/output - prioritize predictions.
- `_get_question(sample: Dict, pred_entry: Dict)` — [`L137`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L137) — Extract question - prioritize predictions for complete content.
- `_is_correct(sample: Dict)` — [`L38`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L38) — Unified correctness check - returns True if sample is correct (should be skipped).
- `_to_bool(value: Any)` — [`L22`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L22) — Unified boolean conversion supporting multiple types.
- `extract_error_samples(results_base: Path, max_samples: int = 10)` — [`L208`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/benchmark/data/default.py#L208) — Extract error samples from OpenCompass benchmark results.

