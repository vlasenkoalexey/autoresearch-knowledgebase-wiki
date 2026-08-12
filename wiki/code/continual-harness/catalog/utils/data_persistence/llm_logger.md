---
title: 'Module: utils/data_persistence/llm_logger.py'
type: catalog
provenance: extracted
module: utils/data_persistence/llm_logger.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `utils.data_persistence.llm_logger`/
symbols:
  LLMLogger.cumulative_metrics: LLMLogger#cumulative_metrics.
  get_llm_logger: get_llm_logger().
  logger: logger.
  LLMLogger: LLMLogger#
  log_llm_interaction: log_llm_interaction().
  LLMLogger.log_file: LLMLogger#log_file.
  LLMLogger.pricing: LLMLogger#pricing.
  LLMLogger.log_milestone_completion: LLMLogger#log_milestone_completion().
  LLMLogger.save_cumulative_metrics: LLMLogger#save_cumulative_metrics().
  LLMLogger.append_cli_step: LLMLogger#append_cli_step().
  LLMLogger.load_cumulative_metrics: LLMLogger#load_cumulative_metrics().
  LLMLogger.log_interaction: LLMLogger#log_interaction().
  _llm_logger: _llm_logger.
  LLMLogger.log_objective_completion: LLMLogger#log_objective_completion().
  log_llm_error: log_llm_error().
  LLMLogger._write_log_entry: LLMLogger#_write_log_entry().
  LLMLogger.save_checkpoint: LLMLogger#save_checkpoint().
  LLMLogger.add_step_tool_calls: LLMLogger#add_step_tool_calls().
  LLMLogger.get_session_summary: LLMLogger#get_session_summary().
  LLMLogger.load_checkpoint: LLMLogger#load_checkpoint().
  LLMLogger._log_session_start: LLMLogger#_log_session_start().
  setup_map_stitcher_checkpoint_integration: setup_map_stitcher_checkpoint_integration().
  LLMLogger.set_run_metadata: LLMLogger#set_run_metadata().
  log_milestone_completion: log_milestone_completion().
  log_objective_completion: log_objective_completion().
  LLMLogger.increment_action_count: LLMLogger#increment_action_count().
  LLMLogger.log_error: LLMLogger#log_error().
  LLMLogger.get_cumulative_metrics: LLMLogger#get_cumulative_metrics().
  LLMLogger.log_step_start: LLMLogger#log_step_start().
  LLMLogger.log_step_end: LLMLogger#log_step_end().
  LLMLogger.log_action: LLMLogger#log_action().
  increment_action_count: increment_action_count().
  LLMLogger.log_thinking: LLMLogger#log_thinking().
  LLMLogger.session_id: LLMLogger#session_id.
  LLMLogger._ensure_metrics_structure: LLMLogger#_ensure_metrics_structure().
  LLMLogger.log_state_snapshot: LLMLogger#log_state_snapshot().
  LLMLogger._metrics_write_enabled: LLMLogger#_metrics_write_enabled().
  setup_map_stitcher_checkpoint_integration.save_callback: setup_map_stitcher_checkpoint_integration().save_callback().
  setup_map_stitcher_checkpoint_integration.load_callback: setup_map_stitcher_checkpoint_integration().load_callback().
  LLMLogger.__init__: LLMLogger#__init__().
  LLMLogger.log_dir: LLMLogger#log_dir.
---
# Module: [`utils/data_persistence/llm_logger.py`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py)

