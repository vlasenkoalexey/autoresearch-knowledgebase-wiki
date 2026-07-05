---
title: rd-agent — overview
type: overview
updated: 2026-07-04
---
# rd-agent — what it is and how it fits together

> Grounded code wiki for [microsoft/RD-Agent](https://github.com/microsoft/RD-Agent), pinned @ `4f9ecb0`.
> This is the *implementation* companion to the paper summary in
> [`../../sources/rd-agent.md`](../../sources/rd-agent.md) and the paper-side concept pages
> [`research-development-loop`](../../concepts/research-development-loop.md) and
> [`closed-loop-experiment-design`](../../concepts/closed-loop-experiment-design.md). Read those for *what the
> system claims and why it matters* (the six-component Research/Development split, MLE-Bench SOTA, RD-Agent(Q)'s
> quant specialization); read this for *how the code actually implements the loop*.

## In one paragraph
RD-Agent is Microsoft Research's framework for automating "data science R&D" — turning a raw dataset and a
task into a trained, evaluated solution with no human in the inner loop. The architectural bet, made concrete
in the code, is the paper's **Research → Development split**: a *Research* phase proposes and filters *what to
try next* cheaply, before a *Development* phase spends compute turning the chosen idea into runnable,
sandboxed, evaluated code. The runtime spine is a single generic async engine,
[`LoopBase`](concepts/rdagent-utils-workflow-loop.md), that every scenario subclasses by declaring an ordered
list of step methods (propose → code → run → feedback) and letting the engine drive them `while time remains`
— the direct realization of the paper's Algorithm 1. Everything flows as one object graph:
[`Experiment`, `Workspace`, and `Task`](concepts/rdagent-core-experiment.md) carry an idea plus its
implementation plus its result; a growing [`Trace`](concepts/rdagent-core-proposal.md) records every
`(hypothesis, code, score)` the loop has produced so the next proposal can condition on history. The
Development phase's code generator is **Co-STEER**, built on a generic
[evolving framework](concepts/rdagent-core-evolving_framework.md) that repeatedly proposes, runs, and refines
an implementation against [multi-evaluator feedback](concepts/rdagent-components-coder-CoSTEER-evaluators.md)
and a [RAG memory of past task/code/feedback triples](concepts/rdagent-components-coder-CoSTEER-knowledge_management.md).
A wall-clock [timer](concepts/rdagent-log-timer.md) is what makes "explore early, exploit late" real, and a
tag-addressed [logging subsystem](concepts/rdagent-log.md) durably records the whole run so it can be replayed
or inspected.

## Core architecture
```mermaid
flowchart TB
    subgraph engine["Loop engine (Algorithm 1)"]
      loop["LoopBase<br/>async step-driver, resumable"]
      timer["RDAgentTimer<br/>wall-clock budget"]
    end

    subgraph research["Research phase — what to try next"]
      expgen["ExpGen / DSTrace<br/>propose + exploration DAG"]
      trace["Trace / Hypothesis<br/>history of past attempts"]
    end

    subgraph dev["Development phase — make it real & scored"]
      evolve["EvolvingFramework<br/>Co-STEER propose/eval/refine"]
      evalr["CoSTEER Evaluators<br/>code → feedback"]
      km["CoSTEER KnowledgeMgmt<br/>RAG over task/code/feedback"]
      env["Env<br/>sandboxed execution"]
    end

    subgraph state["Shared currency & memory"]
      exp["Experiment / Workspace / Task"]
      graph["UndirectedGraph<br/>semantic + connectivity memory"]
    end

    subgraph infra["LLM & I/O plumbing"]
      backend["APIBackend<br/>hardened LLM call surface"]
      tpl["T(...).r(...)<br/>prompt templating"]
      conf["Settings<br/>env-var config"]
      log["rdagent.log<br/>tag-addressed event log"]
    end

    loop -->|"Research step"| expgen
    expgen -->|"reads history"| trace
    expgen -->|"emits"| exp
    loop -->|"Development step"| evolve
    evolve --> evalr
    evolve --> km
    evalr -->|"runs code in"| env
    evolve -->|"appends result"| exp
    exp -->|"scored round"| trace
    km --- graph
    timer -.->|"remain_time gates explore/exploit"| loop
    expgen & evolve & evalr -->|"every LLM call"| backend
    backend --- tpl
    backend --- conf
    loop & backend & evolve -->|"structured events"| log
```

## Main concepts

### The loop engine — Algorithm 1 as a generic async driver
[`LoopBase`](concepts/rdagent-utils-workflow-loop.md) is the concrete realization of the paper's Algorithm 1:
a scenario declares an ordered list of step methods and the engine runs them `while time remains`, with a
producer/consumer split (`kickoff_loop`/`execute_loop`), per-step-name semaphores for bounded concurrency,
and full session pickling so an interrupted run resumes mid-loop. Two exception classes,
`skip_loop_error` and `withdraw_loop_error`, let a step abort just its own iteration without killing the run —
essential for an unattended agent. This is the page to read for "how does an RD-Agent run actually advance?"

### The Research → Development shared currency
[`Experiment`, `FBWorkspace`, and `Task`](concepts/rdagent-core-experiment.md) are the objects that flow
between the two phases: a `Task` is an idea to implement, an `FBWorkspace` is the file-based workspace the
Development phase fills with code and runs, and an `Experiment` bundles the tasks, their implementations, and
the resulting score — the `(parents, idea, code, score)` tuple the paper's Algorithm 1 appends to its
exploration graph.

### The Research phase's proposal machinery
[`Hypothesis`, `Trace`, and ExpGen](concepts/rdagent-core-proposal.md) are the core Research abstractions:
`ExpGen` turns memory context into the next experiment, and `Trace` is the running history of past
`(hypothesis, feedback)` pairs that conditions each new proposal. The data-science scenario specializes this
into [`DSTrace` and a family of ExpGen proposers](concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md),
which is where the paper's "exploration path structuring" (chain vs. tree vs. adaptive DAG) and the
draft-vs-merge scheduling (`MCTSScheduler`, `ProbabilisticScheduler`) actually live.

### Co-STEER — the Development phase's coding agent
Co-STEER is built on a generic [evolving framework](concepts/rdagent-core-evolving_framework.md): a
propose → evaluate → refine loop over a single implementation lineage, driven by feedback rather than a
population/archive. Its judgment layer is a set of
[Co-STEER Evaluators](concepts/rdagent-components-coder-CoSTEER-evaluators.md) whose ~15 domain-specific
`evaluate()` overrides all converge on one `CoSTEERSingleFeedback` contract, aggregated in parallel by
`CoSTEERMultiEvaluator`. Its memory is
[Co-STEER Knowledge Management](concepts/rdagent-components-coder-CoSTEER-knowledge_management.md), a RAG
store over task/code/feedback triples with three distinct similarity-retrieval axes. The
[factor coder](concepts/rdagent-components-coder-factor_coder-factor.md) is the quant-specialized instance
that turns a factor hypothesis into an executed, cached DataFrame value.

### Sandboxed execution
[`Env`](concepts/rdagent-utils-env.md) is the Docker/conda-backed substrate the Development phase runs
candidate code inside: `Env.run` wraps a timeout/chmod shell shim, a cache-or-retry layer, and LLM-assisted
stdout truncation, returning a structured `EnvResult`. This is what makes running untrusted LLM-generated code
in a long unattended loop safe. Edits are applied to a workspace via
[`apply_patch`](concepts/rdagent-utils-agent-apply_patch.md), a fuzzy context-diff parser tolerant of the
imprecise diffs LLMs emit.

### Cross-iteration memory
[`UndirectedGraph`](concepts/rdagent-components-knowledge_management-graph.md) is the shared semantic +
connectivity memory substrate underneath Co-STEER's knowledge base — it supports both embedding-similarity
retrieval and graph-connectivity traversal over accumulated knowledge nodes.

### The time budget behind "explore early, exploit late"
[`RDAgentTimer`](concepts/rdagent-log-timer.md) is the wall-clock authority the loop reads: failed/retried LLM
calls get their elapsed time rebated back into the deadline, and merge-vs-explore decisions gate purely on
`remain_time() >= merge_hours`, re-evaluated every iteration. This *is* the paper's FC-Planning "dynamic
time-aware planning" — grounded in a clock read, not a step count.

### Logging, LLM plumbing, and configuration
The [`rdagent.log` facade](concepts/rdagent-log.md) and its [base types](concepts/rdagent-log-base.md) /
[logger](concepts/rdagent-log-logger.md) form a tag-addressed append-only event log (tags double as a query
index) that every stage writes through, surfaced to humans via a
[Streamlit UI](concepts/rdagent-log-ui-web.md). Every LLM call goes through the hardened
[`APIBackend`](concepts/rdagent-oai-backend-base.md) (retry, auto-continue, provider-aware backoff),
configured by [`LLMSettings`](concepts/rdagent-oai-llm_conf.md) atop the generic
[env-var config system](concepts/rdagent-core-conf.md), with prompts rendered through the
[`T(...).r(...)` templating layer](concepts/rdagent-utils-agent-tpl.md).

### Applications
The framework is instantiated as concrete apps: the
[Data-Science / MLE-Bench config](concepts/rdagent-app-data_science-conf.md) (the benchmarked scenario), an
[LLM fine-tuning config](concepts/rdagent-app-finetune-llm-conf.md), and a
[CI lint-fixing runner](concepts/rdagent-app-CI-run.md) that turns the same evolving-agent machinery on lint
errors.

## How a run flows
A single R&D iteration: [`LoopBase`](concepts/rdagent-utils-workflow-loop.md) checks the
[timer](concepts/rdagent-log-timer.md), then runs the **Research** step — an
[`ExpGen`](concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md) reads the
[`Trace`](concepts/rdagent-core-proposal.md) of past attempts and emits a new
[`Experiment`](concepts/rdagent-core-experiment.md) of `Task`s. The **Development** step hands that to
Co-STEER's [evolving framework](concepts/rdagent-core-evolving_framework.md), which drafts code (via
[templated](concepts/rdagent-utils-agent-tpl.md) [LLM calls](concepts/rdagent-oai-backend-base.md), retrieving
[similar past solutions](concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)), runs it in a
[sandboxed `Env`](concepts/rdagent-utils-env.md), and refines against
[evaluator feedback](concepts/rdagent-components-coder-CoSTEER-evaluators.md) until it passes or the round
budget is spent. The scored `Experiment` is appended back to the `Trace`, every step is
[logged](concepts/rdagent-log.md), and the loop repeats — spending its remaining budget on exploration early
and exploitation/merging late.

