---
slug: Retrodict
commit: 71672e8e5adb008360f52a61ef9e2adf91a62d89
scip_tool: scip-python
updated: 2026-08-12
---

# Retrodict internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| arc3-logwriter | [arc3-logwriter](concepts/arc3-logwriter.md) | fresh |
| arc3-plan_parser | [arc3-plan_parser](concepts/arc3-plan_parser.md) | fresh |
| arc3-runner | [arc3-runner](concepts/arc3-runner.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [context-reset-and-playbook](doc-concepts/context-reset-and-playbook.md)
- [retrodiction-methodology](doc-concepts/retrodiction-methodology.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **326** across 14 modules
- deep (concept pages): **38** (11.7%)
- catalog-only: **288**
- represented total: **326** (100.0%)
- classes represented: **23/23**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
