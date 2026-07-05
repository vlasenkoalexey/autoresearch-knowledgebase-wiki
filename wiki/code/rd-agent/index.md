---
slug: rd-agent
commit: 4f9ecb005881cddc08df0124a2e894c018007679
scip_tool: scip-python
updated: 2026-07-04
---

# rd-agent internals wiki

Generated, grounded wiki. Start from a concept (or an area); drill into cited symbols.
The commit pin above is the single source version for every page in this silo.

**Start here → [Overview](overview.md)** — the whole system in one page (main concepts + core diagrams + a map of the wiki).

## Concepts (deep)
| Concept | Page | Status |
|---|---|---|
| rdagent-app-CI-run | [rdagent-app-CI-run](concepts/rdagent-app-CI-run.md) | fresh |
| rdagent-app-data_science-conf | [rdagent-app-data_science-conf](concepts/rdagent-app-data_science-conf.md) | fresh |
| rdagent-app-finetune-llm-conf | [rdagent-app-finetune-llm-conf](concepts/rdagent-app-finetune-llm-conf.md) | fresh |
| rdagent-components-coder-CoSTEER-evaluators | [rdagent-components-coder-CoSTEER-evaluators](concepts/rdagent-components-coder-CoSTEER-evaluators.md) | fresh |
| rdagent-components-coder-CoSTEER-knowledge_management | [rdagent-components-coder-CoSTEER-knowledge_management](concepts/rdagent-components-coder-CoSTEER-knowledge_management.md) | fresh |
| rdagent-components-coder-factor_coder-factor | [rdagent-components-coder-factor_coder-factor](concepts/rdagent-components-coder-factor_coder-factor.md) | fresh |
| rdagent-components-knowledge_management-graph | [rdagent-components-knowledge_management-graph](concepts/rdagent-components-knowledge_management-graph.md) | fresh |
| rdagent-core-conf | [rdagent-core-conf](concepts/rdagent-core-conf.md) | fresh |
| rdagent-core-evolving_framework | [rdagent-core-evolving_framework](concepts/rdagent-core-evolving_framework.md) | fresh |
| rdagent-core-experiment | [rdagent-core-experiment](concepts/rdagent-core-experiment.md) | fresh |
| rdagent-core-proposal | [rdagent-core-proposal](concepts/rdagent-core-proposal.md) | fresh |
| rdagent-log-base | [rdagent-log-base](concepts/rdagent-log-base.md) | fresh |
| rdagent-log-logger | [rdagent-log-logger](concepts/rdagent-log-logger.md) | fresh |
| rdagent-log-timer | [rdagent-log-timer](concepts/rdagent-log-timer.md) | fresh |
| rdagent-log-ui-web | [rdagent-log-ui-web](concepts/rdagent-log-ui-web.md) | fresh |
| rdagent-log | [rdagent-log](concepts/rdagent-log.md) | fresh |
| rdagent-oai-backend-base | [rdagent-oai-backend-base](concepts/rdagent-oai-backend-base.md) | fresh |
| rdagent-oai-llm_conf | [rdagent-oai-llm_conf](concepts/rdagent-oai-llm_conf.md) | fresh |
| rdagent-oai-llm_utils | [rdagent-oai-llm_utils](concepts/rdagent-oai-llm_utils.md) | fresh |
| rdagent-scenarios-data_science-proposal-exp_gen-base | [rdagent-scenarios-data_science-proposal-exp_gen-base](concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md) | fresh |
| rdagent-utils-agent-apply_patch | [rdagent-utils-agent-apply_patch](concepts/rdagent-utils-agent-apply_patch.md) | fresh |
| rdagent-utils-agent-tpl | [rdagent-utils-agent-tpl](concepts/rdagent-utils-agent-tpl.md) | fresh |
| rdagent-utils-env | [rdagent-utils-env](concepts/rdagent-utils-env.md) | fresh |
| rdagent-utils-workflow-loop | [rdagent-utils-workflow-loop](concepts/rdagent-utils-workflow-loop.md) | fresh |

## Doc-derived concepts
Concepts extracted from the project's own docs (README / `docs/`), grounded to the symbol catalog. The source docs stay in place.
- [docker-sandboxed-execution](doc-concepts/docker-sandboxed-execution.md)
- [litellm-backend](doc-concepts/litellm-backend.md)
- [rdagent-cli](doc-concepts/rdagent-cli.md)
- [research-development-framework](doc-concepts/research-development-framework.md)
- [scenario-catalog](doc-concepts/scenario-catalog.md)
- [web-ui-trace-viewer](doc-concepts/web-ui-trace-viewer.md)

## Coverage
Two tiers: **concept pages** explain mechanisms deeply (selective); **module
catalogs** represent the rest so the whole repo is navigable. Coverage is a
set-difference over the SCIP symbol table, not a graph walk — every documentable
symbol is enumerated and represented.

- documentable symbols: **6226** across 541 modules
- deep (concept pages): **399** (6.4%)
- catalog-only: **5827**
- represented total: **6226** (100.0%)
- classes represented: **592/592**

See [`catalog/`](catalog/) for the generated per-module structural index.

## Provenance
`extracted` = from SCIP / source. `inferred` = LLM judgment, treat as such.
Design-intent dynamics are labeled; none are runtime-measured (no L4 pass run).
Callers/callees are reference-scoped (SCIP has no call role), labeled "calls/refs".