## Map of the wiki
- *"How does a run actually advance, and how does it resume?"* → [LoopBase](concepts/rdagent-utils-workflow-loop.md)
- *"What objects flow between Research and Development?"* → [Experiment / Workspace / Task](concepts/rdagent-core-experiment.md)
- *"How is the next experiment proposed, and how is history tracked?"* → [Hypothesis / Trace / ExpGen](concepts/rdagent-core-proposal.md) and [DSTrace + schedulers](concepts/rdagent-scenarios-data_science-proposal-exp_gen-base.md)
- *"How does Co-STEER write and refine code?"* → [evolving framework](concepts/rdagent-core-evolving_framework.md), [evaluators](concepts/rdagent-components-coder-CoSTEER-evaluators.md), [knowledge management](concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
- *"How is untrusted generated code run safely?"* → [Env](concepts/rdagent-utils-env.md)
- *"How does the time budget drive explore-vs-exploit?"* → [RDAgentTimer](concepts/rdagent-log-timer.md)
- *"How does every component call an LLM?"* → [APIBackend](concepts/rdagent-oai-backend-base.md), [templating](concepts/rdagent-utils-agent-tpl.md), [LLM settings](concepts/rdagent-oai-llm_conf.md)
- *"What is `<symbol>` exactly (signature, source line, callers)?"* → the per-module catalogs under [`catalog/`](catalog/)
- *"What's the full concept table for this repo?"* → [index.md](index.md)
- *"What does the system claim and why does it matter?"* → the paper summary [`../../sources/rd-agent.md`](../../sources/rd-agent.md) and concepts [research-development-loop](../../concepts/research-development-loop.md), [closed-loop-experiment-design](../../concepts/closed-loop-experiment-design.md)
