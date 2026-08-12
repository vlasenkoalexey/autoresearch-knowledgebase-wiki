---
title: 'Module: OpenMLE-ERL/SFT/tts_search/services/rejection.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/services/rejection.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.services.rejection`/
symbols:
  RejectionDecision: RejectionDecision#
  build_rejection_policy: build_rejection_policy().
  BaselinePostprocessPolicy._baseline_config: BaselinePostprocessPolicy#_baseline_config.
  MixedLeaderboardBaselinePolicy.accepts_result: MixedLeaderboardBaselinePolicy#accepts_result().
  MixedLeaderboardBaselinePolicy.accepts_record: MixedLeaderboardBaselinePolicy#accepts_record().
  BaselinePostprocessPolicy.accepts_record: BaselinePostprocessPolicy#accepts_record().
  BaselinePostprocessPolicy._baseline_decision: BaselinePostprocessPolicy#_baseline_decision().
  BetterThanReferencePolicy._decide: BetterThanReferencePolicy#_decide().
  BaselinePostprocessPolicy.accepts_result: BaselinePostprocessPolicy#accepts_result().
  RejectionPolicy: RejectionPolicy#
  RejectionDecision.accepted: RejectionDecision#accepted.
  RejectionPolicy.accepts_record: RejectionPolicy#accepts_record().
  MixedLeaderboardBaselinePolicy.target_for_metadata: MixedLeaderboardBaselinePolicy#target_for_metadata().
  ScoreThresholdPolicy._decide: ScoreThresholdPolicy#_decide().
  RewardThresholdPolicy._decide: RewardThresholdPolicy#_decide().
  MixedLeaderboardBaselinePolicy._reference_policy: MixedLeaderboardBaselinePolicy#_reference_policy.
  MEDAL_LABELS: MEDAL_LABELS.
  MedalPolicy.accepts_result: MedalPolicy#accepts_result().
  MedalPolicy.accepts_record: MedalPolicy#accepts_record().
  MixedLeaderboardBaselinePolicy.has_leaderboard: MixedLeaderboardBaselinePolicy#has_leaderboard().
  ScoreThresholdPolicy.accepts_result: ScoreThresholdPolicy#accepts_result().
  ScoreThresholdPolicy.accepts_record: ScoreThresholdPolicy#accepts_record().
  RewardThresholdPolicy.accepts_result: RewardThresholdPolicy#accepts_result().
  RewardThresholdPolicy.accepts_record: RewardThresholdPolicy#accepts_record().
  BetterThanReferencePolicy.accepts_result: BetterThanReferencePolicy#accepts_result().
  BetterThanReferencePolicy.accepts_record: BetterThanReferencePolicy#accepts_record().
  RejectionPolicy.accepts_result: RejectionPolicy#accepts_result().
  MixedLeaderboardBaselinePolicy._medal_policy: MixedLeaderboardBaselinePolicy#_medal_policy.
  _range_size: _range_size().
  _score_beats_reference: _score_beats_reference().
  _metadata_has_leaderboard: _metadata_has_leaderboard().
  RejectionDecision.reason: RejectionDecision#reason.
  MedalPolicy: MedalPolicy#
  ScoreThresholdPolicy._threshold: ScoreThresholdPolicy#_threshold.
  RewardThresholdPolicy._threshold: RewardThresholdPolicy#_threshold.
  BetterThanReferencePolicy: BetterThanReferencePolicy#
  BaselinePostprocessPolicy._inner: BaselinePostprocessPolicy#_inner.
  _lower_is_better: _lower_is_better().
  AcceptAllPolicy.accepts_result: AcceptAllPolicy#accepts_result().
  AcceptAllPolicy.accepts_record: AcceptAllPolicy#accepts_record().
  AcceptScoredPolicy.accepts_result: AcceptScoredPolicy#accepts_result().
  AcceptScoredPolicy.accepts_record: AcceptScoredPolicy#accepts_record().
  MedalPolicy.__init__: MedalPolicy#__init__().
  BaselinePostprocessPolicy.__init__: BaselinePostprocessPolicy#__init__().
  BaselinePostprocessPolicy.name: BaselinePostprocessPolicy#name.
  BaselinePostprocessPolicy.target_for_metadata: BaselinePostprocessPolicy#target_for_metadata().
  AcceptAllPolicy: AcceptAllPolicy#
  AcceptScoredPolicy: AcceptScoredPolicy#
  MedalPolicy._accepted_medals: MedalPolicy#_accepted_medals.
  ScoreThresholdPolicy: ScoreThresholdPolicy#
  RewardThresholdPolicy: RewardThresholdPolicy#
  BetterThanReferencePolicy._reference_scores: BetterThanReferencePolicy#_reference_scores.
  MixedLeaderboardBaselinePolicy: MixedLeaderboardBaselinePolicy#
  BaselinePostprocessPolicy: BaselinePostprocessPolicy#
  _maybe_float: _maybe_float().
  load_reference_scores: load_reference_scores().
  RejectionPolicy.name: RejectionPolicy#name.
  MixedLeaderboardBaselinePolicy._leaderboard_target: MixedLeaderboardBaselinePolicy#_leaderboard_target.
  MixedLeaderboardBaselinePolicy._no_leaderboard_target: MixedLeaderboardBaselinePolicy#_no_leaderboard_target.
  _feedback_from_record: _feedback_from_record().
  AcceptAllPolicy.name: AcceptAllPolicy#name.
  AcceptScoredPolicy.name: AcceptScoredPolicy#name.
  MedalPolicy.name: MedalPolicy#name.
  ScoreThresholdPolicy.name: ScoreThresholdPolicy#name.
  ScoreThresholdPolicy.__init__: ScoreThresholdPolicy#__init__().
  RewardThresholdPolicy.name: RewardThresholdPolicy#name.
  RewardThresholdPolicy.__init__: RewardThresholdPolicy#__init__().
  BetterThanReferencePolicy.name: BetterThanReferencePolicy#name.
  BetterThanReferencePolicy.__init__: BetterThanReferencePolicy#__init__().
  MixedLeaderboardBaselinePolicy.name: MixedLeaderboardBaselinePolicy#name.
  MixedLeaderboardBaselinePolicy.__init__: MixedLeaderboardBaselinePolicy#__init__().
