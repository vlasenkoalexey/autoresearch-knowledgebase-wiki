---
title: 'Module: OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.tts_search.services.tree_search_state`/
symbols:
  build_state_from_replay: build_state_from_replay().
  replay_search_events: replay_search_events().
  validate_state_consistency: validate_state_consistency().
  SearchEvent: SearchEvent#
  SearchEvent.__post_init__: SearchEvent#__post_init__().
  SearchState: SearchState#
  atomic_write_search_state: atomic_write_search_state().
  append_search_event: append_search_event().
  SearchEvent.event_type: SearchEvent#event_type.
  read_search_events: read_search_events().
  ReplaySummary.generated_count: ReplaySummary#generated_count().
  ReplaySummary.completed_count: ReplaySummary#completed_count().
  ReplaySummary.accepted_count: ReplaySummary#accepted_count().
  NODE_GENERATED: NODE_GENERATED.
  NODE_EVALUATED: NODE_EVALUATED.
  SearchEvent.search_step: SearchEvent#search_step.
  SearchEvent.program_id: SearchEvent#program_id.
  SearchEvent.parent_ids: SearchEvent#parent_ids.
  SearchEvent.generation_mode: SearchEvent#generation_mode.
  SearchEvent.code_path: SearchEvent#code_path.
  SearchState.next_search_step: SearchState#next_search_step.
  SearchState.generated_count: SearchState#generated_count.
  SearchState.completed_count: SearchState#completed_count.
  SearchState.accepted_count: SearchState#accepted_count.
  ReplaySummary.next_search_step: ReplaySummary#next_search_step.
  load_search_state: load_search_state().
  SearchEvent.task_id: SearchEvent#task_id.
  SearchEvent.search_algorithm: SearchEvent#search_algorithm.
  SearchEvent.task_name: SearchEvent#task_name.
  SearchEvent.generated_count: SearchEvent#generated_count.
  SearchEvent.stop_requested: SearchEvent#stop_requested.
  ReplaySummary: ReplaySummary#
  ReplaySummary.generated_program_ids: ReplaySummary#generated_program_ids.
  ReplaySummary.program_ids: ReplaySummary#program_ids.
  SearchEvent.from_dict: SearchEvent#from_dict().
  SearchState.from_dict: SearchState#from_dict().
  utc_now_iso: utc_now_iso().
  SearchEvent.score: SearchEvent#score.
  SearchEvent.fitness: SearchEvent#fitness.
  SearchEvent.accepted_by_rejection_policy: SearchEvent#accepted_by_rejection_policy.
  SearchState.task_id: SearchState#task_id.
  SearchState.search_algorithm: SearchState#search_algorithm.
  SearchState.task_name: SearchState#task_name.
  SearchState.accepted_target: SearchState#accepted_target.
  SearchState.max_generated: SearchState#max_generated.
  SearchState.stop_requested: SearchState#stop_requested.
  SearchState.program_ids: SearchState#program_ids.
  SearchState.program_scores: SearchState#program_scores.
  SearchState.program_fitness: SearchState#program_fitness.
  SearchState.program_code_paths: SearchState#program_code_paths.
  SearchState.parent_map: SearchState#parent_map.
  SearchState.generation_modes: SearchState#generation_modes.
  ReplaySummary.evaluated_program_ids: ReplaySummary#evaluated_program_ids.
  ReplaySummary.program_scores: ReplaySummary#program_scores.
  ReplaySummary.program_fitness: ReplaySummary#program_fitness.
  ReplaySummary.program_code_paths: ReplaySummary#program_code_paths.
  ReplaySummary.parent_map: ReplaySummary#parent_map.
  ReplaySummary.generation_modes: ReplaySummary#generation_modes.
  ReplaySummary.stop_requested: ReplaySummary#stop_requested.
  SearchEvent.timestamp: SearchEvent#timestamp.
  SearchEvent.schema_version: SearchEvent#schema_version.
  SearchState.updated_at: SearchState#updated_at.
  SearchState.schema_version: SearchState#schema_version.
  SCHEMA_VERSION: SCHEMA_VERSION.
  SearchEvent.code_sha256: SearchEvent#code_sha256.
  SearchEvent.reward: SearchEvent#reward.
  SearchEvent.feedback_path: SearchEvent#feedback_path.
  SearchEvent.raw_log_path: SearchEvent#raw_log_path.
  SearchEvent.rejection_reason: SearchEvent#rejection_reason.
  SearchEvent.completed_count: SearchEvent#completed_count.
  SearchEvent.accepted_count: SearchEvent#accepted_count.
  SearchState.island_populations: SearchState#island_populations.
  SearchState.generation_buffer: SearchState#generation_buffer.
  SearchState.journal_path: SearchState#journal_path.
  ReplaySummary.accepted_program_ids: ReplaySummary#accepted_program_ids.
  SearchEvent.extra: SearchEvent#extra.
  SearchEvent.to_dict: SearchEvent#to_dict().
  SearchState.event_log_path: SearchState#event_log_path.
  SearchState.to_dict: SearchState#to_dict().
  ReplaySummary.generated_but_not_evaluated: ReplaySummary#generated_but_not_evaluated.
  SearchState.extra: SearchState#extra.
