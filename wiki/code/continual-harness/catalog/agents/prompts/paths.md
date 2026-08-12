---
title: 'Module: agents/prompts/paths.py'
type: catalog
provenance: extracted
module: agents/prompts/paths.py
status: fresh
symbol_base: scip-python python continual-harness 0.0.0 `agents.prompts.paths`/
symbols:
  GAME_NAME: GAME_NAME.
  POKEAGENT_PROMPT_PATH: POKEAGENT_PROMPT_PATH.
  CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH: CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH.
  PROMPTS_ROOT: PROMPTS_ROOT.
  CONTINUAL_HARNESS_SYSTEM_PROMPT_PATH: CONTINUAL_HARNESS_SYSTEM_PROMPT_PATH.
  render_prompt: render_prompt().
  resolve_repo_path: resolve_repo_path().
  SIMPLE_PROMPT_PATH: SIMPLE_PROMPT_PATH.
  SIMPLEST_PROMPT_PATH: SIMPLEST_PROMPT_PATH.
  game_type: game_type.
  POKEAGENT_SYSTEM_PROMPT_PATH: POKEAGENT_SYSTEM_PROMPT_PATH.
  CLI_AGENT_DIRECTIVE_PATH: CLI_AGENT_DIRECTIVE_PATH.
  _optimization_enabled_prompts: _optimization_enabled_prompts.
  _default_system_prompts: _default_system_prompts.
  _simple_prompts: _simple_prompts.
  _simplest_prompts: _simplest_prompts.
  _continual_harness_base_orchestrator_policies: _continual_harness_base_orchestrator_policies.
  _continual_harness_system_prompts: _continual_harness_system_prompts.
  GAME_NAMES: GAME_NAMES.
---
# Module: [`agents/prompts/paths.py`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py)

## Functions
- `render_prompt(content: str)` — [`L20`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L20) — Substitute {game_name} in prompt content based on GAME_TYPE env var.
- `resolve_repo_path(relative_path: str)` — [`L75`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L75) — Resolve a repository-root-relative path to an absolute Path.

## Module values
- `CLI_AGENT_DIRECTIVE_PATH` — [`L60`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L60)
- `CONTINUAL_HARNESS_BASE_ORCHESTRATOR_POLICY_PATH` — [`L71`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L71) — documented in [agents-prompts-paths](../../../concepts/agents-prompts-paths.md)
- `CONTINUAL_HARNESS_SYSTEM_PROMPT_PATH` — [`L72`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L72)
- `GAME_NAME` — [`L17`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L17)
- `GAME_NAMES` — [`L13`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L13)
- `POKEAGENT_PROMPT_PATH` — [`L52`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L52)
- `POKEAGENT_SYSTEM_PROMPT_PATH` — [`L53`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L53)
- `PROMPTS_ROOT` — [`L7`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L7)
- `SIMPLEST_PROMPT_PATH` — [`L55`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L55)
- `SIMPLE_PROMPT_PATH` — [`L54`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L54)
- `_continual_harness_base_orchestrator_policies` — [`L63`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L63)
- `_continual_harness_system_prompts` — [`L67`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L67)
- `_default_system_prompts` — [`L38`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L38)
- `_optimization_enabled_prompts` — [`L34`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L34)
- `_simple_prompts` — [`L42`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L42)
- `_simplest_prompts` — [`L47`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L47)
- `game_type` — [`L8`](../../../../../../raw/code/continual-harness/agents/prompts/paths.py#L8)

