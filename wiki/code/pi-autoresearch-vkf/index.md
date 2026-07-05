---
slug: pi-autoresearch-vkf
commit: cd8085d9ad3a9f50260808840b773eeee0e58ef7
scip_tool: scip-python
updated: 2026-07-04
---

# pi-autoresearch-vkf internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| extensions-pi-autoresearch-vkf-autonomy.ts | [extensions-pi-autoresearch-vkf-autonomy.ts](concepts/extensions-pi-autoresearch-vkf-autonomy.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-cards.ts | [extensions-pi-autoresearch-vkf-cards.ts](concepts/extensions-pi-autoresearch-vkf-cards.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-config.ts | [extensions-pi-autoresearch-vkf-config.ts](concepts/extensions-pi-autoresearch-vkf-config.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-context_prune.ts | [extensions-pi-autoresearch-vkf-context_prune.ts](concepts/extensions-pi-autoresearch-vkf-context_prune.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-dashboard.ts | [extensions-pi-autoresearch-vkf-dashboard.ts](concepts/extensions-pi-autoresearch-vkf-dashboard.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-experiments.ts | [extensions-pi-autoresearch-vkf-experiments.ts](concepts/extensions-pi-autoresearch-vkf-experiments.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-frontmatter.ts | [extensions-pi-autoresearch-vkf-frontmatter.ts](concepts/extensions-pi-autoresearch-vkf-frontmatter.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-index.ts | [extensions-pi-autoresearch-vkf-index.ts](concepts/extensions-pi-autoresearch-vkf-index.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-paths.ts | [extensions-pi-autoresearch-vkf-paths.ts](concepts/extensions-pi-autoresearch-vkf-paths.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-progress_data.ts | [extensions-pi-autoresearch-vkf-progress_data.ts](concepts/extensions-pi-autoresearch-vkf-progress_data.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-scoring.ts | [extensions-pi-autoresearch-vkf-scoring.ts](concepts/extensions-pi-autoresearch-vkf-scoring.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-synthesis.ts | [extensions-pi-autoresearch-vkf-synthesis.ts](concepts/extensions-pi-autoresearch-vkf-synthesis.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-tree.ts | [extensions-pi-autoresearch-vkf-tree.ts](concepts/extensions-pi-autoresearch-vkf-tree.ts.md) | fresh |
| extensions-pi-autoresearch-vkf-vkf.ts | [extensions-pi-autoresearch-vkf-vkf.ts](concepts/extensions-pi-autoresearch-vkf-vkf.ts.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [benchmark-methodology](doc-concepts/benchmark-methodology.md)
- [browser-dashboard-export](doc-concepts/browser-dashboard-export.md)
- [configuration-env-vars](doc-concepts/configuration-env-vars.md)
- [skills-architecture](doc-concepts/skills-architecture.md)
- [tool-reference](doc-concepts/tool-reference.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **746** across 27 modules
- deep (concept pages): **394** (52.8%)
- catalog-only: **352**
- represented total: **746** (100.0%)
- classes represented: **72/72**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
