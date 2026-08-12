---
title: 'Module: agents/objectives/objective_types.py'
type: catalog
provenance: extracted
module: agents/objectives/objective_types.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.objectives.objective_types`/DirectObjective#
symbols:
  DirectObjective.id: id.
  DirectObjective.description: description.
  DirectObjective: ''
  DirectObjective.action_type: action_type.
  DirectObjective.target_location: target_location.
  DirectObjective.navigation_hint: navigation_hint.
  DirectObjective.completion_condition: completion_condition.
  DirectObjective.priority: priority.
  DirectObjective.category: category.
  DirectObjective.prerequisite_story_objective: prerequisite_story_objective.
  DirectObjective.recommended_battling_objectives: recommended_battling_objectives.
  DirectObjective.to_dict: to_dict().
  DirectObjective.completed: completed.
  DirectObjective.optional: optional.
  DirectObjective.target_coords: target_coords.
  DirectObjective.completed_at: completed_at.
  DirectObjective.from_dict: from_dict().
---
# Module: [`agents/objectives/objective_types.py`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py)

## Classes
### `DirectObjective`
- def: [`agents/objectives/objective_types.py:14`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L14) — documented in [agents-objectives-objective_types](../../../concepts/agents-objectives-objective_types.md)
- doc: Single direct objective with specific guidance.
- signature: `class DirectObjective:`
- members:
  - `from_dict(cls, data: Dict[str, Any])` — [`L79`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L79) — Reconstruct a DirectObjective from a serialized dict.
  - `to_dict(self)` — [`L51`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L51) — Serialize to a JSON-compatible dict for persistence.
  - `action_type` — [`L38`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L38)
  - `category` — [`L39`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L39)
  - `completed` — [`L45`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L45)
  - `completed_at` — [`L46`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L46)
  - `completion_condition` — [`L43`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L43)
  - `description` — [`L37`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L37)
  - `id` — [`L36`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L36)
  - `navigation_hint` — [`L42`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L42)
  - `optional` — [`L47`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L47)
  - `prerequisite_story_objective` — [`L49`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L49)
  - `priority` — [`L44`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L44)
  - `recommended_battling_objectives` — [`L48`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L48)
  - `target_coords` — [`L41`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L41)
  - `target_location` — [`L40`](../../../../../../raw/code/continual-harness/agents/objectives/objective_types.py#L40)
- used by: [`mcp_complete_direct_objective`](../../server/app.md#mcp_complete_direct_objective), [`mcp_get_game_state`](../../server/app.md#mcp_get_game_state), [`replan_category`](direct_objectives.md#DirectObjectiveManager.replan_category), [`story_sequence`](direct_objectives.md#DirectObjectiveManager.story_sequence), [`add_objectives_to_category`](direct_objectives.md#DirectObjectiveManager.add_objectives_to_category), [`load_autonomous_objective_creation_sequence`](direct_objectives.md#DirectObjectiveManager.load_autonomous_objective_creation_sequence), [`_update_objectives_cache`](../../server/app.md#_update_objectives_cache), [`_save_dynamics_objectives_backup`](direct_objectives.md#DirectObjectiveManager._save_dynamics_objectives_backup), [`current_sequence`](direct_objectives.md#DirectObjectiveManager.current_sequence), [`load_categorized_full_game_sequence`](direct_objectives.md#DirectObjectiveManager.load_categorized_full_game_sequence), [`restore_from_state`](direct_objectives.md#DirectObjectiveManager.restore_from_state), [`_get_current_objective_for_category`](direct_objectives.md#DirectObjectiveManager._get_current_objective_for_category), [`battling_sequence`](direct_objectives.md#DirectObjectiveManager.battling_sequence), [`BATTLING_OBJECTIVES`](all_obj_categorized.md#BATTLING_OBJECTIVES), [`_serialize_sequence`](direct_objectives.md#DirectObjectiveManager._serialize_sequence), [`load_part_1_walkthrough_claude_4_5_sequence`](direct_objectives.md#DirectObjectiveManager.load_part_1_walkthrough_claude_4_5_sequence), [`load_tutorial_to_rustboro_city_sequence`](direct_objectives.md#DirectObjectiveManager.load_tutorial_to_rustboro_city_sequence), [`dynamics_sequence`](direct_objectives.md#DirectObjectiveManager.dynamics_sequence), [`STORY_OBJECTIVES`](all_obj_categorized_red.md#STORY_OBJECTIVES), [`get_categorized_objective_guidance`](direct_objectives.md#DirectObjectiveManager.get_categorized_objective_guidance), [`STORY_OBJECTIVES`](all_obj_categorized.md#STORY_OBJECTIVES), [`serialize_full_state`](direct_objectives.md#DirectObjectiveManager.serialize_full_state), [`BATTLING_OBJECTIVES`](all_obj_categorized_red.md#BATTLING_OBJECTIVES), [`add_dynamic_objectives`](direct_objectives.md#DirectObjectiveManager.add_dynamic_objectives), [`load_birch_to_rival_sequence`](direct_objectives.md#DirectObjectiveManager.load_birch_to_rival_sequence), [`load_hackathon_route102_to_petalburg_sequence`](direct_objectives.md#DirectObjectiveManager.load_hackathon_route102_to_petalburg_sequence), [`_build_story_planning_objective`](../../server/app.md#_build_story_planning_objective), [`get_full_sequence_snapshot`](direct_objectives.md#DirectObjectiveManager.get_full_sequence_snapshot), [`get_current_objective_guidance`](direct_objectives.md#DirectObjectiveManager.get_current_objective_guidance), [`complete_objective_in_category`](direct_objectives.md#DirectObjectiveManager.complete_objective_in_category), [`get_categorized_status`](direct_objectives.md#DirectObjectiveManager.get_categorized_status), [`get_current_battling_group`](direct_objectives.md#DirectObjectiveManager.get_current_battling_group), [`get_sequence_status`](direct_objectives.md#DirectObjectiveManager.get_sequence_status), [`_build_story_exhaustion_fallback`](direct_objectives.md#DirectObjectiveManager._build_story_exhaustion_fallback), [`get_first_objective_info`](direct_objectives.md#get_first_objective_info), [`get_current_objective`](direct_objectives.md#DirectObjectiveManager.get_current_objective), [`get_objective_context`](direct_objectives.md#DirectObjectiveManager.get_objective_context), [`_get_sequence_for_category`](direct_objectives.md#DirectObjectiveManager._get_sequence_for_category), [`get_current_objectives_by_category`](direct_objectives.md#DirectObjectiveManager.get_current_objectives_by_category), [`_mark_objective_completed`](direct_objectives.md#DirectObjectiveManager._mark_objective_completed)  (+1 more; 22 test-only)

