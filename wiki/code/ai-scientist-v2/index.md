---
slug: ai-scientist-v2
commit: 96bd51617cfdbb494a9fc283af00fe090edfae48
scip_tool: scip-python
updated: 2026-07-04
---

# ai-scientist-v2 internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| ai_scientist-ideas-i_cant_believe_its_not_better | [ai_scientist-ideas-i_cant_believe_its_not_better](concepts/ai_scientist-ideas-i_cant_believe_its_not_better.md) | fresh |
| ai_scientist-ideas-i_cant_believe_its_not_betterrealworld | [ai_scientist-ideas-i_cant_believe_its_not_betterrealworld](concepts/ai_scientist-ideas-i_cant_believe_its_not_betterrealworld.md) | fresh |
| ai_scientist-llm | [ai_scientist-llm](concepts/ai_scientist-llm.md) | fresh |
| ai_scientist-perform_icbinb_writeup | [ai_scientist-perform_icbinb_writeup](concepts/ai_scientist-perform_icbinb_writeup.md) | fresh |
| ai_scientist-perform_ideation_temp_free | [ai_scientist-perform_ideation_temp_free](concepts/ai_scientist-perform_ideation_temp_free.md) | fresh |
| ai_scientist-treesearch-agent_manager | [ai_scientist-treesearch-agent_manager](concepts/ai_scientist-treesearch-agent_manager.md) | fresh |
| ai_scientist-treesearch-backend-utils | [ai_scientist-treesearch-backend-utils](concepts/ai_scientist-treesearch-backend-utils.md) | fresh |
| ai_scientist-treesearch-interpreter | [ai_scientist-treesearch-interpreter](concepts/ai_scientist-treesearch-interpreter.md) | fresh |
| ai_scientist-treesearch-journal | [ai_scientist-treesearch-journal](concepts/ai_scientist-treesearch-journal.md) | fresh |
| ai_scientist-treesearch-log_summarization | [ai_scientist-treesearch-log_summarization](concepts/ai_scientist-treesearch-log_summarization.md) | fresh |
| ai_scientist-treesearch-parallel_agent | [ai_scientist-treesearch-parallel_agent](concepts/ai_scientist-treesearch-parallel_agent.md) | fresh |
| ai_scientist-treesearch-utils-config | [ai_scientist-treesearch-utils-config](concepts/ai_scientist-treesearch-utils-config.md) | fresh |
| ai_scientist-treesearch-utils-metric | [ai_scientist-treesearch-utils-metric](concepts/ai_scientist-treesearch-utils-metric.md) | fresh |
| ai_scientist-utils-token_tracker | [ai_scientist-utils-token_tracker](concepts/ai_scientist-utils-token_tracker.md) | fresh |
| launch_scientist_bfts | [launch_scientist_bfts](concepts/launch_scientist_bfts.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [aide-lineage](doc-concepts/aide-lineage.md)
- [bfts-tree-search-configuration](doc-concepts/bfts-tree-search-configuration.md)
- [executing-llm-written-code](doc-concepts/executing-llm-written-code.md)
- [multi-provider-model-selection](doc-concepts/multi-provider-model-selection.md)
- [two-stage-operator-workflow](doc-concepts/two-stage-operator-workflow.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **785** across 33 modules
- deep (concept pages): **367** (46.8%)
- catalog-only: **418**
- represented total: **785** (100.0%)
- classes represented: **32/32**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
