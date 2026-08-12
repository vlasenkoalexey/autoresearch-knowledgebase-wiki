---
title: 'Module: agents/utils/prompt_optimizer.py'
type: catalog
provenance: extracted
module: agents/utils/prompt_optimizer.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.utils.prompt_optimizer`/
symbols:
  PromptOptimizer.optimize_prompt: PromptOptimizer#optimize_prompt().
  PromptOptimizer.current_base_prompt: PromptOptimizer#current_base_prompt.
  logger: logger.
  PromptOptimizer.system_prompt_content: PromptOptimizer#system_prompt_content.
  PromptOptimizer.get_recent_trajectories: PromptOptimizer#get_recent_trajectories().
  PromptOptimizer: PromptOptimizer#
  create_prompt_optimizer: create_prompt_optimizer().
  PromptOptimizer._save_optimized_prompt: PromptOptimizer#_save_optimized_prompt().
  PromptOptimizer.__init__: PromptOptimizer#__init__().
  PromptOptimizer.get_current_prompt: PromptOptimizer#get_current_prompt().
  PromptOptimizer.vlm: PromptOptimizer#vlm.
  PromptOptimizer.base_prompt_path: PromptOptimizer#base_prompt_path.
  PromptOptimizer.optimization_history: PromptOptimizer#optimization_history.
  PromptOptimizer.should_optimize: PromptOptimizer#should_optimize().
  PromptOptimizer._format_trajectories_for_analysis: PromptOptimizer#_format_trajectories_for_analysis().
  PromptOptimizer.run_manager: PromptOptimizer#run_manager.
  MIN_PROMPT_OPTIMIZATION_WARMUP_STEPS: MIN_PROMPT_OPTIMIZATION_WARMUP_STEPS.
  PromptOptimizer._get_default_prompt: PromptOptimizer#_get_default_prompt().
---
# Module: [`agents/utils/prompt_optimizer.py`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py)

## Classes
### `PromptOptimizer`
- def: [`agents/utils/prompt_optimizer.py:30`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L30)
- doc: Optimizes agent base prompt based on trajectory analysis.
- signature: `class PromptOptimizer:`
- members:
  - `__init__(self, vlm, run_data_manager, base_prompt_path: str = CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH, system_prompt_path: str = POKEAGENT_SYSTEM_PROMPT_PATH, initial_prompt_override: Optional[str] = None)` — [`L33`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L33) — Initialize the prompt optimizer.
  - `_format_trajectories_for_analysis(self, trajectories: List[Dict[str, Any]])` — [`L249`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L249) — Format trajectories into readable text for LLM analysis.
  - `_get_default_prompt(self)` — [`L87`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L87) — Returns a minimal default prompt if base file doesn't exist.
  - `_save_optimized_prompt(self, prompt: str, end_step: int, start_step: int)` — [`L321`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L321) — Save optimized prompt to run_data directory.
  - `get_current_prompt(self)` — [`L349`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L349) — Get the current active base prompt.
  - `get_recent_trajectories(self, num_steps: int = 10)` — [`L115`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L115) — Load recent trajectory data from run_data.
  - `optimize_prompt(self, current_step: int, num_trajectory_steps: int = 10)` — [`L138`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L138) — Generate optimized base prompt based on recent trajectories.
  - `should_optimize(self, current_step: int, optimization_window_length: int = 50)` — [`L103`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L103) — Check if optimization should run at this step.
  - `base_prompt_path` — [`L69`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L69)
  - `current_base_prompt` — [`L73`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L73)
  - `optimization_history` — [`L83`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L83)
  - `run_manager` — [`L67`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L67)
  - `system_prompt_content` — [`L50`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L50)
  - `vlm` — [`L61`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L61)
- uses (calls/refs, reference-scoped): [`GAME_NAME`](../prompts/paths.md#GAME_NAME), [`get_text_query`](../../utils/agent_infrastructure/vlm_backends.md#VLM.get_text_query), [`CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH`](../prompts/paths.md#CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH), [`logger`](prompt_optimizer.md#logger), [`VLM`](../../utils/agent_infrastructure/vlm_backends.md#VLM), [`render_prompt`](../prompts/paths.md#render_prompt), [`resolve_repo_path`](../prompts/paths.md#resolve_repo_path), [`resolve_trajectory_path`](../subagents/utils/trajectory_window.md#resolve_trajectory_path), [`POKEAGENT_SYSTEM_PROMPT_PATH`](../prompts/paths.md#POKEAGENT_SYSTEM_PROMPT_PATH), [`read_last_jsonl_lines`](../subagents/utils/trajectory_window.md#read_last_jsonl_lines), [`MIN_PROMPT_OPTIMIZATION_WARMUP_STEPS`](prompt_optimizer.md#MIN_PROMPT_OPTIMIZATION_WARMUP_STEPS)
- used by: [`run_step`](../PokeAgent.md#PokeAgent.run_step), [`_evolve_subagents`](harness_evolver.md#HarnessEvolver._evolve_subagents), [`_evolve_skills`](harness_evolver.md#HarnessEvolver._evolve_skills), [`_evolve_memory`](harness_evolver.md#HarnessEvolver._evolve_memory), [`evolve`](harness_evolver.md#HarnessEvolver.evolve), [`_load_base_prompt`](../PokeAgent.md#PokeAgent._load_base_prompt), [`prompt_optimizer`](harness_evolver.md#HarnessEvolver.prompt_optimizer), [`create_prompt_optimizer`](prompt_optimizer.md#create_prompt_optimizer), [`_evolve_prompt`](harness_evolver.md#HarnessEvolver._evolve_prompt), [`text_vlm`](harness_evolver.md#HarnessEvolver.text_vlm), [`get_current_prompt`](harness_evolver.md#HarnessEvolver.get_current_prompt)  (3 test-only)

## Functions
- `create_prompt_optimizer(vlm, run_data_manager, base_prompt_path: str = CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH, system_prompt_path: str = POKEAGENT_SYSTEM_PROMPT_PATH, initial_prompt_override: Optional[str] = None)` — [`L354`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L354) — Factory function to create a PromptOptimizer instance.

## Module values
- `MIN_PROMPT_OPTIMIZATION_WARMUP_STEPS` — [`L27`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L27)
- `logger` — [`L26`](../../../../../../raw/code/continual-harness/agents/utils/prompt_optimizer.py#L26)