---
# Module: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py)

## Classes
### `AcceptAllPolicy`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:52`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L52)
- doc: Accept every evaluated sample, including failed sandbox runs.
- signature: `class AcceptAllPolicy:`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L60`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L60)
  - `accepts_result(self, result: Any)` — [`L57`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L57)
  - `name` — [`L55`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L55)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision)
- used by: [`build_rejection_policy`](rejection.md#build_rejection_policy)

### `AcceptScoredPolicy`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:68`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L68)
- doc: Accept every sample that has a numeric sandbox score.
- signature: `class AcceptScoredPolicy:`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L78`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L78)
  - `accepts_result(self, result: Any)` — [`L73`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L73)
  - `name` — [`L71`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L71)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision)
- used by: [`build_rejection_policy`](rejection.md#build_rejection_policy)

### `BaselinePostprocessPolicy`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:280`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L280) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Apply GLM-4.7-style token and valid-test gap filters before a policy.
- signature: `class BaselinePostprocessPolicy:`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L311`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L311) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `accepts_result(self, result: Any)` — [`L301`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L301) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `target_for_metadata(self, metadata: Mapping[str, Any] | None)` — [`L325`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L325)
  - `name` — [`L299`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L299)
- protocol/private: `__init__`[`L283`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L283), `_baseline_config`[`L292`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L292), `_baseline_decision`[`L331`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L331), `_inner`[`L291`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L291)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision), [`evaluate_baseline_token_gap`](../data_produce/baseline_filter.md#evaluate_baseline_token_gap), [`GapFilterConfig`](../data_produce/gap_filter.md#GapFilterConfig), [`RejectionPolicy`](rejection.md#RejectionPolicy), [`accepted`](rejection.md#RejectionDecision.accepted), [`max_relative_gap`](../data_produce/gap_filter.md#GapFilterConfig.max_relative_gap), [`accepts_record`](rejection.md#RejectionPolicy.accepts_record), [`BaselineTokenGapConfig`](../data_produce/baseline_filter.md#BaselineTokenGapConfig), [`accepts_result`](rejection.md#RejectionPolicy.accepts_result), [`gap_config`](../data_produce/baseline_filter.md#BaselineTokenGapConfig.gap_config), [`max_total_tokens`](../data_produce/baseline_filter.md#BaselineTokenGapConfig.max_total_tokens), [`require_comparable`](../data_produce/gap_filter.md#GapFilterConfig.require_comparable), [`_feedback_from_record`](rejection.md#_feedback_from_record), [`accepted`](../data_produce/baseline_filter.md#BaselineTokenGapDecision.accepted), [`name`](rejection.md#RejectionPolicy.name), [`reason`](../data_produce/baseline_filter.md#BaselineTokenGapDecision.reason)
- used by: [`build_rejection_policy`](rejection.md#build_rejection_policy)

### `BetterThanReferencePolicy`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:168`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L168) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Accept samples whose score beats a reference model score for the task.
- signature: `class BetterThanReferencePolicy:`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L186`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L186)
  - `accepts_result(self, result: Any)` — [`L178`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L178)
  - `name` — [`L171`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L171)
- protocol/private: `__init__`[`L173`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L173), `_decide`[`L198`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L198), `_reference_scores`[`L174`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L174)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision), [`_score_beats_reference`](rejection.md#_score_beats_reference), [`_lower_is_better`](rejection.md#_lower_is_better)
- used by: [`build_rejection_policy`](rejection.md#build_rejection_policy), [`accepts_record`](rejection.md#MixedLeaderboardBaselinePolicy.accepts_record), [`accepts_result`](rejection.md#MixedLeaderboardBaselinePolicy.accepts_result), [`_reference_policy`](rejection.md#MixedLeaderboardBaselinePolicy._reference_policy)

### `MedalPolicy`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:88`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L88) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Accept samples that earned one of the requested medal labels.
- signature: `class MedalPolicy:`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L103`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L103)
  - `accepts_result(self, result: Any)` — [`L97`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L97)
  - `name` — [`L91`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L91)
- protocol/private: `__init__`[`L93`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L93), `_accepted_medals`[`L95`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L95)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision), [`MEDAL_LABELS`](rejection.md#MEDAL_LABELS)
- used by: [`build_rejection_policy`](rejection.md#build_rejection_policy), [`accepts_record`](rejection.md#MixedLeaderboardBaselinePolicy.accepts_record), [`accepts_result`](rejection.md#MixedLeaderboardBaselinePolicy.accepts_result), [`_medal_policy`](rejection.md#MixedLeaderboardBaselinePolicy._medal_policy)

### `MixedLeaderboardBaselinePolicy`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:226`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L226) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Use medal rejection for leaderboard tasks and baseline-best otherwise.
- signature: `class MixedLeaderboardBaselinePolicy:`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L265`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L265) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `accepts_result(self, result: Any)` — [`L254`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L254) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `has_leaderboard(self, metadata: Mapping[str, Any] | None)` — [`L244`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L244) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `target_for_metadata(self, metadata: Mapping[str, Any] | None)` — [`L247`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L247)
  - `name` — [`L229`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L229)
- protocol/private: `__init__`[`L231`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L231), `_leaderboard_target`[`L241`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L241), `_medal_policy`[`L240`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L240), `_no_leaderboard_target`[`L242`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L242), `_reference_policy`[`L238`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L238)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision), [`_decide`](rejection.md#BetterThanReferencePolicy._decide), [`MEDAL_LABELS`](rejection.md#MEDAL_LABELS), [`accepts_record`](rejection.md#MedalPolicy.accepts_record), [`accepts_result`](rejection.md#MedalPolicy.accepts_result), [`_metadata_has_leaderboard`](rejection.md#_metadata_has_leaderboard), [`BetterThanReferencePolicy`](rejection.md#BetterThanReferencePolicy), [`MedalPolicy`](rejection.md#MedalPolicy)
- used by: [`build_rejection_policy`](rejection.md#build_rejection_policy)

### `RejectionDecision`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:29`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L29) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Decision returned by a rejection policy.
- signature: `class RejectionDecision:`
- members:
  - `accepted` — [`L32`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L32)
  - `reason` — [`L33`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L33)