## Classes
### `LLMLogger`
- def: [`utils/data_persistence/llm_logger.py:20`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L20) — documented in [utils-data_persistence-llm_logger](../../../concepts/utils-data_persistence-llm_logger.md)
- doc: Logger for all LLM interactions
- signature: `class LLMLogger:`
- members:
  - `__init__(self, log_dir: str = "llm_logs", session_id: Optional[str] = None)` — [`L23`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L23) — Initialize the LLM logger
  - `_ensure_metrics_structure(self)` — [`L181`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L181) — Ensure cumulative_metrics has all required fields (for loading old format).
  - `_log_session_start(self)` — [`L194`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L194) — Log session start information
  - `_metrics_write_enabled(self)` — [`L169`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L169) — Return True if this process should write cumulative metrics.
  - `_write_log_entry(self, log_entry: Dict[str, Any])` — [`L588`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L588) — Write a log entry to the log file
  - `add_step_tool_calls(self, step_number: int, tool_calls: list[Dict[str, Any]])` — [`L966`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L966) — Attach tool call parameters to a step entry in cumulative metrics.
  - `append_cli_step(self, step_number: int, token_usage: Dict[str, Any], duration: float, timestamp: float, model_info: Optional[Dict[str, Any]] = None, tool_calls: Optional[list] = None)` — [`L348`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L348) — Append one step derived from a Claude Code JSONL entry into cumulative_metrics.
  - `get_cumulative_metrics(self)` — [`L809`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L809) — Get cumulative metrics for the session
  - `get_session_summary(self)` — [`L818`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L818) — Get a summary of the current session
  - `increment_action_count(self, count: int = 1)` — [`L630`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L630) — Increment the action counter (called when buttons are actually queued)
  - `load_checkpoint(self, checkpoint_file: str = None)` — [`L1045`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1045) — Load LLM interaction history from checkpoint file
  - `load_cumulative_metrics(self, metrics_file: str = None)` — [`L884`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L884) — Load cumulative metrics from cache file
  - `log_action(self, action: str, step: int, reasoning: Optional[str] = None)` — [`L567`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L567) — Log an action taken by the agent
  - `log_error(self, interaction_type: str, prompt: str, error: str, metadata: Optional[Dict[str, Any]] = None)` — [`L471`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L471) — Log an LLM interaction error
  - `log_interaction(self, interaction_type: str, prompt: str, response: str, metadata: Optional[Dict[str, Any]] = None, duration: Optional[float] = None, model_info: Optional[Dict[str, Any]] = None, step_number: Optional[int] = None)` — [`L204`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L204) — Log a complete LLM interaction
  - `log_milestone_completion(self, milestone_id: str, step_number: int, timestamp: float = None)` — [`L640`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L640) — Log milestone completion with cumulative and split metrics
  - `log_objective_completion(self, objective_id: str, category: str, objective_index: int, step_number: int, timestamp: Optional[float] = None)` — [`L719`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L719) — Log direct objective completion with cumulative and split metrics.
  - `log_state_snapshot(self, state_data: Dict[str, Any], step: int)` — [`L539`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L539) — Log a snapshot of the game state
  - `log_step_end(self, step: int, step_type: str = "agent_step", duration: Optional[float] = None, summary: Optional[str] = None)` — [`L513`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L513) — Log the end of an agent step
  - `log_step_start(self, step: int, step_type: str = "agent_step")` — [`L496`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L496) — Log the start of an agent step
  - `log_thinking(self, text: str, interaction_type: str = "thinking", duration: float = 0, agent_step: Optional[int] = None)` — [`L600`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L600) — Log agent thinking for UI streaming (same format as log_interaction, no metrics update).
  - `save_checkpoint(self, checkpoint_file: str = None, agent_step_count: int = None)` — [`L995`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L995) — Save current LLM interaction history to checkpoint file
  - `save_cumulative_metrics(self, metrics_file: str = None)` — [`L856`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L856) — Save just the cumulative metrics to a lightweight cache file.
  - `set_run_metadata(self, metadata: Dict[str, Any], overwrite: bool = False)` — [`L947`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L947) — Set run metadata in cumulative metrics.
  - `cumulative_metrics` — [`L49`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L49) — documented in [utils-data_persistence-llm_logger](../../../concepts/utils-data_persistence-llm_logger.md)
  - `log_dir` — [`L32`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L32)
  - `log_file` — [`L43`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L43)
  - `pricing` — [`L86`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L86)
  - `session_id` — [`L42`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L42)
