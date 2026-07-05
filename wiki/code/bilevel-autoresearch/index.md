---
slug: bilevel-autoresearch
commit: 2010e958028fa13e5aacfe2bf73d65314ecdde65
scip_tool: scip-python
updated: 2026-07-05
---

# bilevel-autoresearch internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| core-base_mechanism_research | [core-base_mechanism_research](concepts/core-base_mechanism_research.md) | fresh |
| core-inner_loop | [core-inner_loop](concepts/core-inner_loop.md) | fresh |
| core-llm_client | [core-llm_client](concepts/core-llm_client.md) | fresh |
| core-state | [core-state](concepts/core-state.md) | fresh |
| domains-article_opt-cli | [domains-article_opt-cli](concepts/domains-article_opt-cli.md) | fresh |
| domains-article_opt-mechanism_research | [domains-article_opt-mechanism_research](concepts/domains-article_opt-mechanism_research.md) | fresh |
| domains-article_opt-outer | [domains-article_opt-outer](concepts/domains-article_opt-outer.md) | fresh |
| domains-article_opt-pipeline-base | [domains-article_opt-pipeline-base](concepts/domains-article_opt-pipeline-base.md) | fresh |
| domains-article_opt-runner | [domains-article_opt-runner](concepts/domains-article_opt-runner.md) | fresh |
| domains-train_opt-config | [domains-train_opt-config](concepts/domains-train_opt-config.md) | fresh |
| domains-train_opt-mechanism_research | [domains-train_opt-mechanism_research](concepts/domains-train_opt-mechanism_research.md) | fresh |
| domains-train_opt-mechanisms-register_adaptation | [domains-train_opt-mechanisms-register_adaptation](concepts/domains-train_opt-mechanisms-register_adaptation.md) | fresh |
| domains-train_opt-mechanisms-seasonal_cycling | [domains-train_opt-mechanisms-seasonal_cycling](concepts/domains-train_opt-mechanisms-seasonal_cycling.md) | fresh |
| domains-train_opt-outer | [domains-train_opt-outer](concepts/domains-train_opt-outer.md) | fresh |
| domains-train_opt-runner | [domains-train_opt-runner](concepts/domains-train_opt-runner.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [bilevel-architecture](doc-concepts/bilevel-architecture.md)
- [evaluator-isolation](doc-concepts/evaluator-isolation.md)
- [level-1.5-config-adjustment](doc-concepts/level-1.5-config-adjustment.md)
- [level-2-mechanism-generation](doc-concepts/level-2-mechanism-generation.md)
- [recursive-bootstrapping](doc-concepts/recursive-bootstrapping.md)
- [two-demo-domains](doc-concepts/two-demo-domains.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **5644** across 118 modules
- deep (concept pages): **236** (4.2%)
- catalog-only: **5408**
- represented total: **5644** (100.0%)
- classes represented: **427/427**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
