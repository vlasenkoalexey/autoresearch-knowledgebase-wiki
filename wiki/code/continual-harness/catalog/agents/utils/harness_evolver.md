---
title: 'Module: agents/utils/harness_evolver.py'
type: catalog
provenance: extracted
module: agents/utils/harness_evolver.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.utils.harness_evolver`/
symbols:
  HarnessEvolver._evolve_subagents: HarnessEvolver#_evolve_subagents().
  HarnessEvolver._evolve_skills: HarnessEvolver#_evolve_skills().
  HarnessEvolver._evolve_memory: HarnessEvolver#_evolve_memory().
  HarnessEvolver.evolve: HarnessEvolver#evolve().
  logger: logger.
  HarnessEvolver._save_evolution_log: HarnessEvolver#_save_evolution_log().
  HarnessEvolver.should_evolve: HarnessEvolver#should_evolve().
  HarnessEvolver.prompt_optimizer: HarnessEvolver#prompt_optimizer.
  create_harness_evolver: create_harness_evolver().
  HarnessEvolver._evolve_prompt: HarnessEvolver#_evolve_prompt().
  HarnessEvolver.text_vlm: HarnessEvolver#text_vlm.
  HarnessEvolver.evolution_log: HarnessEvolver#evolution_log.
  HarnessEvolver._parse_json_response: HarnessEvolver#_parse_json_response().
  HarnessEvolver.__init__: HarnessEvolver#__init__().
  HarnessEvolver.get_current_prompt: HarnessEvolver#get_current_prompt().
  HarnessEvolver._get_memory_store: HarnessEvolver#_get_memory_store().
  HarnessEvolver._get_skill_store: HarnessEvolver#_get_skill_store().
  HarnessEvolver._get_subagent_store: HarnessEvolver#_get_subagent_store().
  HarnessEvolver.generation: HarnessEvolver#generation.
  MIN_WARMUP_STEPS: MIN_WARMUP_STEPS.
  _ALWAYS_AVAILABLE_TOOLS: _ALWAYS_AVAILABLE_TOOLS.
  HarnessEvolver: HarnessEvolver#
  HarnessEvolver._extract_tool_failures: HarnessEvolver#_extract_tool_failures().
  EARLY_PHASE_CUTOFF: EARLY_PHASE_CUTOFF.
  EARLY_FREQUENCY: EARLY_FREQUENCY.
  STABLE_FREQUENCY: STABLE_FREQUENCY.
  HarnessEvolver.run_manager: HarnessEvolver#run_manager.
---
# Module: [`agents/utils/harness_evolver.py`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py)

## Classes
### `HarnessEvolver`
- def: [`agents/utils/harness_evolver.py:53`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L53)
- doc: Evolves all harness components: prompt, subagents, skills, memory.
- signature: `class HarnessEvolver:`
- members:
  - `_evolve_memory(self, trajectories: List[Dict[str, Any]], current_step: int)` — [`L462`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L462) — Lightweight memory curation: fill gaps and rebalance importance.
  - `_evolve_prompt(self, current_step: int, num_trajectory_steps: int)` — [`L154`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L154) — Evolve the orchestrator base prompt via PromptOptimizer.
  - `_evolve_skills(self, trajectories: List[Dict[str, Any]], current_step: int)` — [`L329`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L329) — Extract successful patterns as skills and update effectiveness.
  - `_evolve_subagents(self, trajectories: List[Dict[str, Any]], current_step: int)` — [`L198`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L198) — Analyze trajectories and create/update/retire subagents.
  - `_extract_tool_failures(self, trajectories: List[Dict[str, Any]])` — [`L166`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L166) — Extract tool failure patterns from trajectories for evolution analysis.
  - `_parse_json_response(self, response: str)` — [`L569`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L569) — Extract JSON from VLM response, handling markdown fences.
  - `_save_evolution_log(self, current_step: int, results: Dict[str, Any])` — [`L595`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L595) — Persist evolution log entry to cache.
  - `evolve(self, current_step: int, num_trajectory_steps: int = 50)` — [`L115`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L115) — Run all evolution passes and return a summary.
  - `get_current_prompt(self)` — [`L111`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L111) — Delegate to the inner PromptOptimizer.
  - `should_evolve(self, current_step: int, frequency: int)` — [`L98`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L98) — Return True if evolution should fire at this step.
  - `evolution_log` — [`L74`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L74)
  - `generation` — [`L73`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L73)
  - `prompt_optimizer` — [`L65`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L65)
  - `run_manager` — [`L71`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L71)
  - `text_vlm` — [`L70`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L70)
- protocol/private: `__init__`[`L56`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L56), `_get_memory_store`[`L82`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L82), `_get_skill_store`[`L86`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L86), `_get_subagent_store`[`L90`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L90)
- uses (calls/refs, reference-scoped): [`get_cache_path`](../../utils/data_persistence/run_data_manager.md#get_cache_path), [`add`](../../utils/stores/base_store.md#BaseStore.add), [`get_tree_overview`](../../utils/stores/base_store.md#BaseStore.get_tree_overview), [`optimize_prompt`](prompt_optimizer.md#PromptOptimizer.optimize_prompt), [`add`](../../utils/stores/memory.md#Memory.add), [`GAME_NAME`](../prompts/paths.md#GAME_NAME), [`logger`](harness_evolver.md#logger), [`update`](../../utils/stores/base_store.md#BaseStore.update), [`get_text_query`](../../utils/agent_infrastructure/vlm_backends.md#VLM.get_text_query), [`get_memory_store`](../../utils/stores/memory.md#get_memory_store), [`CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH`](../prompts/paths.md#CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH), [`get_skill_store`](../../utils/stores/skills.md#get_skill_store), [`get_subagent_store`](../../utils/stores/subagents.md#get_subagent_store), [`CONTINUAL_HARNESS_SYSTEM_PROMPT_PATH`](../prompts/paths.md#CONTINUAL_HARNESS_SYSTEM_PROMPT_PATH), [`get_recent_trajectories`](prompt_optimizer.md#PromptOptimizer.get_recent_trajectories), [`PromptOptimizer`](prompt_optimizer.md#PromptOptimizer), [`add`](../../utils/stores/subagents.md#SubagentStore.add), [`remove`](../../utils/stores/subagents.md#SubagentStore.remove), [`update`](../../utils/stores/subagents.md#SubagentStore.update), [`get_current_prompt`](prompt_optimizer.md#PromptOptimizer.get_current_prompt), [`vlm`](prompt_optimizer.md#PromptOptimizer.vlm), [`_format_trajectories_for_analysis`](prompt_optimizer.md#PromptOptimizer._format_trajectories_for_analysis), [`MIN_WARMUP_STEPS`](harness_evolver.md#MIN_WARMUP_STEPS), [`_ALWAYS_AVAILABLE_TOOLS`](harness_evolver.md#_ALWAYS_AVAILABLE_TOOLS), [`EARLY_FREQUENCY`](harness_evolver.md#EARLY_FREQUENCY), [`EARLY_PHASE_CUTOFF`](harness_evolver.md#EARLY_PHASE_CUTOFF), [`STABLE_FREQUENCY`](harness_evolver.md#STABLE_FREQUENCY)
- used by: [`run_step`](../PokeAgent.md#PokeAgent.run_step), [`harness_evolver`](../PokeAgent.md#PokeAgent.harness_evolver), [`_execute_evolve_harness`](../PokeAgent.md#PokeAgent._execute_evolve_harness), [`create_harness_evolver`](harness_evolver.md#create_harness_evolver)

## Functions
- `create_harness_evolver(vlm, run_data_manager, base_prompt_path: str = CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH, system_prompt_path: str = CONTINUAL_HARNESS_SYSTEM_PROMPT_PATH, initial_prompt_override: str | None = None)` — [`L634`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L634) — Factory function to create a HarnessEvolver instance.

## Module values
- `EARLY_FREQUENCY` — [`L32`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L32)
- `EARLY_PHASE_CUTOFF` — [`L31`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L31)
- `MIN_WARMUP_STEPS` — [`L27`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L27)
- `STABLE_FREQUENCY` — [`L33`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L33)
- `_ALWAYS_AVAILABLE_TOOLS` — [`L37`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L37)
- `logger` — [`L24`](../../../../../../raw/code/continual-harness/agents/utils/harness_evolver.py#L24)