- used by: [`rebuild_task_states_from_results`](scheduler.md#rebuild_task_states_from_results), [`collect_sft_rows`](../data_produce/collect.md#collect_sft_rows), [`_decision_for_eval`](scheduler.md#Scheduler._decision_for_eval), [`select_top_per_task`](../data_produce/selection.md#select_top_per_task), [`accepts_record`](rejection.md#BaselinePostprocessPolicy.accepts_record), [`accepts_record`](rejection.md#MixedLeaderboardBaselinePolicy.accepts_record), [`accepts_result`](rejection.md#MixedLeaderboardBaselinePolicy.accepts_result), [`_baseline_decision`](rejection.md#BaselinePostprocessPolicy._baseline_decision), [`_decide`](rejection.md#BetterThanReferencePolicy._decide), [`accepts_result`](rejection.md#BaselinePostprocessPolicy.accepts_result), [`accepts_record`](rejection.md#RejectionPolicy.accepts_record), [`_decide`](rejection.md#RewardThresholdPolicy._decide), [`_decide`](rejection.md#ScoreThresholdPolicy._decide), [`accepts_record`](rejection.md#MedalPolicy.accepts_record), [`accepts_result`](rejection.md#MedalPolicy.accepts_result), [`accepts_record`](rejection.md#BetterThanReferencePolicy.accepts_record), [`accepts_record`](rejection.md#RewardThresholdPolicy.accepts_record), [`accepts_record`](rejection.md#ScoreThresholdPolicy.accepts_record), [`accepts_result`](rejection.md#BetterThanReferencePolicy.accepts_result), [`accepts_result`](rejection.md#RewardThresholdPolicy.accepts_result), [`accepts_result`](rejection.md#ScoreThresholdPolicy.accepts_result), [`accepts_result`](rejection.md#RejectionPolicy.accepts_result), [`accepts_record`](rejection.md#AcceptAllPolicy.accepts_record), [`accepts_record`](rejection.md#AcceptScoredPolicy.accepts_record), [`accepts_result`](rejection.md#AcceptAllPolicy.accepts_result), [`accepts_result`](rejection.md#AcceptScoredPolicy.accepts_result)  (1 test-only)

### `RejectionPolicy`  ·  implements/extends Protocol
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:36`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L36) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Interface for deciding whether an evaluated sample is accepted.
- signature: `class RejectionPolicy(Protocol):`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L44`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L44) — Return whether a serialized eval_results.jsonl record is accepted. — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `accepts_result(self, result: Any)` — [`L41`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L41) — Return whether an EvaluationResult-like object should be accepted. — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
  - `name` — [`L39`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L39)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision)
