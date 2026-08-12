---
title: 'Module: OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.data_produce.baseline_filter`/
symbols:
  evaluate_baseline_token_gap: evaluate_baseline_token_gap().
  BaselineTokenGapDecision: BaselineTokenGapDecision#
  BaselineTokenGapConfig: BaselineTokenGapConfig#
  BaselineTokenGapDecision.token_length: BaselineTokenGapDecision#token_length.
  BaselineTokenGapConfig.gap_config: BaselineTokenGapConfig#gap_config.
  BaselineTokenGapConfig.max_total_tokens: BaselineTokenGapConfig#max_total_tokens.
  BaselineTokenGapDecision.gap_info: BaselineTokenGapDecision#gap_info.
  BaselineTokenGapConfig.keep_equal: BaselineTokenGapConfig#keep_equal.
  BaselineTokenGapDecision.accepted: BaselineTokenGapDecision#accepted.
  BaselineTokenGapDecision.reason: BaselineTokenGapDecision#reason.
---
# Module: [`OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py)

## Classes
### `BaselineTokenGapConfig`
- def: [`OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py:18`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L18) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Configuration shared by generation-time and postprocess filtering.
- signature: `class BaselineTokenGapConfig:`
- members:
  - `gap_config` — [`L22`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L22) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `keep_equal` — [`L23`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L23)
  - `max_total_tokens` — [`L21`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L21) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- uses (calls/refs, reference-scoped): [`GapFilterConfig`](gap_filter.md#GapFilterConfig)
- used by: [`evaluate_baseline_token_gap`](baseline_filter.md#evaluate_baseline_token_gap), [`_baseline_config`](../services/rejection.md#BaselinePostprocessPolicy._baseline_config)

### `BaselineTokenGapDecision`
- def: [`OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py:27`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L27)
- doc: Decision returned by the shared baseline token/gap filter.
- signature: `class BaselineTokenGapDecision:`
- members:
  - `accepted` — [`L30`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L30)
  - `gap_info` — [`L33`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L33)
  - `reason` — [`L31`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L31)
  - `token_length` — [`L32`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L32)
- used by: [`evaluate_baseline_token_gap`](baseline_filter.md#evaluate_baseline_token_gap), [`_baseline_decision`](../services/rejection.md#BaselinePostprocessPolicy._baseline_decision)

## Functions
- `evaluate_baseline_token_gap(*, slime_message_tokens: Any, feedback_text: str | None, metadata: Mapping[str, Any] | None, config: BaselineTokenGapConfig | None = None, task_score_scale: float | None = None)` — [`L36`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/baseline_filter.py#L36) — Apply the baseline token and validation/test gap filters.

