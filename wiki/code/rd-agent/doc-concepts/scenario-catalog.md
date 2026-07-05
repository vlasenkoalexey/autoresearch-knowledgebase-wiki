---
title: Scenario catalog (the runnable R&D loops)
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Scenario catalog (the runnable R&D loops)

## Definition
The same R&D loop is instantiated across a catalog of concrete, industrial scenarios, each a runnable demo. The README groups them by domain (💹 Finance, 🩺 Medical, 🏭 General) and by role: a **🦾 Copilot** that "follows human instructions to automate repetitive tasks" versus a more autonomous **🤖 Agent** that "actively proposes ideas." Headline members: quant factor/model/joint evolution on Qlib, factor extraction from financial reports, medical model evolution, general model R&D from a paper URL, the Kaggle / general **Data Science Agent** (which leads MLE-bench as the top ML-engineering agent), and the **FT-Agent** LLM fine-tuning scenario.

## In rd-agent (grounded)
Each scenario is a distinct CLI subcommand backed by its own config and loop. The **Finance** loops map to [`fin_quant_cli`](../catalog/rdagent/app/cli.md#fin_quant_cli), [`fin_factor_cli`](../catalog/rdagent/app/cli.md#fin_factor_cli), [`fin_model_cli`](../catalog/rdagent/app/cli.md#fin_model_cli), and report-driven [`fin_factor_report_cli`](../catalog/rdagent/app/cli.md#fin_factor_report_cli). The **General model copilot** is [`general_model_cli`](../catalog/rdagent/app/cli.md#general_model_cli) (takes a paper URL). The **Data Science / Kaggle / Medical** scenarios all run through [`data_science_cli`](../catalog/rdagent/app/cli.md#data_science_cli), switched by config (`DS_SCEN`, e.g. `DataScienceScen` vs `KaggleScen`) in [`DataScienceBasePropSetting`](../catalog/rdagent/app/data_science/conf.md#DataScienceBasePropSetting) / [`DS_RD_SETTING`](../catalog/rdagent/app/data_science/conf.md#DS_RD_SETTING) (module `rdagent/app/data_science/conf.py`). The **FT-Agent** scenario is [`llm_finetune_cli`](../catalog/rdagent/app/cli.md#llm_finetune_cli), configured by [`LLMFinetunePropSetting`](../catalog/rdagent/app/finetune/llm/conf.md#LLMFinetunePropSetting) with its [`target_benchmark`](../catalog/rdagent/app/finetune/llm/conf.md#LLMFinetunePropSetting.target_benchmark) and [`base_model`](../catalog/rdagent/app/finetune/llm/conf.md#LLMFinetunePropSetting.base_model). (The specific `DataScienceScen`/`KaggleScen` scenario classes live under `rdagent/scenarios/…`, selected by the `DS_SCEN` string rather than a single symbol the README names.)

## Why it matters / when it applies
The README's claim is that "R&D is a very general scenario" — one loop, many instantiations — so the catalog is how the general framework earns concrete value (Automatic Quant Factory, Data Mining Agent, Research Copilot, Kaggle Agent, FT-Agent). Which scenario you pick determines the entrance command, the config settings, and the sandbox image; the README stresses "different scenarios vary in entrance and configuration."

## Connections
- Code concepts: [app/data_science/conf](../concepts/rdagent-app-data_science-conf.md) — the Data Science / Kaggle scenario config; [app/finetune/llm/conf](../concepts/rdagent-app-finetune-llm-conf.md) — the FT-Agent config; [core/proposal](../concepts/rdagent-core-proposal.md) — the shared propose loop; [factor_coder factor](../concepts/rdagent-components-coder-factor_coder-factor.md) — the finance factor coder.
- Module catalogs: [app/cli](../catalog/rdagent/app/cli.md), [app/data_science/conf](../catalog/rdagent/app/data_science/conf.md), [app/finetune/llm/conf](../catalog/rdagent/app/finetune/llm/conf.md).
- Related doc-concepts: [rdagent-cli](rdagent-cli.md), [research-development-framework](research-development-framework.md), [docker-sandboxed-execution](docker-sandboxed-execution.md).

## Source
Extracted from `README.md` (kept in place).