- used by: [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`rebuild_task_states_from_results`](scheduler.md#rebuild_task_states_from_results), [`collect_sft_rows`](../data_produce/collect.md#collect_sft_rows), [`build_rejection_policy`](rejection.md#build_rejection_policy), [`_decision_for_eval`](scheduler.md#Scheduler._decision_for_eval), [`select_top_per_task`](../data_produce/selection.md#select_top_per_task), [`accepts_record`](rejection.md#BaselinePostprocessPolicy.accepts_record), [`accepts_result`](rejection.md#BaselinePostprocessPolicy.accepts_result), [`_build_accepted_targets`](scheduler.md#Scheduler._build_accepted_targets), [`__init__`](rejection.md#BaselinePostprocessPolicy.__init__), [`name`](rejection.md#BaselinePostprocessPolicy.name)  (1 test-only)

### `RewardThresholdPolicy`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:141`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L141) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Accept samples whose reward is at least a fixed threshold.
- signature: `class RewardThresholdPolicy:`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L152`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L152)
  - `accepts_result(self, result: Any)` — [`L149`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L149)
  - `name` — [`L144`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L144)
- protocol/private: `__init__`[`L146`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L146), `_decide`[`L159`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L159), `_threshold`[`L147`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L147)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision)
- used by: [`build_rejection_policy`](rejection.md#build_rejection_policy)

### `ScoreThresholdPolicy`
- def: [`OpenMLE-ERL/SFT/tts_search/services/rejection.py:114`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L114) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- doc: Accept samples whose sandbox score is at least a fixed threshold.
- signature: `class ScoreThresholdPolicy:`
- members:
  - `accepts_record(self, record: Mapping[str, Any], metadata: Mapping[str, Any] | None = None)` — [`L125`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L125)
  - `accepts_result(self, result: Any)` — [`L122`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L122)
  - `name` — [`L117`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L117)
- protocol/private: `__init__`[`L119`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L119), `_decide`[`L132`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L132), `_threshold`[`L120`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L120)
- uses (calls/refs, reference-scoped): [`RejectionDecision`](rejection.md#RejectionDecision)
- used by: [`build_rejection_policy`](rejection.md#build_rejection_policy)

## Functions
- `_feedback_from_record(record: Mapping[str, Any])` — [`L368`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L368)
- `_lower_is_better(metadata: Mapping[str, Any] | None)` — [`L380`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L380) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `_maybe_float(value: Any)` — [`L347`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L347)
- `_metadata_has_leaderboard(metadata: Mapping[str, Any] | None)` — [`L397`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L397) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `_range_size(low: Any, high: Any)` — [`L359`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L359) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `_score_beats_reference(score: float, reference: float, metadata: Mapping[str, Any] | None)` — [`L389`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L389) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `build_rejection_policy(*, name: str | None, score_threshold: float | None = None, reward_threshold: float | None = None, reference_scores_path: str | Path | None = None, accepted_medals: list[str] | tuple[str, ...] | set[str] | None = None, apply_baseline_filters: bool = False, baseline_token_limit: int = 32768, baseline_relative_gap_limit: float = 0.12, mixed_leaderboard_target: int = 2, mixed_no_leaderboard_target: int = 4)` — [`L456`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L456) — Build a rejection policy from config values. — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)
- `load_reference_scores(path: str | Path)` — [`L421`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L421) — Load reference scores from JSON/JSONL. — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)

## Module values
- `MEDAL_LABELS` — [`L25`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/rejection.py#L25) — documented in [OpenMLE-ERL-SFT-tts_search-services-rejection](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md)

