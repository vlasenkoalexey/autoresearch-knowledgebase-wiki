---
title: 'Module: agents/objectives/direct_objectives.py'
type: catalog
provenance: extracted
module: agents/objectives/direct_objectives.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.objectives.direct_objectives`/
symbols:
  DirectObjectiveManager.replan_category: DirectObjectiveManager#replan_category().
  DirectObjectiveManager.story_sequence: DirectObjectiveManager#story_sequence.
  DirectObjectiveManager.add_objectives_to_category: DirectObjectiveManager#add_objectives_to_category().
  DirectObjectiveManager.load_autonomous_objective_creation_sequence: DirectObjectiveManager#load_autonomous_objective_creation_sequence().
  logger: logger.
  DirectObjectiveManager._save_dynamics_objectives_backup: DirectObjectiveManager#_save_dynamics_objectives_backup().
  DirectObjectiveManager.current_sequence: DirectObjectiveManager#current_sequence.
  DirectObjectiveManager.load_categorized_full_game_sequence: DirectObjectiveManager#load_categorized_full_game_sequence().
  DirectObjectiveManager.restore_from_state: DirectObjectiveManager#restore_from_state().
  DirectObjectiveManager._get_current_objective_for_category: DirectObjectiveManager#_get_current_objective_for_category().
  DirectObjectiveManager.battling_sequence: DirectObjectiveManager#battling_sequence.
  DirectObjectiveManager._serialize_sequence: DirectObjectiveManager#_serialize_sequence().
  DirectObjectiveManager.story_index: DirectObjectiveManager#story_index.
  DirectObjectiveManager.load_tutorial_to_rustboro_city_sequence: DirectObjectiveManager#load_tutorial_to_rustboro_city_sequence().
  DirectObjectiveManager.load_part_1_walkthrough_claude_4_5_sequence: DirectObjectiveManager#load_part_1_walkthrough_claude_4_5_sequence().
  DirectObjectiveManager.dynamics_sequence: DirectObjectiveManager#dynamics_sequence.
  DirectObjectiveManager.get_categorized_objective_guidance: DirectObjectiveManager#get_categorized_objective_guidance().
  DirectObjectiveManager.battling_index: DirectObjectiveManager#battling_index.
  DirectObjectiveManager.serialize_full_state: DirectObjectiveManager#serialize_full_state().
  DirectObjectiveManager.load_birch_to_rival_sequence: DirectObjectiveManager#load_birch_to_rival_sequence().
  DirectObjectiveManager.load_hackathon_route102_to_petalburg_sequence: DirectObjectiveManager#load_hackathon_route102_to_petalburg_sequence().
  DirectObjectiveManager.add_dynamic_objectives: DirectObjectiveManager#add_dynamic_objectives().
  DirectObjectiveManager.current_index: DirectObjectiveManager#current_index.
  DirectObjectiveManager.mode: DirectObjectiveManager#mode.
  DirectObjectiveManager.dynamics_index: DirectObjectiveManager#dynamics_index.
  DirectObjectiveManager.reset_sequence: DirectObjectiveManager#reset_sequence().
  DirectObjectiveManager.is_sequence_active: DirectObjectiveManager#is_sequence_active().
  DirectObjectiveManager.get_full_sequence_snapshot: DirectObjectiveManager#get_full_sequence_snapshot().
  DirectObjectiveManager.get_current_objective_guidance: DirectObjectiveManager#get_current_objective_guidance().
  DirectObjectiveManager.complete_objective_in_category: DirectObjectiveManager#complete_objective_in_category().
  DirectObjectiveManager.get_categorized_status: DirectObjectiveManager#get_categorized_status().
  DirectObjectiveManager.sequence_name: DirectObjectiveManager#sequence_name.
  DirectObjectiveManager.get_current_battling_group: DirectObjectiveManager#get_current_battling_group().
  DirectObjectiveManager.get_sequence_status: DirectObjectiveManager#get_sequence_status().
  DirectObjectiveManager.auto_save: DirectObjectiveManager#auto_save().
  DirectObjectiveManager: DirectObjectiveManager#
  DirectObjectiveManager._build_story_exhaustion_fallback: DirectObjectiveManager#_build_story_exhaustion_fallback().
  get_first_objective_info: get_first_objective_info().
  DirectObjectiveManager.get_current_objective: DirectObjectiveManager#get_current_objective().
  DirectObjectiveManager.get_objective_context: DirectObjectiveManager#get_objective_context().
  DirectObjectiveManager._get_sequence_for_category: DirectObjectiveManager#_get_sequence_for_category().
  DirectObjectiveManager.enable_categorized_mode: DirectObjectiveManager#enable_categorized_mode().
  DirectObjectiveManager.get_current_objectives_by_category: DirectObjectiveManager#get_current_objectives_by_category().
  DirectObjectiveManager._mark_objective_completed: DirectObjectiveManager#_mark_objective_completed().
  DirectObjectiveManager._get_index_for_category: DirectObjectiveManager#_get_index_for_category().
  DirectObjectiveManager._set_index_for_category: DirectObjectiveManager#_set_index_for_category().
  DirectObjectiveManager.save_to_file: DirectObjectiveManager#save_to_file().
  DirectObjectiveManager.load_from_file: DirectObjectiveManager#load_from_file().
  DirectObjectiveManager.save_completed_objectives: DirectObjectiveManager#save_completed_objectives().
  DirectObjectiveManager._OBJECTIVES_JSON_VERSION: DirectObjectiveManager#_OBJECTIVES_JSON_VERSION.
  DirectObjectiveManager._is_objective_completed: DirectObjectiveManager#_is_objective_completed().
  DirectObjectiveManager.obj_to_dict: DirectObjectiveManager#obj_to_dict().
  DirectObjectiveManager.__init__: DirectObjectiveManager#__init__().
---
# Module: [`agents/objectives/direct_objectives.py`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py)

## Classes
### `DirectObjectiveManager`
- def: [`agents/objectives/direct_objectives.py:55`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L55)
- doc: Manages objective sequences across 3 categories: story, battling, and dynamics
- signature: `class DirectObjectiveManager:`
- members:
  - `_build_story_exhaustion_fallback(self)` — [`L3285`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3285) — Build scaffold-aware guidance for continuing objectives planning.
  - `_get_current_objective_for_category(self, category: str)` — [`L3317`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3317) — Get current objective for a specific category
  - `_get_sequence_for_category(self, category: str)` — [`L3468`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3468) — Helper to get sequence list for a category
  - `_is_objective_completed(self, objective: DirectObjective, game_state: Dict[str, Any])` — [`L3034`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3034) — DEPRECATED: Check if an objective is completed based on game state.
  - `_mark_objective_completed(self, objective: DirectObjective)` — [`L3053`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3053) — Mark an objective as completed
  - `_save_dynamics_objectives_backup(self, run_dir: Optional[str] = None)` — [`L3541`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3541) — Save dynamics objectives history to backup file (similar to all_obj.py format)
  - `add_dynamic_objectives(self, objectives_data: List[Dict[str, Any]], set_as_current: bool = True)` — [`L3058`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3058) — Add dynamically created objectives to the current sequence
  - `add_objectives_to_category(self, category: str, objectives_data: List[Dict[str, Any]], run_dir: Optional[str] = None)` — [`L3418`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3418) — Add objectives to a specific category — documented in [agents-objectives-direct_objectives](../../../concepts/agents-objectives-direct_objectives.md)
  - `auto_save(self)` — [`L3908`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3908) — Persist current state to the standard cache and run_data locations.
  - `complete_objective_in_category(self, category: str, reasoning: str = "")` — [`L3478`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3478) — Mark current objective in specified category as complete and advance index
  - `enable_categorized_mode(self)` — [`L3160`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3160) — Enable categorized objectives mode with 3 separate sequences
  - `get_categorized_objective_guidance(self, game_state: Dict[str, Any] = None)` — [`L2957`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L2957) — Get guidance for all current objectives in categorized mode.
  - `get_categorized_status(self)` — [`L3513`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3513) — Get status summary for all 3 categories
  - `get_current_battling_group(self)` — [`L3367`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3367) — Get all battling objectives in the current group (same prerequisite)
  - `get_current_objective(self)` — [`L2927`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L2927) — Get the current objective in the sequence
  - `get_current_objective_guidance(self, game_state: Dict[str, Any] = None)` — [`L2933`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L2933) — Get guidance for the current objective.
  - `get_current_objectives_by_category(self)` — [`L3269`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3269) — Get current objectives for all 3 categories
  - `get_full_sequence_snapshot(self)` — [`L3757`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3757) — Return the complete objective state across all three categories.
  - `get_objective_context(self, game_state: Dict[str, Any] = None)` — [`L3134`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3134) — Get previous objective context for better agent understanding.
  - `get_sequence_status(self)` — [`L3099`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3099) — Get current status of the objective sequence
  - `is_sequence_active(self)` — [`L3123`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3123) — Check if a sequence is currently active
  - `load_autonomous_objective_creation_sequence(self, start_index: int = 0, run_dir: Optional[str] = None)` — [`L2806`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L2806) — Load a sequence with one objective that triggers the objectives-planning subagent.
  - `load_birch_to_rival_sequence(self)` — [`L77`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L77) — Load the hardcoded sequence for transitioning from birch state to rival state.
  - `load_categorized_full_game_sequence(self, start_story_index: int = 0, start_battling_index: int = 0, run_dir: Optional[str] = None)` — [`L3166`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3166) — Load the full game sequence split into story and battling categories
  - `load_from_file(cls, path: str)` — [`L3900`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3900) — Create a new manager restored from a previously saved objectives.json.
  - `load_hackathon_route102_to_petalburg_sequence(self)` — [`L161`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L161) — Load the hardcoded sequence for navigating from Route 102 to Petalburg City.
  - `load_part_1_walkthrough_claude_4_5_sequence(self, start_index: int = 0, run_dir: Optional[str] = None)` — [`L2559`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L2559) — Load the Part 1 walkthrough sequence from game start through Route 104.
  - `load_tutorial_to_rustboro_city_sequence(self, start_index: int = 0, run_dir: Optional[str] = None)` — [`L218`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L218) — Load the combined sequence from tutorial to rustboro city (10 objectives total).
  - `obj_to_dict(obj)` — [`L3212`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3212)
  - `replan_category(self, category: str, edits: List[Dict[str, Any]])` — [`L3613`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3613) — Apply a batch of index-based edits to a single objective category. — documented in [agents-objectives-direct_objectives](../../../concepts/agents-objectives-direct_objectives.md)
  - `reset_sequence(self)` — [`L3110`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3110) — Reset the current sequence
  - `restore_from_state(self, data: Dict[str, Any])` — [`L3842`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3842) — Reconstruct manager state from a dict produced by ``serialize_full_state``.
  - `save_completed_objectives(self, run_dir: Optional[str] = None)` — [`L3088`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3088) — DEPRECATED: Use auto_save() instead. Delegates to auto_save() for backward compat.
  - `save_to_file(self, path: str)` — [`L3881`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3881) — Serialize full state and write to *path* atomically.
  - `serialize_full_state(self)` — [`L3813`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3813) — Serialize the complete manager state for persistence to objectives.json.
  - `battling_index` — [`L69`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L69)
  - `battling_sequence` — [`L68`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L68)
  - `current_index` — [`L61`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L61)
  - `current_sequence` — [`L60`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L60)
  - `dynamics_index` — [`L72`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L72)
  - `dynamics_sequence` — [`L71`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L71)
  - `mode` — [`L75`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L75)
  - `sequence_name` — [`L62`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L62)
  - `story_index` — [`L66`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L66)
  - `story_sequence` — [`L65`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L65)
- protocol/private: `_OBJECTIVES_JSON_VERSION`[`L3811`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3811), `__init__`[`L58`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L58), `_get_index_for_category`[`L3604`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3604), `_serialize_sequence`[`L3763`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3763), `_set_index_for_category`[`L3749`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L3749)
- uses (calls/refs, reference-scoped): [`id`](objective_types.md#DirectObjective.id), [`description`](objective_types.md#DirectObjective.description), [`DirectObjective`](objective_types.md#DirectObjective), [`action_type`](objective_types.md#DirectObjective.action_type), [`target_location`](objective_types.md#DirectObjective.target_location), [`completion_condition`](objective_types.md#DirectObjective.completion_condition), [`navigation_hint`](objective_types.md#DirectObjective.navigation_hint), [`priority`](objective_types.md#DirectObjective.priority), [`category`](objective_types.md#DirectObjective.category), [`get_cache_path`](../../utils/data_persistence/run_data_manager.md#get_cache_path), [`prerequisite_story_objective`](objective_types.md#DirectObjective.prerequisite_story_objective), [`get_run_data_manager`](../../utils/data_persistence/run_data_manager.md#get_run_data_manager), [`logger`](direct_objectives.md#logger), [`recommended_battling_objectives`](objective_types.md#DirectObjective.recommended_battling_objectives), [`to_dict`](objective_types.md#DirectObjective.to_dict), [`completed`](objective_types.md#DirectObjective.completed), [`optional`](objective_types.md#DirectObjective.optional), [`STORY_OBJECTIVES`](all_obj_categorized_red.md#STORY_OBJECTIVES), [`BATTLING_OBJECTIVES`](all_obj_categorized_red.md#BATTLING_OBJECTIVES), [`target_coords`](objective_types.md#DirectObjective.target_coords), [`completed_at`](objective_types.md#DirectObjective.completed_at), [`get_scratch_space_dir`](../../utils/data_persistence/run_data_manager.md#RunDataManager.get_scratch_space_dir), [`from_dict`](objective_types.md#DirectObjective.from_dict)
- used by: [`mcp_complete_direct_objective`](../../server/app.md#mcp_complete_direct_objective), [`mcp_get_game_state`](../../server/app.md#mcp_get_game_state), [`_update_objectives_cache`](../../server/app.md#_update_objectives_cache), [`mcp_get_progress_summary`](../../server/app.md#mcp_get_progress_summary), [`mcp_replan_objectives`](../../server/app.md#mcp_replan_objectives), [`mcp_get_full_objective_sequence`](../../server/app.md#mcp_get_full_objective_sequence)  (38 test-only)

## Functions
- `get_first_objective_info(sequence_name: str, start_index: int = 0)` — [`L22`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L22) — Get first objective ID and description from a sequence without loading it

## Module values
- `logger` — [`L19`](../../../../../../raw/code/continual-harness/agents/objectives/direct_objectives.py#L19)