- uses (calls/refs, reference-scoped): [`get_cache_path`](run_data_manager.md#get_cache_path), [`logger`](llm_logger.md#logger)
- used by: [`main`](../../server/app.md#main), [`run_step`](../../agents/PokeAgent.md#PokeAgent.run_step), [`take_action`](../../server/app.md#take_action), [`_run_agent_loop`](../../run_cli.md#_run_agent_loop), [`_run_planner_loop`](../../agents/PokeAgent.md#PokeAgent._run_planner_loop), [`get_llm_logger`](llm_logger.md#get_llm_logger), [`signal_handler`](../../server/app.md#signal_handler), [`_run_battler_loop`](../../agents/PokeAgent.md#PokeAgent._run_battler_loop), [`_run_one_step_subagent`](../../agents/PokeAgent.md#PokeAgent._run_one_step_subagent), [`get_metrics`](../../server/app.md#get_metrics), [`log_llm_interaction`](llm_logger.md#log_llm_interaction), [`get_agent_thinking`](../../server/app.md#get_agent_thinking), [`update_agent_step`](../../server/app.md#update_agent_step), [`log_cli_interaction`](../agent_infrastructure/cli_agent_backends.md#ClaudeCodeBackend.log_cli_interaction), [`event_stream`](../../server/app.md#stream_agent_thinking.event_stream), [`log_cli_interaction`](../agent_infrastructure/cli_agent_backends.md#HermesCliBackend.log_cli_interaction), [`sync_llm_metrics`](../../server/app.md#sync_llm_metrics), [`update_server_metrics`](../metric_tracking/server_metrics.md#update_server_metrics), [`log_cli_interaction`](../agent_infrastructure/cli_agent_backends.md#GeminiCliBackend.log_cli_interaction), [`log_cli_interaction`](../agent_infrastructure/cli_agent_backends.md#CodexCliBackend.log_cli_interaction), [`log_llm_error`](llm_logger.md#log_llm_error), [`save_metadata`](run_data_manager.md#RunDataManager.save_metadata), [`_log_thinking`](../../agents/PokeAgent.md#PokeAgent._log_thinking), [`get_llm_logs`](../../server/app.md#get_llm_logs), [`save_agent_history`](../../server/app.md#save_agent_history), [`_sync_metrics_to_server`](../agent_infrastructure/cli_agent_backends.md#CliAgentBackend._sync_metrics_to_server), [`finalize_run`](run_data_manager.md#RunDataManager.finalize_run), [`log_milestone_completion`](llm_logger.md#log_milestone_completion), [`log_objective_completion`](llm_logger.md#log_objective_completion), [`increment_action_count`](llm_logger.md#increment_action_count)  (39 test-only)

## Functions
- `get_llm_logger()` — [`L1103`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1103) — Get the global LLM logger instance — documented in [utils-data_persistence-llm_logger](../../../concepts/utils-data_persistence-llm_logger.md)
- `increment_action_count(count: int = 1)` — [`L1164`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1164) — Convenience function to increment action count from anywhere
- `load_callback(checkpoint_data)` — [`L1124`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1124)
- `log_llm_error(interaction_type: str, prompt: str, error: str, metadata: Optional[Dict[str, Any]] = None)` — [`L1151`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1151) — Convenience function to log an LLM error
- `log_llm_interaction(interaction_type: str, prompt: str, response: str, metadata: Optional[Dict[str, Any]] = None, duration: Optional[float] = None, model_info: Optional[Dict[str, Any]] = None, step_number: Optional[int] = None)` — [`L1131`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1131) — Convenience function to log an LLM interaction
- `log_milestone_completion(milestone_id: str, step_number: int, timestamp: float = None)` — [`L1173`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1173) — Convenience function to log milestone completion
- `log_objective_completion(objective_id: str, category: str, objective_index: int, step_number: int, timestamp: Optional[float] = None)` — [`L1185`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1185) — Convenience function to log direct objective completion.
- `save_callback(checkpoint_data)` — [`L1120`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1120)
- `setup_map_stitcher_checkpoint_integration(memory_reader)` — [`L1116`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1116) — Set up map stitcher integration with checkpoint system

## Module values
- `_llm_logger` — [`L1101`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L1101)
- `logger` — [`L18`](../../../../../../raw/code/continual-harness/utils/data_persistence/llm_logger.py#L18)

