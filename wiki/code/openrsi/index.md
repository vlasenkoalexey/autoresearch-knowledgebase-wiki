---
slug: openrsi
commit: eab05672624b540278c8cff83a24436b99f6cc69
scip_tool: scip-python
updated: 2026-08-06
---

# openrsi internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| OpenMLE-ERL-RL-airaevo_experience | [OpenMLE-ERL-RL-airaevo_experience](concepts/OpenMLE-ERL-RL-airaevo_experience.md) | fresh |
| OpenMLE-ERL-RL-generate_mle | [OpenMLE-ERL-RL-generate_mle](concepts/OpenMLE-ERL-RL-generate_mle.md) | fresh |
| OpenMLE-ERL-RL-program_database | [OpenMLE-ERL-RL-program_database](concepts/OpenMLE-ERL-RL-program_database.md) | fresh |
| OpenMLE-ERL-RL-reward_func_utils | [OpenMLE-ERL-RL-reward_func_utils](concepts/OpenMLE-ERL-RL-reward_func_utils.md) | fresh |
| OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter | [OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter](concepts/OpenMLE-ERL-SFT-tts_search-data_produce-gap_filter.md) | fresh |
| OpenMLE-ERL-SFT-tts_search-program_database | [OpenMLE-ERL-SFT-tts_search-program_database](concepts/OpenMLE-ERL-SFT-tts_search-program_database.md) | fresh |
| OpenMLE-ERL-SFT-tts_search-services-evaluator | [OpenMLE-ERL-SFT-tts_search-services-evaluator](concepts/OpenMLE-ERL-SFT-tts_search-services-evaluator.md) | fresh |
| OpenMLE-ERL-SFT-tts_search-services-generator | [OpenMLE-ERL-SFT-tts_search-services-generator](concepts/OpenMLE-ERL-SFT-tts_search-services-generator.md) | fresh |
| OpenMLE-ERL-SFT-tts_search-services-rejection | [OpenMLE-ERL-SFT-tts_search-services-rejection](concepts/OpenMLE-ERL-SFT-tts_search-services-rejection.md) | fresh |
| OpenMLE-ERL-SFT-tts_search-services-scheduler | [OpenMLE-ERL-SFT-tts_search-services-scheduler](concepts/OpenMLE-ERL-SFT-tts_search-services-scheduler.md) | fresh |
| OpenMLE-ERL-SFT-tts_search-services-tree_search_state | [OpenMLE-ERL-SFT-tts_search-services-tree_search_state](concepts/OpenMLE-ERL-SFT-tts_search-services-tree_search_state.md) | fresh |
| OpenMLE-Evo-tts_search-airaevo_async_resources | [OpenMLE-Evo-tts_search-airaevo_async_resources](concepts/OpenMLE-Evo-tts_search-airaevo_async_resources.md) | fresh |
| OpenMLE-Evo-tts_search-eval_utils | [OpenMLE-Evo-tts_search-eval_utils](concepts/OpenMLE-Evo-tts_search-eval_utils.md) | fresh |
| OpenMLE-Evo-tts_search-program_database | [OpenMLE-Evo-tts_search-program_database](concepts/OpenMLE-Evo-tts_search-program_database.md) | fresh |
| OpenMLE-Gym-builder_core-utils-nodes | [OpenMLE-Gym-builder_core-utils-nodes](concepts/OpenMLE-Gym-builder_core-utils-nodes.md) | fresh |
| OpenMLE-Gym-openmle_gym-process_runner | [OpenMLE-Gym-openmle_gym-process_runner](concepts/OpenMLE-Gym-openmle_gym-process_runner.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [openmle-evo-max-profile](doc-concepts/openmle-evo-max-profile.md)
- [shared-action-space](doc-concepts/shared-action-space.md)
- [trainable-atomic-operators](doc-concepts/trainable-atomic-operators.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **6228** across 413 modules
- deep (concept pages): **554** (8.9%)
- catalog-only: **5674**
- represented total: **6228** (100.0%)
- classes represented: **380/380**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
