---
slug: rlm
commit: caf0bffa1acec17c062559433b4cd4ed92eee3d6
scip_tool: scip-python
updated: 2026-08-12
---

# rlm internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| rlm-clients-anthropic | [rlm-clients-anthropic](concepts/rlm-clients-anthropic.md) | fresh |
| rlm-clients-base_lm | [rlm-clients-base_lm](concepts/rlm-clients-base_lm.md) | fresh |
| rlm-clients-gemini | [rlm-clients-gemini](concepts/rlm-clients-gemini.md) | fresh |
| rlm-clients-openai | [rlm-clients-openai](concepts/rlm-clients-openai.md) | fresh |
| rlm-clients-portkey | [rlm-clients-portkey](concepts/rlm-clients-portkey.md) | fresh |
| rlm-core-comms_utils | [rlm-core-comms_utils](concepts/rlm-core-comms_utils.md) | fresh |
| rlm-core-lm_handler | [rlm-core-lm_handler](concepts/rlm-core-lm_handler.md) | fresh |
| rlm-core-rlm | [rlm-core-rlm](concepts/rlm-core-rlm.md) | fresh |
| rlm-core-types | [rlm-core-types](concepts/rlm-core-types.md) | fresh |
| rlm-environments-base_env | [rlm-environments-base_env](concepts/rlm-environments-base_env.md) | fresh |
| rlm-environments-daytona_repl | [rlm-environments-daytona_repl](concepts/rlm-environments-daytona_repl.md) | fresh |
| rlm-environments-docker_repl | [rlm-environments-docker_repl](concepts/rlm-environments-docker_repl.md) | fresh |
| rlm-environments-e2b_repl | [rlm-environments-e2b_repl](concepts/rlm-environments-e2b_repl.md) | fresh |
| rlm-environments-ipython_repl | [rlm-environments-ipython_repl](concepts/rlm-environments-ipython_repl.md) | fresh |
| rlm-environments-local_repl | [rlm-environments-local_repl](concepts/rlm-environments-local_repl.md) | fresh |
| rlm-environments-modal_repl | [rlm-environments-modal_repl](concepts/rlm-environments-modal_repl.md) | fresh |
| rlm-environments-prime_repl | [rlm-environments-prime_repl](concepts/rlm-environments-prime_repl.md) | fresh |
| rlm-logger-rlm_logger | [rlm-logger-rlm_logger](concepts/rlm-logger-rlm_logger.md) | fresh |
| rlm-logger-verbose | [rlm-logger-verbose](concepts/rlm-logger-verbose.md) | fresh |
| training-src-rlm_train-env | [training-src-rlm_train-env](concepts/training-src-rlm_train-env.md) | fresh |
| training-src-rlm_train-proxy | [training-src-rlm_train-proxy](concepts/training-src-rlm_train-proxy.md) | fresh |
| training-src-rlm_train-repl-subprocess | [training-src-rlm_train-repl-subprocess](concepts/training-src-rlm_train-repl-subprocess.md) | fresh |
| training-src-rlm_train-worker | [training-src-rlm_train-worker](concepts/training-src-rlm_train-worker.md) | fresh |
| visualizer-src-lib-types.ts | [visualizer-src-lib-types.ts](concepts/visualizer-src-lib-types.ts.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [codeact-bet](doc-concepts/codeact-bet.md)
- [repl-environment-taxonomy](doc-concepts/repl-environment-taxonomy.md)
- [trajectory-logging-and-visualization](doc-concepts/trajectory-logging-and-visualization.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **1753** across 121 modules
- deep (concept pages): **91** (5.2%)
- catalog-only: **1662**
- represented total: **1753** (100.0%)
- classes represented: **191/191**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
