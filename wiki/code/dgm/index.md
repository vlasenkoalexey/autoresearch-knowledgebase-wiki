---
slug: dgm
commit: a565fd2d1dca504ef5104a7cc0f3bdc4ab9b4fd2
scip_tool: scip-python
updated: 2026-07-05
---

# dgm internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| DGM_outer | [DGM_outer](concepts/DGM_outer.md) | fresh |
| analysis-visualize_archive | [analysis-visualize_archive](concepts/analysis-visualize_archive.md) | fresh |
| coding_agent | [coding_agent](concepts/coding_agent.md) | fresh |
| llm_withtools | [llm_withtools](concepts/llm_withtools.md) | fresh |
| polyglot-docker_build | [polyglot-docker_build](concepts/polyglot-docker_build.md) | fresh |
| prompts-self_improvement_prompt | [prompts-self_improvement_prompt](concepts/prompts-self_improvement_prompt.md) | fresh |
| self_improve_step | [self_improve_step](concepts/self_improve_step.md) | fresh |
| tools-bash | [tools-bash](concepts/tools-bash.md) | fresh |
| utils-swe_log_parsers | [utils-swe_log_parsers](concepts/utils-swe_log_parsers.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [benchmark-evaluation-swe-and-polyglot](doc-concepts/benchmark-evaluation-swe-and-polyglot.md)
- [running-the-dgm](doc-concepts/running-the-dgm.md)
- [safety-untrusted-model-code](doc-concepts/safety-untrusted-model-code.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **371** across 37 modules
- deep (concept pages): **173** (46.6%)
- catalog-only: **198**
- represented total: **371** (100.0%)
- classes represented: **10/10**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
