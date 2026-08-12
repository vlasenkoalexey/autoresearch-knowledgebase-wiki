---
slug: continual-harness
commit: bbab97ad73e460b7cd7c08527d10ced30cc03fbe
scip_tool: scip-python
updated: 2026-08-12
---

# continual-harness internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| agents-PokeAgent | [agents-PokeAgent](concepts/agents-PokeAgent.md) | fresh |
| agents-objectives-direct_objectives | [agents-objectives-direct_objectives](concepts/agents-objectives-direct_objectives.md) | fresh |
| agents-objectives-objective_types | [agents-objectives-objective_types](concepts/agents-objectives-objective_types.md) | fresh |
| agents-prompts-paths | [agents-prompts-paths](concepts/agents-prompts-paths.md) | fresh |
| agents-subagents-utils-registry | [agents-subagents-utils-registry](concepts/agents-subagents-utils-registry.md) | fresh |
| agents-tools-registry | [agents-tools-registry](concepts/agents-tools-registry.md) | fresh |
| agents-utils-harness_evolver | [agents-utils-harness_evolver](concepts/agents-utils-harness_evolver.md) | fresh |
| agents-vision_only_agent | [agents-vision_only_agent](concepts/agents-vision_only_agent.md) | fresh |
| pokemon_env-emerald_utils | [pokemon_env-emerald_utils](concepts/pokemon_env-emerald_utils.md) | fresh |
| pokemon_env-emulator | [pokemon_env-emulator](concepts/pokemon_env-emulator.md) | fresh |
| pokemon_env-enums | [pokemon_env-enums](concepts/pokemon_env-enums.md) | fresh |
| pokemon_env-memory_reader | [pokemon_env-memory_reader](concepts/pokemon_env-memory_reader.md) | fresh |
| pokemon_red_env-red_emulator | [pokemon_red_env-red_emulator](concepts/pokemon_red_env-red_emulator.md) | fresh |
| pokemon_red_env-red_map_reader | [pokemon_red_env-red_map_reader](concepts/pokemon_red_env-red_map_reader.md) | fresh |
| pokemon_red_env-red_memory_reader | [pokemon_red_env-red_memory_reader](concepts/pokemon_red_env-red_memory_reader.md) | fresh |
| pokemon_red_env-utils-red_metatile_behavior | [pokemon_red_env-utils-red_metatile_behavior](concepts/pokemon_red_env-utils-red_metatile_behavior.md) | fresh |
| server-app | [server-app](concepts/server-app.md) | fresh |
| utils-agent_infrastructure-cli_agent_backends | [utils-agent_infrastructure-cli_agent_backends](concepts/utils-agent_infrastructure-cli_agent_backends.md) | fresh |
| utils-agent_infrastructure-vlm_backends | [utils-agent_infrastructure-vlm_backends](concepts/utils-agent_infrastructure-vlm_backends.md) | fresh |
| utils-data_persistence-llm_logger | [utils-data_persistence-llm_logger](concepts/utils-data_persistence-llm_logger.md) | fresh |
| utils-data_persistence-run_data_manager | [utils-data_persistence-run_data_manager](concepts/utils-data_persistence-run_data_manager.md) | fresh |
| utils-mapping-map_stitcher | [utils-mapping-map_stitcher](concepts/utils-mapping-map_stitcher.md) | fresh |
| utils-state_formatter | [utils-state_formatter](concepts/utils-state_formatter.md) | fresh |
| utils-stores-base_store | [utils-stores-base_store](concepts/utils-stores-base_store.md) | fresh |
| utils-stores-memory | [utils-stores-memory](concepts/utils-stores-memory.md) | fresh |
| utils-stores-subagents | [utils-stores-subagents](concepts/utils-stores-subagents.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [immutable-base-prompt](doc-concepts/immutable-base-prompt.md)
- [reset-free-harness-evolution](doc-concepts/reset-free-harness-evolution.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **4582** across 137 modules
- deep (concept pages): **35** (0.8%)
- catalog-only: **4547**
- represented total: **4582** (100.0%)
- classes represented: **210/210**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
