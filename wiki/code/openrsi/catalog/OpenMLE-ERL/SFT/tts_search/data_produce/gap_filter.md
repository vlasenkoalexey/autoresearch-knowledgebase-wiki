---
title: 'Module: OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.data_produce.gap_filter`/
symbols:
  annotate_gap_rows: annotate_gap_rows().
  load_task_meta_from_parquet: load_task_meta_from_parquet().
  metadata_to_task_meta: metadata_to_task_meta().
  load_task_meta: load_task_meta().
  choose_gap_denominator: choose_gap_denominator().
  relative_gap_from_feedback: relative_gap_from_feedback().
  _metadata_range_denominator: _metadata_range_denominator().
  TaskMeta: TaskMeta#
  GapFilterConfig: GapFilterConfig#
  filter_by_relative_gap: filter_by_relative_gap().
  _metric_class: _metric_class().
  extract_submission_score: extract_submission_score().
  choose_legacy_gap_denominator: choose_legacy_gap_denominator().
  relative_gap_from_scores: relative_gap_from_scores().
  metric_gap_threshold: metric_gap_threshold().
  enrich_tasks_with_metric_protocol: enrich_tasks_with_metric_protocol().
  GapFilterConfig.max_relative_gap: GapFilterConfig#max_relative_gap.
  _metric_fields_from_metadata: _metric_fields_from_metadata().
  feedback_is_success: feedback_is_success().
  TaskMeta.metric_class: TaskMeta#metric_class.
  extract_validation_score: extract_validation_score().
  TaskMeta.task_id: TaskMeta#task_id.
  TaskMeta.metric_label: TaskMeta#metric_label.
  TaskMeta.metric_name: TaskMeta#metric_name.
  _score_looks_percent_scale: _score_looks_percent_scale().
  TaskMeta.task_name: TaskMeta#task_name.
  TaskMeta.theoretical_min: TaskMeta#theoretical_min.
  TaskMeta.theoretical_max: TaskMeta#theoretical_max.
  TaskMeta.leaderboard_min: TaskMeta#leaderboard_min.
  TaskMeta.leaderboard_max: TaskMeta#leaderboard_max.
  classify_metric: classify_metric().
  _load_metric_fields_from_parquet: _load_metric_fields_from_parquet().
  extract_feedback_status: extract_feedback_status().
  extract_feedback_result: extract_feedback_result().
  TaskMeta.higher_is_better: TaskMeta#higher_is_better.
  TaskMeta.metric_direction: TaskMeta#metric_direction.
  TaskMeta.validation_strategy: TaskMeta#validation_strategy.
  TaskMeta.metric_source: TaskMeta#metric_source.
  lookup_task_meta: lookup_task_meta().
  TaskMeta.matched_text: TaskMeta#matched_text.
  GapFilterConfig.require_comparable: GapFilterConfig#require_comparable.
  _score_scale: _score_scale().
  GapFilterConfig.no_range_is_big: GapFilterConfig#no_range_is_big.
  GapFilterConfig.require_feedback_success: GapFilterConfig#require_feedback_success.
  infer_metricprompt_parquet: infer_metricprompt_parquet().
  _range_size: _range_size().
  SCORE_RE: SCORE_RE.
  FINAL_SCORE_RE: FINAL_SCORE_RE.
  PREFIX_SCORE_RE: PREFIX_SCORE_RE.
  VAL_SCORE_RE: VAL_SCORE_RE.
  STATUS_RE: STATUS_RE.
  RESULT_RE: RESULT_RE.
  GapFilterConfig.theoretical_small_range_max: GapFilterConfig#theoretical_small_range_max.
  GapFilterConfig.big_range_threshold: GapFilterConfig#big_range_threshold.
  GapFilterConfig.unitless_loss_floor: GapFilterConfig#unitless_loss_floor.
  GapFilterConfig.use_metric_aware_denominator: GapFilterConfig#use_metric_aware_denominator.
  _parse_self_valid_protocol: _parse_self_valid_protocol().
  enrich_metadata_with_metric_protocol: enrich_metadata_with_metric_protocol().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py)

