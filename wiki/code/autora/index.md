---
slug: autora
commit: fc5cc3ea213a5f097c72eeaf3a16016f8065acd5
scip_tool: scip-python
updated: 2026-07-05
---

# autora internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts
_(none synthesized; see `catalog/` for the structural index)_

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [closed-loop-research-cycle](doc-concepts/closed-loop-research-cycle.md)
- [experiment-runner-component-family](doc-concepts/experiment-runner-component-family.md)
- [experimentalist-component-family](doc-concepts/experimentalist-component-family.md)
- [state-and-delta-data-model](doc-concepts/state-and-delta-data-model.md)
- [theorist-component-family](doc-concepts/theorist-component-family.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **16** across 3 modules
- deep (concept pages): **0** (0.0%)
- catalog-only: **16**
- represented total: **16** (100.0%)
- classes represented: **0/0**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
