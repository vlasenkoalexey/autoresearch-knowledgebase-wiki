---
title: 'Module: pokemon_red_env/red_milestone_tracker.py'
type: catalog
provenance: extracted
module: pokemon_red_env/red_milestone_tracker.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `pokemon_red_env.red_milestone_tracker`/
symbols:
  RedMilestoneTracker.milestones: RedMilestoneTracker#milestones.
  RedMilestoneTracker.filename: RedMilestoneTracker#filename.
  logger: logger.
  RedMilestoneTracker.mark_completed: RedMilestoneTracker#mark_completed().
  RedMilestoneTracker.load_milestones_for_state: RedMilestoneTracker#load_milestones_for_state().
  RedMilestoneTracker.load_from_file: RedMilestoneTracker#load_from_file().
  RedMilestoneTracker.save_milestones_for_state: RedMilestoneTracker#save_milestones_for_state().
  RedMilestoneTracker.save_to_file: RedMilestoneTracker#save_to_file().
  RedMilestoneTracker._calculate_split_time: RedMilestoneTracker#_calculate_split_time().
  RedMilestoneTracker.reset_all: RedMilestoneTracker#reset_all().
  RedMilestoneTracker.cache_dir: RedMilestoneTracker#cache_dir.
  RedMilestoneTracker.is_completed: RedMilestoneTracker#is_completed().
  RedMilestoneTracker.reset_milestone: RedMilestoneTracker#reset_milestone().
  RedMilestoneTracker._calculate_total_time: RedMilestoneTracker#_calculate_total_time().
  RedMilestoneTracker.get_latest_milestone_info: RedMilestoneTracker#get_latest_milestone_info().
  RedMilestoneTracker.latest_milestone: RedMilestoneTracker#latest_milestone.
  RedMilestoneTracker._format_time: RedMilestoneTracker#_format_time().
  RedMilestoneTracker: RedMilestoneTracker#
  RedMilestoneTracker.__init__: RedMilestoneTracker#__init__().
  RedMilestoneTracker.get_milestone_data: RedMilestoneTracker#get_milestone_data().
  RedMilestoneTracker.get_all_completed_milestones: RedMilestoneTracker#get_all_completed_milestones().
  RedMilestoneTracker.loaded_state_milestones_file: RedMilestoneTracker#loaded_state_milestones_file.
  RedMilestoneTracker.latest_split_time: RedMilestoneTracker#latest_split_time.
---
# Module: [`pokemon_red_env/red_milestone_tracker.py`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py)

## Classes
### `RedMilestoneTracker`
- def: [`pokemon_red_env/red_milestone_tracker.py:15`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L15)
- doc: Persistent milestone tracking system for Pokemon Red.
- signature: `class RedMilestoneTracker:`
- members:
  - `_calculate_split_time(self, milestone_id: str, timestamp: float)` — [`L138`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L138) — Calculate split time from previous milestone completion or start.
  - `_calculate_total_time(self, timestamp: float)` — [`L210`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L210) — Calculate total time from game start.
  - `_format_time(self, seconds: float)` — [`L200`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L200) — Format time in HH:MM:SS format.
  - `get_all_completed_milestones(self)` — [`L232`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L232) — Get a list of all completed milestones with their times.
  - `get_latest_milestone_info(self)` — [`L220`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L220) — Get the latest milestone information for submission logging.
  - `get_milestone_data(self, milestone_id: str)` — [`L127`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L127) — Get milestone data.
  - `is_completed(self, milestone_id: str)` — [`L123`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L123) — Check if a milestone is completed.
  - `load_from_file(self)` — [`L34`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L34) — Load milestone progress from file.
  - `load_milestones_for_state(self, state_filename: str = None)` — [`L251`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L251) — Load milestones from file, optionally with a specific state filename.
  - `mark_completed(self, milestone_id: str, timestamp: float = None, agent_step_count: int = None)` — [`L80`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L80) — Mark a milestone as completed and log split time.
  - `reset_all(self)` — [`L245`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L245) — Reset all milestones (for testing).
  - `reset_milestone(self, milestone_id: str)` — [`L131`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L131) — Reset a milestone (for testing).
  - `save_milestones_for_state(self, state_filename: str = None)` — [`L282`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L282) — Save milestones to file, optionally with a specific state filename.
  - `save_to_file(self)` — [`L66`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L66) — Save milestone progress to file.
  - `cache_dir` — [`L21`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L21)
  - `filename` — [`L27`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L27)
  - `latest_milestone` — [`L30`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L30)
  - `latest_split_time` — [`L31`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L31)
  - `loaded_state_milestones_file` — [`L28`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L28)
  - `milestones` — [`L29`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L29)
- protocol/private: `__init__`[`L18`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L18)
- uses (calls/refs, reference-scoped): [`get_cache_directory`](../utils/data_persistence/run_data_manager.md#get_cache_directory), [`logger`](red_milestone_tracker.md#logger)
- used by: [`main`](../server/app.md#main), [`get_comprehensive_state`](../server/app.md#get_comprehensive_state), [`take_action`](../server/app.md#take_action), [`milestone_tracker`](red_emulator.md#RedEmulator.milestone_tracker), [`setup_environment`](../server/app.md#setup_environment), [`mcp_get_progress_summary`](../server/app.md#mcp_get_progress_summary), [`load_state`](red_emulator.md#RedEmulator.load_state), [`test_milestone_operations`](../server/app.md#test_milestone_operations), [`check_and_update_milestones`](red_emulator.md#RedEmulator.check_and_update_milestones), [`load_checkpoint`](../server/app.md#load_checkpoint), [`reset_milestones`](../server/app.md#reset_milestones), [`save_checkpoint`](../server/app.md#save_checkpoint), [`debug_milestones`](../server/app.md#debug_milestones), [`_last_milestone_update`](red_emulator.md#RedEmulator._last_milestone_update), [`save_state`](red_emulator.md#RedEmulator.save_state), [`_check_red_milestone`](red_emulator.md#RedEmulator._check_red_milestone)  (1 test-only)

## Module values
- `logger` — [`L12`](../../../../../raw/code/continual-harness/pokemon_red_env/red_milestone_tracker.py#L12)

