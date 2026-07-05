---
title: Research→Development (R&D) framework
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Research→Development (R&D) framework

## Definition
R&D-Agent's central framing splits automated data-driven R&D into two cooperating roles: **'R' (Research)** proposes new ideas — hypotheses about a model structure, a factor, or a data transformation — and **'D' (Development)** implements those ideas as runnable code and executes them for real-world feedback. The README describes the human analogue directly: an expert "proposes a hypothesis … designs experiments … implements the experiment as code … then executes the code to get feedback," and "learns from the feedback and improve[s] in the next iteration." R&D-Agent automates that propose → implement → execute → feedback → evolve cycle, and stakes its bet on *evolving* R&D capability rather than one-shot generation.

## In rd-agent (grounded)
The cycle is a concrete loop engine, not just a metaphor. The **Research** side emits a [`Hypothesis`](../catalog/rdagent/core/proposal.md#Hypothesis) via an [`ExpGen`](../catalog/rdagent/core/proposal.md#ExpGen), packaged as an [`Experiment`](../catalog/rdagent/core/experiment.md#Experiment) carrying [`Task`](../catalog/rdagent/core/experiment.md#Task)s (module `rdagent/core/proposal.py`, `rdagent/core/experiment.py`). The **Development** side implements those tasks into an [`FBWorkspace`](../catalog/rdagent/core/experiment.md#FBWorkspace) and runs it. Execution feedback returns as an [`ExperimentFeedback`](../catalog/rdagent/core/proposal.md#ExperimentFeedback) / [`HypothesisFeedback`](../catalog/rdagent/core/proposal.md#HypothesisFeedback), and the whole history accumulates in a [`Trace`](../catalog/rdagent/core/proposal.md#Trace) (see [`Trace.hist`](../catalog/rdagent/core/proposal.md#Trace.hist)). The iteration itself is driven by [`LoopBase`](../catalog/rdagent/utils/workflow/loop.md#LoopBase) — its [`LoopBase.run`](../catalog/rdagent/utils/workflow/loop.md#LoopBase.run) steps propose→code→run→feedback each cycle (module `rdagent/utils/workflow/loop.py`).

## Why it matters / when it applies
The README argues the key to "high-quality solutions lies in the ability to evolve R&D capabilities" — agents should "learn like human experts, continuously improving." That is why the framework is a persistent loop with a `Trace` rather than a single LLM call: each iteration's feedback conditions the next proposal, and the Development side uses an evolving coding strategy (Co-STEER) to repair and improve implementations that an LLM cannot get right in one shot. This framing underlies every scenario in the repo.

## Connections
- Code concepts: [utils/workflow/loop (LoopBase)](../concepts/rdagent-utils-workflow-loop.md) — the loop engine; [core/proposal (Hypothesis/Trace)](../concepts/rdagent-core-proposal.md); [core/experiment (Experiment/Task)](../concepts/rdagent-core-experiment.md); [core/evolving_framework](../concepts/rdagent-core-evolving_framework.md) and [CoSTEER evaluators](../concepts/rdagent-components-coder-CoSTEER-evaluators.md) — the evolving "D" side.
- Module catalogs: [core/proposal](../catalog/rdagent/core/proposal.md), [core/experiment](../catalog/rdagent/core/experiment.md), [utils/workflow/loop](../catalog/rdagent/utils/workflow/loop.md).
- Related doc-concepts: [scenario-catalog](scenario-catalog.md), [rdagent-cli](rdagent-cli.md), [docker-sandboxed-execution](docker-sandboxed-execution.md).

## Source
Extracted from `README.md` (kept in place).