## Classes
### `GapFilterConfig`
- def: [`OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py:61`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L61) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- doc: Configuration for relative validation/test gap filtering.
- signature: `class GapFilterConfig:`
- members:
  - `big_range_threshold` — [`L81`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L81) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `max_relative_gap` — [`L79`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L79) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `no_range_is_big` — [`L82`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L82) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `require_comparable` — [`L83`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L83) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `require_feedback_success` — [`L84`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L84)
  - `theoretical_small_range_max` — [`L80`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L80) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `unitless_loss_floor` — [`L85`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L85) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `use_metric_aware_denominator` — [`L86`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L86) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- used by: [`build_sft_dataset`](pipeline.md#build_sft_dataset), [`annotate_gap_rows`](gap_filter.md#annotate_gap_rows), [`evaluate_baseline_token_gap`](baseline_filter.md#evaluate_baseline_token_gap), [`choose_gap_denominator`](gap_filter.md#choose_gap_denominator), [`relative_gap_from_feedback`](gap_filter.md#relative_gap_from_feedback), [`_metadata_range_denominator`](gap_filter.md#_metadata_range_denominator), [`_baseline_config`](../services/rejection.md#BaselinePostprocessPolicy._baseline_config), [`filter_by_relative_gap`](gap_filter.md#filter_by_relative_gap), [`choose_legacy_gap_denominator`](gap_filter.md#choose_legacy_gap_denominator), [`relative_gap_from_scores`](gap_filter.md#relative_gap_from_scores), [`metric_gap_threshold`](gap_filter.md#metric_gap_threshold), [`gap_config`](baseline_filter.md#BaselineTokenGapConfig.gap_config)

### `TaskMeta`
- def: [`OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py:26`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L26) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- doc: Task score-range metadata used by validation/test gap filtering.
- signature: `class TaskMeta:`
- members:
  - `higher_is_better` — [`L45`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L45) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `leaderboard_max` — [`L49`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L49) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `leaderboard_min` — [`L48`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L48) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `matched_text` — [`L57`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L57) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `metric_class` — [`L54`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L54) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `metric_direction` — [`L53`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L53) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `metric_label` — [`L51`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L51) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `metric_name` — [`L52`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L52) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `metric_source` — [`L56`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L56) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `task_id` — [`L50`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L50) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `task_name` — [`L44`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L44) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `theoretical_max` — [`L47`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L47) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `theoretical_min` — [`L46`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L46) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
  - `validation_strategy` — [`L55`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L55) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- used by: [`annotate_gap_rows`](gap_filter.md#annotate_gap_rows), [`load_task_meta_from_parquet`](gap_filter.md#load_task_meta_from_parquet), [`metadata_to_task_meta`](gap_filter.md#metadata_to_task_meta), [`load_task_meta`](gap_filter.md#load_task_meta), [`choose_gap_denominator`](gap_filter.md#choose_gap_denominator), [`relative_gap_from_feedback`](gap_filter.md#relative_gap_from_feedback), [`_metadata_range_denominator`](gap_filter.md#_metadata_range_denominator), [`_metric_class`](gap_filter.md#_metric_class), [`choose_legacy_gap_denominator`](gap_filter.md#choose_legacy_gap_denominator), [`relative_gap_from_scores`](gap_filter.md#relative_gap_from_scores), [`metric_gap_threshold`](gap_filter.md#metric_gap_threshold), [`lookup_task_meta`](gap_filter.md#lookup_task_meta)

## Functions
- `_load_metric_fields_from_parquet(path: Path)` — [`L239`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L239) — Load metric protocol fields keyed by task UUID and task name. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `_metadata_range_denominator(*, metadata: TaskMeta | None, config: GapFilterConfig)` — [`L487`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L487) — Return the legacy range-based denominator candidate. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `_metric_class(metadata: TaskMeta | None)` — [`L541`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L541) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `_metric_fields_from_metadata(row: dict[str, Any])` — [`L198`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L198) — Extract metric classification fields from a parquet metadata row. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `_parse_self_valid_protocol(value: Any)` — [`L129`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L129) — Return a normalized self-validation protocol dictionary. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `_range_size(low: float | None, high: float | None)` — [`L471`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L471) — Compute a positive score range width.
- `_score_looks_percent_scale(validation_score: float | None, test_score: float | None)` — [`L532`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L532) — Heuristically detect 0-100 metric scores. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `_score_scale(validation_score: float | None, test_score: float | None, *, use_abs: bool = True)` — [`L515`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L515) — Return a positive per-row score scale. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `annotate_gap_rows(rows: list[dict[str, Any]], task_meta: dict[str, TaskMeta], config: GapFilterConfig | None = None)` — [`L771`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L771) — Annotate rows with validation/test gap fields. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `choose_gap_denominator(*, metadata: TaskMeta | None, validation_score: float | None, test_score: float | None, config: GapFilterConfig, task_score_scale: float | None = None)` — [`L593`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L593) — Choose a metric-aware denominator for validation/test gap. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `choose_legacy_gap_denominator(*, metadata: TaskMeta | None, validation_score: float | None, test_score: float | None, config: GapFilterConfig)` — [`L562`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L562) — Choose denominator using the previous final-run range rules. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `classify_metric(metric_label: Any, metric_name: Any = None)` — [`L142`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L142) — Classify a metric into a gap-normalization family. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `enrich_metadata_with_metric_protocol(metadata: dict[str, Any], metric_fields: dict[str, dict[str, Any]])` — [`L259`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L259) — Attach metric protocol fields to one task metadata dictionary.
- `enrich_tasks_with_metric_protocol(tasks: list[dict[str, Any]], *, source_parquet: Path | None = None, metric_metadata_parquet: Path | None = None, metadata_key: str = "metadata")` — [`L288`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L288) — Enrich loaded task records with metric protocol from metricprompt parquet.
- `extract_feedback_result(feedback_text: str)` — [`L450`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L450) — Extract sandbox result label from formatted feedback.
- `extract_feedback_status(feedback_text: str)` — [`L444`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L444) — Extract sandbox status from formatted feedback.
- `extract_submission_score(feedback_text: str)` — [`L415`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L415) — Extract final submission/test score from feedback text. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `extract_validation_score(feedback_text: str)` — [`L431`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L431) — Extract validation score from feedback text. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `feedback_is_success(feedback_text: str, *, status_values: set[str] | None = None, result_values: set[str] | None = None)` — [`L456`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L456) — Check whether feedback represents a successful run. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `filter_by_relative_gap(rows: list[dict[str, Any]], config: GapFilterConfig)` — [`L858`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L858) — Split annotated rows by relative gap rules.
- `infer_metricprompt_parquet(path: Path)` — [`L228`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L228) — Infer a sibling ``*_metricprompt/train.parquet`` path when it exists. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `load_task_meta(path: Path)` — [`L89`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L89) — Load task metadata from a CSV manifest. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `load_task_meta_from_parquet(path: Path, *, metadata_col: str = "metadata", metric_metadata_parquet: Path | None = None, enrich_metric_protocol: bool = True)` — [`L326`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L326) — Load task score-range metadata from a source parquet. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `lookup_task_meta(task_name: str, meta_map: dict[str, TaskMeta], *, task_id: str | None = None)` — [`L391`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L391) — Look up task metadata with optional version suffix stripping. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `metadata_to_task_meta(metadata: TaskMeta | dict[str, Any] | None)` — [`L733`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L733) — Convert generation-time metadata dicts to ``TaskMeta``. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `metric_gap_threshold(metadata: TaskMeta | None, config: GapFilterConfig)` — [`L549`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L549) — Return the relative-gap threshold for a task metric. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `relative_gap_from_feedback(feedback_text: str, metadata: TaskMeta | dict[str, Any] | None, config: GapFilterConfig | None = None, *, task_score_scale: float | None = None)` — [`L700`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L700) — Compute metric-aware relative gap from feedback text and metadata. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `relative_gap_from_scores(*, validation_score: float | None, test_score: float | None, metadata: TaskMeta | None, config: GapFilterConfig | None = None, task_score_scale: float | None = None)` — [`L670`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L670) — Compute abs gap, relative gap, denominator source, and threshold. — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)

## Module values
- `FINAL_SCORE_RE` — [`L18`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L18) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `PREFIX_SCORE_RE` — [`L19`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L19) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `RESULT_RE` — [`L22`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L22)
- `SCORE_RE` — [`L17`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L17) — documented in [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md)
- `STATUS_RE` — [`L21`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L21)
- `VAL_SCORE_RE` — [`L20`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/data_produce/gap_filter.py#L20)