---
# Module: [`OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py)

## Classes
### `ReplaySummary`
- def: [`OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py:118`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L118) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- doc: Counters and indexes reconstructed from search_events.jsonl.
- signature: `class ReplaySummary:`
- members:
  - `accepted_count(self)` — [`L143`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L143) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `completed_count(self)` — [`L139`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L139) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `generated_count(self)` — [`L135`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L135) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `accepted_program_ids` — [`L123`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L123) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `evaluated_program_ids` — [`L122`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L122) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `generated_but_not_evaluated` — [`L124`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L124) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `generated_program_ids` — [`L121`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L121) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `generation_modes` — [`L130`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L130) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `next_search_step` — [`L131`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L131)
  - `parent_map` — [`L129`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L129) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `program_code_paths` — [`L128`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L128)
  - `program_fitness` — [`L127`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L127)
  - `program_ids` — [`L125`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L125) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `program_scores` — [`L126`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L126)
  - `stop_requested` — [`L132`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L132)
- used by: [`build_state_from_replay`](tree_search_state.md#build_state_from_replay), [`replay_search_events`](tree_search_state.md#replay_search_events), [`validate_state_consistency`](tree_search_state.md#validate_state_consistency)  (2 test-only)

### `SearchEvent`
- def: [`OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py:25`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L25) — documented in [OpenMLE-ERL-SFT-tts_search-services-scheduler](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md)
- doc: Append-only event for one generated or evaluated tree-search node.
- signature: `class SearchEvent:`
- members:
  - `from_dict(cls, data: dict[str, Any])` — [`L68`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L68) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `to_dict(self)` — [`L61`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L61)
  - `accepted_by_rejection_policy` — [`L43`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L43) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `accepted_count` — [`L47`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L47)
  - `code_path` — [`L36`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L36) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `code_sha256` — [`L37`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L37)
  - `completed_count` — [`L46`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L46)
  - `event_type` — [`L28`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L28)
  - `extra` — [`L51`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L51)
  - `feedback_path` — [`L41`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L41)
  - `fitness` — [`L40`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L40) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `generated_count` — [`L45`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L45)
  - `generation_mode` — [`L35`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L35) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `parent_ids` — [`L34`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L34) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `program_id` — [`L32`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L32) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `raw_log_path` — [`L42`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L42)
  - `rejection_reason` — [`L44`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L44)
  - `reward` — [`L39`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L39)
  - `schema_version` — [`L50`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L50)
  - `score` — [`L38`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L38) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `search_algorithm` — [`L30`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L30)
  - `search_step` — [`L31`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L31) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `stop_requested` — [`L48`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L48) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `task_id` — [`L29`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L29)
  - `task_name` — [`L33`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L33)
  - `timestamp` — [`L49`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L49)
- protocol/private: `__post_init__`[`L53`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L53)
- uses (calls/refs, reference-scoped): [`NODE_EVALUATED`](tree_search_state.md#NODE_EVALUATED), [`NODE_GENERATED`](tree_search_state.md#NODE_GENERATED), [`utc_now_iso`](tree_search_state.md#utc_now_iso), [`SCHEMA_VERSION`](tree_search_state.md#SCHEMA_VERSION)
- used by: [`_on_eval_result`](scheduler.md#Scheduler._on_eval_result), [`_on_gen_result`](scheduler.md#Scheduler._on_gen_result), [`replay_search_events`](tree_search_state.md#replay_search_events), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`append_search_event`](tree_search_state.md#append_search_event), [`read_search_events`](tree_search_state.md#read_search_events)  (2 test-only)

### `SearchState`
- def: [`OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py:76`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L76) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- doc: Current resumable state for one task's tree-search run.
- signature: `class SearchState:`
- members:
  - `from_dict(cls, data: dict[str, Any])` — [`L110`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L110)
  - `to_dict(self)` — [`L103`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L103)
  - `accepted_count` — [`L85`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L85)
  - `accepted_target` — [`L86`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L86) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `completed_count` — [`L84`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L84)
  - `event_log_path` — [`L98`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L98)
  - `extra` — [`L101`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L101)
  - `generated_count` — [`L83`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L83) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `generation_buffer` — [`L96`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L96) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `generation_modes` — [`L94`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L94) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `island_populations` — [`L95`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L95) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `journal_path` — [`L97`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L97) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `max_generated` — [`L87`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L87) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `next_search_step` — [`L81`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L81) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `parent_map` — [`L93`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L93) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `program_code_paths` — [`L92`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L92) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `program_fitness` — [`L91`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L91) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `program_ids` — [`L89`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L89) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `program_scores` — [`L90`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L90) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `schema_version` — [`L100`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L100)
  - `search_algorithm` — [`L80`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L80)
  - `stop_requested` — [`L88`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L88)
  - `task_id` — [`L79`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L79) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
  - `task_name` — [`L82`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L82)
  - `updated_at` — [`L99`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L99)
- uses (calls/refs, reference-scoped): [`utc_now_iso`](tree_search_state.md#utc_now_iso), [`SCHEMA_VERSION`](tree_search_state.md#SCHEMA_VERSION)
- used by: [`_write_tree_search_state`](scheduler.md#Scheduler._write_tree_search_state), [`build_state_from_replay`](tree_search_state.md#build_state_from_replay), [`_HAS_MATPLOTLIB`](scheduler.md#_HAS_MATPLOTLIB), [`validate_state_consistency`](tree_search_state.md#validate_state_consistency), [`atomic_write_search_state`](tree_search_state.md#atomic_write_search_state), [`load_search_state`](tree_search_state.md#load_search_state)  (2 test-only)

## Functions
- `append_search_event(event_log_path: Path, event: SearchEvent | dict[str, Any])` — [`L147`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L147) — Append one search event to a JSONL event log. — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- `atomic_write_search_state(state_path: Path, state: SearchState | dict[str, Any])` — [`L174`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L174) — Atomically write the latest resumable search state.
- `build_state_from_replay(*, task_id: str, search_algorithm: str, summary: ReplaySummary, task_name: str | None = None, accepted_target: int | None = None, max_generated: int | None = None, event_log_path: str = "search_events.jsonl", stop_requested: bool | None = None, island_populations: list[list[str]] | None = None, generation_buffer: dict[str, Any] | None = None, journal_path: str | None = None)` — [`L233`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L233) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- `load_search_state(state_path: Path)` — [`L188`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L188)
- `read_search_events(event_log_path: Path)` — [`L158`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L158) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- `replay_search_events(events: Iterable[SearchEvent])` — [`L194`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L194) — Replay events with idempotent counters keyed by program_id. — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- `utc_now_iso()` — [`L18`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L18) — Return a stable UTC timestamp for persisted search records.
- `validate_state_consistency(state: SearchState, summary: ReplaySummary)` — [`L271`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L271) — Fail fast when persisted state and replayed events disagree on counters. — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)

## Module values
- `NODE_EVALUATED` — [`L15`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L15) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- `NODE_GENERATED` — [`L14`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L14) — documented in [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](../../../../../concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md)
- `SCHEMA_VERSION` — [`L13`](../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/tts_search/services/tree_search_state.py#L13)

