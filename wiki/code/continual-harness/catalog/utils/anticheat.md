---
title: 'Module: utils/anticheat.py'
type: catalog
provenance: extracted
module: utils/anticheat.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.anticheat`/
symbols:
  AntiCheatTracker.log_submission_data: AntiCheatTracker#log_submission_data().
  AntiCheatTracker.submission_logger: AntiCheatTracker#submission_logger.
  AntiCheatTracker.calculate_behavioral_metrics: AntiCheatTracker#calculate_behavioral_metrics().
  AntiCheatTracker.analyze_movement_behavior: AntiCheatTracker#analyze_movement_behavior().
  AntiCheatTracker.update_milestone: AntiCheatTracker#update_milestone().
  AntiCheatTracker.initialize_submission_log: AntiCheatTracker#initialize_submission_log().
  AntiCheatTracker.latest_milestone: AntiCheatTracker#latest_milestone.
  AntiCheatTracker.decision_times: AntiCheatTracker#decision_times.
  AntiCheatTracker.total_actions: AntiCheatTracker#total_actions.
  AntiCheatTracker.detect_milestone: AntiCheatTracker#detect_milestone().
  logger: logger.
  MILESTONES: MILESTONES.
  AntiCheatTracker.start_time: AntiCheatTracker#start_time.
  AntiCheatTracker: AntiCheatTracker#
  AntiCheatTracker.previous_position: AntiCheatTracker#previous_position.
  AntiCheatTracker.invalid_actions: AntiCheatTracker#invalid_actions.
  AntiCheatTracker.exploration_moves: AntiCheatTracker#exploration_moves.
  AntiCheatTracker.backtrack_moves: AntiCheatTracker#backtrack_moves.
  AntiCheatTracker.position_history: AntiCheatTracker#position_history.
  AntiCheatTracker.__init__: AntiCheatTracker#__init__().
  AntiCheatTracker.create_state_hash: AntiCheatTracker#create_state_hash().
---
# Module: [`utils/anticheat.py`](../../../../../raw/code/continual-harness/utils/anticheat.py)

## Classes
### `AntiCheatTracker`
- def: [`utils/anticheat.py:37`](../../../../../raw/code/continual-harness/utils/anticheat.py#L37)
- doc: Tracks anti-cheat metrics and behavioral patterns for Pokemon Emerald AI agent.
- signature: `class AntiCheatTracker:`
- members:
  - `analyze_movement_behavior(self, current_pos, previous_pos, action_taken)` — [`L106`](../../../../../raw/code/continual-harness/utils/anticheat.py#L106) — Analyze movement patterns for behavioral fingerprinting.
  - `calculate_behavioral_metrics(self)` — [`L155`](../../../../../raw/code/continual-harness/utils/anticheat.py#L155) — Calculate behavioral fingerprinting metrics.
  - `create_state_hash(self, state_data)` — [`L68`](../../../../../raw/code/continual-harness/utils/anticheat.py#L68) — Create a hash of critical game state elements for integrity verification.
  - `detect_milestone(self, location_name)` — [`L172`](../../../../../raw/code/continual-harness/utils/anticheat.py#L172) — Detect if the current location corresponds to a milestone.
  - `initialize_submission_log(self, model_name)` — [`L363`](../../../../../raw/code/continual-harness/utils/anticheat.py#L363) — Initialize submission log with header information
  - `log_submission_data(self, step, state_data, action_taken, decision_time, state_hash, manual_mode=False, milestone_override=None)` — [`L258`](../../../../../raw/code/continual-harness/utils/anticheat.py#L258) — Log structured data for anticheat verification
  - `update_milestone(self, current_location)` — [`L235`](../../../../../raw/code/continual-harness/utils/anticheat.py#L235) — Update the latest milestone based on current location
  - `backtrack_moves` — [`L49`](../../../../../raw/code/continual-harness/utils/anticheat.py#L49)
  - `decision_times` — [`L45`](../../../../../raw/code/continual-harness/utils/anticheat.py#L45)
  - `exploration_moves` — [`L48`](../../../../../raw/code/continual-harness/utils/anticheat.py#L48)
  - `invalid_actions` — [`L46`](../../../../../raw/code/continual-harness/utils/anticheat.py#L46)
  - `latest_milestone` — [`L43`](../../../../../raw/code/continual-harness/utils/anticheat.py#L43)
  - `position_history` — [`L50`](../../../../../raw/code/continual-harness/utils/anticheat.py#L50)
  - `previous_position` — [`L44`](../../../../../raw/code/continual-harness/utils/anticheat.py#L44)
  - `start_time` — [`L51`](../../../../../raw/code/continual-harness/utils/anticheat.py#L51)
  - `submission_logger` — [`L54`](../../../../../raw/code/continual-harness/utils/anticheat.py#L54)
  - `total_actions` — [`L47`](../../../../../raw/code/continual-harness/utils/anticheat.py#L47)
- protocol/private: `__init__`[`L42`](../../../../../raw/code/continual-harness/utils/anticheat.py#L42)
- uses (calls/refs, reference-scoped): [`get_cache_path`](data_persistence/run_data_manager.md#get_cache_path), [`MILESTONES`](anticheat.md#MILESTONES), [`logger`](anticheat.md#logger)
- used by: [`take_action`](../server/app.md#take_action), [`setup_environment`](../server/app.md#setup_environment)

## Module values
- `MILESTONES` — [`L12`](../../../../../raw/code/continual-harness/utils/anticheat.py#L12)
- `logger` — [`L9`](../../../../../raw/code/continual-harness/utils/anticheat.py#L9)

