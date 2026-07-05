---
title: rdagent CLI entry-point surface
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# rdagent CLI entry-point surface

## Definition
`rdagent` is the single console command through which every scenario, UI, and diagnostic is launched. The README's "Run the Application" section is essentially a tour of its subcommands: `rdagent fin_quant`, `fin_factor`, `fin_model`, `fin_factor_report`, `general_model <url>`, `data_science --competition <name>`, `llm_finetune --base-model <m>`, plus operational commands `rdagent health_check`, `rdagent ui`, and `rdagent server_ui`. Each subcommand maps a demo to a fully-configured R&D loop.

## In rd-agent (grounded)
All subcommands are registered on a single Fire/Typer-style [`app`](../catalog/rdagent/app/cli.md#app) in module `rdagent/app/cli.py`. The scenario runners: [`fin_quant_cli`](../catalog/rdagent/app/cli.md#fin_quant_cli), [`fin_factor_cli`](../catalog/rdagent/app/cli.md#fin_factor_cli), [`fin_model_cli`](../catalog/rdagent/app/cli.md#fin_model_cli), [`fin_factor_report_cli`](../catalog/rdagent/app/cli.md#fin_factor_report_cli), [`general_model_cli`](../catalog/rdagent/app/cli.md#general_model_cli), [`data_science_cli`](../catalog/rdagent/app/cli.md#data_science_cli), and [`llm_finetune_cli`](../catalog/rdagent/app/cli.md#llm_finetune_cli). Operational commands: [`health_check_cli`](../catalog/rdagent/app/cli.md#health_check_cli) (Docker + port checks, gated by [`CheckEnvOption`](../catalog/rdagent/app/cli.md#CheckEnvOption)/[`CheckDockerOption`](../catalog/rdagent/app/cli.md#CheckDockerOption)/[`CheckPortsOption`](../catalog/rdagent/app/cli.md#CheckPortsOption)), [`ui`](../catalog/rdagent/app/cli.md#ui) (Streamlit log viewer), [`server_ui`](../catalog/rdagent/app/cli.md#server_ui) (Flask backend), plus [`grade_summary_cli`](../catalog/rdagent/app/cli.md#grade_summary_cli) and [`collect_info_cli`](../catalog/rdagent/app/cli.md#collect_info_cli). Most scenario runners accept the shared `step_n` / `loop_n` / `all_duration` / [`checkout`](../catalog/rdagent/app/cli.md#CheckoutOption) flags that thread down into the loop engine to bound or resume a run.

## Why it matters / when it applies
This is the user's actual entry point — the README's "Quick start" and "Run the Application" both operate entirely through it. The uniform `step_n`/`loop_n`/`checkout` flags are the practical handle on the R&D loop: they let you cap iterations, set a wall-clock budget, or resume from a checkpoint without touching code. `rdagent health_check` is called out as a *necessary* first step to validate Docker and port availability before any scenario will run.

## Connections
- Code concepts: [utils/workflow/loop](../concepts/rdagent-utils-workflow-loop.md) — where `step_n`/`loop_n`/`checkout` are honored; [app/data_science/conf](../concepts/rdagent-app-data_science-conf.md) and [app/finetune/llm/conf](../concepts/rdagent-app-finetune-llm-conf.md) — the configs a subcommand loads.
- Module catalogs: [app/cli](../catalog/rdagent/app/cli.md).
- Related doc-concepts: [scenario-catalog](scenario-catalog.md), [web-ui-trace-viewer](web-ui-trace-viewer.md), [docker-sandboxed-execution](docker-sandboxed-execution.md).

## Source
Extracted from `README.md` (kept in place).
