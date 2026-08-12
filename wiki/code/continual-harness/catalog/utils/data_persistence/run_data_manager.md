---
title: 'Module: utils/data_persistence/run_data_manager.py'
type: catalog
provenance: extracted
module: utils/data_persistence/run_data_manager.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.data_persistence.run_data_manager`/
symbols:
  get_cache_path: get_cache_path().
  logger: logger.
  get_run_data_manager: get_run_data_manager().
  RunDataManager.run_dir: RunDataManager#run_dir.
  get_cache_directory: get_cache_directory().
  RunDataManager: RunDataManager#
  RunDataManager.run_id: RunDataManager#run_id.
  RunDataManager._export_bootstrap_artifacts: RunDataManager#_export_bootstrap_artifacts().
  RunDataManager.save_end_state_snapshot: RunDataManager#save_end_state_snapshot().
  initialize_run_data_manager: initialize_run_data_manager().
  RunDataManager.copy_game_state: RunDataManager#copy_game_state().
  RunDataManager.save_metadata: RunDataManager#save_metadata().
  RunDataManager.copy_memory: RunDataManager#copy_memory().
  RunDataManager.get_scratch_space_dir: RunDataManager#get_scratch_space_dir().
  RunDataManager.sync_trajectories_to_run_data: RunDataManager#sync_trajectories_to_run_data().
  RunDataManager.copy_objectives_state: RunDataManager#copy_objectives_state().
  RunDataManager.copy_map_data: RunDataManager#copy_map_data().
  RunDataManager.copy_submission_log: RunDataManager#copy_submission_log().
  RunDataManager.copy_skills: RunDataManager#copy_skills().
  RunDataManager.copy_subagents: RunDataManager#copy_subagents().
  RunDataManager.copy_frame_cache: RunDataManager#copy_frame_cache().
  RunDataManager.copy_video_recording: RunDataManager#copy_video_recording().
  RunDataManager.finalize_run: RunDataManager#finalize_run().
  RunDataManager.get_run_directory: RunDataManager#get_run_directory().
  RunDataManager.log_trajectory: RunDataManager#log_trajectory().
  RunDataManager.trajectory_step: RunDataManager#trajectory_step.
  RunDataManager.copy_llm_traces: RunDataManager#copy_llm_traces().
  get_checkpoint_llm_path: get_checkpoint_llm_path().
  _run_data_manager._run_data_manager: _run_data_manager._run_data_manager.
  RunDataManager._create_directory_structure: RunDataManager#_create_directory_structure().
  RunDataManager.copy_objectives: RunDataManager#copy_objectives().
  RunDataManager.base_dir: RunDataManager#base_dir.
  RunDataManager.create_state_snapshot: RunDataManager#create_state_snapshot().
  RunDataManager.__str__: RunDataManager#__str__().
  RunDataManager.get_prompt_evolution_dir: RunDataManager#get_prompt_evolution_dir().
  RunDataManager.get_end_state_dir: RunDataManager#get_end_state_dir().
  RunDataManager.copy_knowledge_base: RunDataManager#copy_knowledge_base().
  get_cli_workspace_dir: get_cli_workspace_dir().
  RunDataManager._determine_context: RunDataManager#_determine_context().
  RunDataManager.__init__: RunDataManager#__init__().
  cleanup_old_cache_runs: cleanup_old_cache_runs().
---
# Module: [`utils/data_persistence/run_data_manager.py`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py)

## Classes
### `RunDataManager`
- def: [`utils/data_persistence/run_data_manager.py:22`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L22)
- doc: Manages structured data collection for a single run
- signature: `class RunDataManager:`
- members:
  - `__init__(self, run_id: Optional[str] = None, base_dir: str = "run_data", run_name: Optional[str] = None, first_objective_id: Optional[str] = None, first_objective_desc: Optional[str] = None)` — [`L25`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L25) — Initialize run data manager
  - `_create_directory_structure(self)` — [`L72`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L72) — Create the standardized directory structure with 3 components:
  - `_determine_context(self, game_info: Dict[str, Any])` — [`L299`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L299) — Determine the game context from game info
  - `_export_bootstrap_artifacts(self)` — [`L449`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L449) — Create ``bootstrap/`` directories with final store state + evolved prompt.
  - `copy_frame_cache(self, frame_cache_file: Optional[str] = None)` — [`L597`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L597) — Copy frame_cache.json to end_state/frame_cache
  - `copy_game_state(self, checkpoint_state: Optional[str] = None, milestones: Optional[str] = None, maps: Optional[str] = None, memory: Optional[str] = None, skills: Optional[str] = None, subagents: Optional[str] = None)` — [`L392`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L392) — Copy game state files to run_data end_state
  - `copy_knowledge_base(self, knowledge_base_file: Optional[str] = None)` — [`L578`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L578) — Deprecated: use copy_memory() instead.
  - `copy_llm_traces(self, llm_log_file: str)` — [`L310`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L310) — Copy LLM traces from llm_logs directory to run_data prompt_evolution
  - `copy_map_data(self, map_stitcher_file: Optional[str] = None)` — [`L483`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L483) — Copy map stitcher data to run_data end_state
  - `copy_memory(self, memory_file: Optional[str] = None)` — [`L521`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L521) — Copy memory.json to agent_scratch_space
  - `copy_objectives(self, objectives_file: Optional[str] = None)` — [`L351`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L351) — Copy completed objectives to run_data agent_scratch_space
  - `copy_objectives_state(self, objectives_state_file: Optional[str] = None)` — [`L375`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L375) — Sync objectives.json from cache to agent_scratch_space.
  - `copy_skills(self, skills_file: Optional[str] = None)` — [`L542`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L542) — Copy skills.json to agent_scratch_space.
  - `copy_subagents(self, subagents_file: Optional[str] = None)` — [`L560`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L560) — Copy subagents.json to agent_scratch_space.
  - `copy_submission_log(self, submission_log: Optional[str] = None)` — [`L498`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L498) — Copy submission.log to run_data end_state
  - `copy_video_recording(self, record_enabled: bool = False)` — [`L615`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L615) — Video is saved directly to run_data/end_state/videos/ when recording is enabled.
  - `create_state_snapshot(self, game_state: Dict[str, Any])` — [`L265`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L265) — Create a simple state snapshot
  - `finalize_run(self, end_time: Optional[datetime] = None, final_metrics: Optional[Dict[str, Any]] = None)` — [`L646`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L646) — Finalize the run (metadata.json deprecated).
  - `get_end_state_dir(self)` — [`L99`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L99) — Get the end state directory
  - `get_prompt_evolution_dir(self)` — [`L95`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L95) — Get the prompt evolution directory
  - `get_run_directory(self)` — [`L662`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L662) — Get the run directory path
  - `get_scratch_space_dir(self)` — [`L103`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L103) — Get the agent scratch space directory
  - `log_trajectory(self, step: int, reasoning: str, action: Dict[str, Any], pre_state: Dict[str, Any], outcome: Optional[Dict[str, Any]] = None, llm_prompt: Optional[str] = None, llm_trace_ref: Optional[str] = None, objective_context: Optional[str] = None, **kwargs)` — [`L192`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L192) — Log a system-level trajectory entry.
  - `save_end_state_snapshot(self)` — [`L632`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L632) — Save current end-state snapshot (can be called periodically)
  - `save_metadata(self, command_args: Dict[str, Any], sys_argv: List[str], additional_info: Optional[Dict[str, Any]] = None)` — [`L107`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L107) — Save run metadata to cumulative metrics (metadata.json deprecated)
  - `sync_trajectories_to_run_data(self)` — [`L584`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L584) — Copy trajectory_history.jsonl from cache to run_data/{run_id}/.
  - `base_dir` — [`L36`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L36)
  - `run_dir` — [`L62`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L62)
  - `run_id` — [`L61`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L61)
  - `trajectory_step` — [`L68`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L68)
- protocol/private: `__str__`[`L666`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L666)
- uses (calls/refs, reference-scoped): [`get_cache_path`](run_data_manager.md#get_cache_path), [`get_llm_logger`](llm_logger.md#get_llm_logger), [`logger`](run_data_manager.md#logger), [`get_cache_directory`](run_data_manager.md#get_cache_directory), [`set_run_metadata`](llm_logger.md#LLMLogger.set_run_metadata)
- used by: [`mcp_complete_direct_objective`](../../server/app.md#mcp_complete_direct_objective), [`main`](../../server/app.md#main), [`mcp_get_game_state`](../../server/app.md#mcp_get_game_state), [`run_step`](../../agents/PokeAgent.md#PokeAgent.run_step), [`_run_planner_loop`](../../agents/PokeAgent.md#PokeAgent._run_planner_loop), [`signal_handler`](../../server/app.md#signal_handler), [`_run_battler_loop`](../../agents/PokeAgent.md#PokeAgent._run_battler_loop), [`main`](../../run_cli.md#main), [`get_run_data_manager`](run_data_manager.md#get_run_data_manager), [`_save_dynamics_objectives_backup`](../../agents/objectives/direct_objectives.md#DirectObjectiveManager._save_dynamics_objectives_backup), [`main`](../../run.md#main), [`get_cache_directory`](run_data_manager.md#get_cache_directory), [`mcp_get_progress_summary`](../../server/app.md#mcp_get_progress_summary), [`init_video_recording`](../../server/app.md#init_video_recording), [`update_agent_step`](../../server/app.md#update_agent_step), [`create_cache_backup`](backup_manager.md#create_cache_backup), [`auto_save`](../../agents/objectives/direct_objectives.md#DirectObjectiveManager.auto_save), [`initialize_run_data_manager`](run_data_manager.md#initialize_run_data_manager), [`mcp_add_memory`](../../server/app.md#mcp_add_memory), [`mcp_process_memory`](../../server/app.md#mcp_process_memory), [`mcp_process_skill`](../../server/app.md#mcp_process_skill), [`mcp_process_subagent`](../../server/app.md#mcp_process_subagent), [`_run_data_manager`](run_data_manager.md#_run_data_manager._run_data_manager)  (8 test-only)

## Functions
- `cleanup_old_cache_runs()` — [`L760`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L760) — Deprecated. No-op: CLI and other runs now use datetime_runname (no run_* prefix).
- `get_cache_directory()` — [`L703`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L703) — Get the cache directory for the current run
- `get_cache_path(relative_path: str)` — [`L727`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L727) — Get a path within the run-specific cache directory — documented in [utils-data_persistence-run_data_manager](../../../concepts/utils-data_persistence-run_data_manager.md)
- `get_checkpoint_llm_path()` — [`L748`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L748) — Get path to checkpoint_llm.txt (cache folder first, then legacy location).
- `get_cli_workspace_dir()` — [`L740`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L740) — Get the CLI agent workspace directory (inside cache for backup/restore).
- `get_run_data_manager()` — [`L674`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L674) — Get the global run data manager instance — documented in [utils-data_persistence-run_data_manager](../../../concepts/utils-data_persistence-run_data_manager.md)
- `initialize_run_data_manager(run_id: Optional[str] = None, run_name: Optional[str] = None, first_objective_id: Optional[str] = None, first_objective_desc: Optional[str] = None)` — [`L679`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L679) — Initialize the global run data manager

## Module values
- `_run_data_manager` — [`L671`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L671)
- `logger` — [`L19`](../../../../../../raw/code/continual-harness/utils/data_persistence/run_data_manager.py#L19)

