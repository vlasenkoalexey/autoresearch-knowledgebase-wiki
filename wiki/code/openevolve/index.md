---
slug: openevolve
commit: 39db2f6da82bea2a59f49134b7375ba57adbfb24
scip_tool: scip-python
updated: 2026-07-05
---

# openevolve internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| openevolve-api | [openevolve-api](concepts/openevolve-api.md) | fresh |
| openevolve-config | [openevolve-config](concepts/openevolve-config.md) | fresh |
| openevolve-controller | [openevolve-controller](concepts/openevolve-controller.md) | fresh |
| openevolve-database | [openevolve-database](concepts/openevolve-database.md) | fresh |
| openevolve-evaluation_result | [openevolve-evaluation_result](concepts/openevolve-evaluation_result.md) | fresh |
| openevolve-evaluator | [openevolve-evaluator](concepts/openevolve-evaluator.md) | fresh |
| openevolve-evolution_trace | [openevolve-evolution_trace](concepts/openevolve-evolution_trace.md) | fresh |
| openevolve-llm-ensemble | [openevolve-llm-ensemble](concepts/openevolve-llm-ensemble.md) | fresh |
| openevolve-llm-openai | [openevolve-llm-openai](concepts/openevolve-llm-openai.md) | fresh |
| openevolve-process_parallel | [openevolve-process_parallel](concepts/openevolve-process_parallel.md) | fresh |
| openevolve-prompt-sampler | [openevolve-prompt-sampler](concepts/openevolve-prompt-sampler.md) | fresh |
| openevolve-prompt-templates | [openevolve-prompt-templates](concepts/openevolve-prompt-templates.md) | fresh |
| openevolve-utils-code_utils | [openevolve-utils-code_utils](concepts/openevolve-utils-code_utils.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [artifacts-feedback-loop](doc-concepts/artifacts-feedback-loop.md)
- [evolve-block-markers](doc-concepts/evolve-block-markers.md)
- [reproducibility-seeding](doc-concepts/reproducibility-seeding.md)
- [system-message-design](doc-concepts/system-message-design.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **2582** across 219 modules
- deep (concept pages): **267** (10.3%)
- catalog-only: **2315**
- represented total: **2582** (100.0%)
- classes represented: **177/177**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
