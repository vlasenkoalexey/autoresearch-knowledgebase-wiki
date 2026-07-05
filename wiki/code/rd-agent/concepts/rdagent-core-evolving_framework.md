---
title: The evolving framework — Co-STEER's propose/evaluate/refine engine
type: concept
provenance: mixed
concept: rdagent-core-evolving_framework
concepts: [research-development-loop, closed-loop-experiment-design]
updated: 2026-07-04
status: fresh
---

# The evolving framework — Co-STEER's propose/evaluate/refine engine

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [closed-loop-experiment-design](../../../concepts/closed-loop-experiment-design.md), [research-development-loop](../../../concepts/research-development-loop.md) across this wiki's repos.
<!-- connect:up:end -->
## Overview

Where the proposal machinery (see the proposal page) is the outer, coarse-grained Research↔Development
cycle, `rdagent.core.evolving_framework` and `rdagent.core.evolving_agent` implement a second, *nested*
closed loop that runs entirely inside Development: this is the generic engine underneath Co-STEER, the
coding agent [the RD-Agent paper](../../../sources/rd-agent.md) credits with the "efficient & iterative
debug workflow." The key design idea is a strict separation of three roles — `EvolvingStrategy` (how a
candidate implementation changes this round), `RAGStrategy` (what past knowledge informs that change),
and `Evaluator`/`RAGEvaluator` (whether the change is good enough) — coordinated by `RAGEvoAgent` through
a lockstep pair of Python **generators** rather than a simple call/return loop, so a costly evaluation
chain can be aborted the moment something fails.

## Diagram

```mermaid
sequenceDiagram
    participant Loop as RAGEvoAgent.multistep_evolve
    participant RAG as RAGStrategy (query)
    participant Strat as EvolvingStrategy (evolve_iter)
    participant Eval as RAGEvaluator (evaluate_iter)
    participant KB as knowledgebase

    loop up to max_loop rounds
        Loop->>RAG: query(evo, evolving_trace)
        RAG->>KB: read knowledgebase
        RAG-->>Loop: QueriedKnowledge
        Loop->>Strat: evolve_iter(evo, queried_knowledge, evolving_trace)
        Strat-->>Loop: yields evolved evo
        Loop->>Eval: evaluate_iter(...).send(evolved_evo)
        Eval-->>Loop: partial Feedback (or None to stop early)
        Loop->>Loop: pack EvoStep(evo, queried_knowledge, feedback)
        Loop->>RAG: generate_knowledge(evolving_trace) [if knowledge_self_gen]
        RAG->>KB: dump_knowledge_base()
    end
```

## Design rationale (why it's built this way)

[`QueriedKnowledge`](../catalog/rdagent/core/evolving_framework.md#QueriedKnowledge) is defined as
literally `class QueriedKnowledge: pass` — an intentionally empty marker base class. The real payload
lives entirely in scenario-specific subclasses:
[`CoSTEERQueriedKnowledge`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge)
adds `success_task_to_knowledge_dict`/`failed_task_info_set`, and
[`CoSTEERQueriedKnowledgeV2`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2)
extends it further.

> [!inferred] Reading the empty base class next to its heavily-populated subclasses, this looks like a
> deliberate "extension point by emptiness": the core framework commits to *when* knowledge gets queried
> (once per evolve round, before mutating) but not *what shape* that knowledge takes, leaving every
> concrete `RAGStrategy` free to define its own retrieval payload.

[`EvoStep`](../catalog/rdagent/core/evolving_framework.md#EvoStep)'s own docstring states the intent
directly: "At a specific step, based on previous trace and newly RAG knowledge `QueriedKnowledge`, the
`EvolvableSubjects` is evolved to a new one." Its three fields —
`evolvable_subjects`, `queried_knowledge`, `feedback` — are exactly the state a "hypothesize → implement
→ evaluate → feed back" cycle needs to record per round, making `EvoStep` a fine-grained,
code-refinement-level instance of the same closed-loop pattern the outer `Trace` implements at the
whole-experiment level (see the proposal page).

`evolve_iter`/`evaluate_iter` are both **generators**, coordinated by `.send()` rather than plain
function calls, and
[`evolve_iter`](../catalog/rdagent/core/evolving_framework.md#EvolvingStrategy.evolve_iter)'s own
docstring warns about the consequence directly: "the evolving process will make modifications in-place.
So the yield evo and the parameter evo are the same object!!!!" — callers cannot diff rounds by object
identity; anything that needs a "before" snapshot must copy explicitly (which is exactly what
`CoSTEER.develop`'s fallback logic does with `deepcopy`, see the experiment page). The generator protocol
also buys early termination: `RAGEvaluator.`[`evaluate_iter`](../catalog/rdagent/core/evolving_agent.md#RAGEvaluator.evaluate_iter)'s
docstring notes "sending a None feedback will stop the evaluation chain and just return the overall
feedback" — a costly per-sub-task evaluation loop can bail out after the first failure instead of always
scoring every sub-task.

## Entry points

- [`multistep_evolve`](../catalog/rdagent/core/evolving_agent.md#RAGEvoAgent.multistep_evolve) — the
  top-level generator `CoSTEER.develop` iterates over; each `yield` is one completed evolve round, giving
  the caller a chance to check timeouts or log progress between rounds.
- [`evolve_iter`](../catalog/rdagent/core/evolving_framework.md#EvolvingStrategy.evolve_iter) (abstract)
  and its concrete override
  [`evolve_iter`](../catalog/rdagent/components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter) —
  where actual code mutation happens, dispatched across sub-tasks in parallel worker processes.
- [`query`](../catalog/rdagent/core/evolving_framework.md#RAGStrategy.query) (abstract) and
  [`query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query) —
  where the current attempt is contextualized against prior successes/failures *before* the next mutation
  happens.
- [`generate_knowledge`](../catalog/rdagent/core/evolving_framework.md#RAGStrategy.generate_knowledge)
  (abstract) — where a completed evolving trace is distilled into durable `Knowledge`, available not just
  to later rounds of the *same* task but to *future* tasks that query the same knowledge base.
- [`evaluate_iter`](../catalog/rdagent/core/evolving_agent.md#RAGEvaluator.evaluate_iter) (abstract) —
  where each partial mutation is scored, running in lockstep with `evolve_iter` via the generator
  `send()` protocol described above.

## Mechanism (step-by-step)

1. **Retrieve relevant knowledge before mutating.** If `with_knowledge` is set,
   [`multistep_evolve`](../catalog/rdagent/core/evolving_agent.md#RAGEvoAgent.multistep_evolve) calls
   [`query`](../catalog/rdagent/core/evolving_framework.md#RAGStrategy.query) on the configured
   `RAGStrategy`. The concrete
   [`query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query)
   composes three independent lookups —
   [`former_trace_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query)
   (this task's own retry history),
   [`component_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.component_query)
   (semantically related components via
   [`analyze_component`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.analyze_component),
   which asks an LLM to pick relevant nodes out of a knowledge graph), and
   [`error_query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.error_query)
   (similar past errors) — merging all three into one
   [`CoSTEERQueriedKnowledgeV2`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2).

2. **Mutate only what still needs work.** The concrete
   [`evolve_iter`](../catalog/rdagent/components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter)
   first partitions `evo.sub_tasks` using the queried knowledge: tasks already present in
   `success_task_to_knowledge_dict` get their known-good code reused verbatim, tasks in
   `failed_task_info_set` are skipped, and only the remainder is actually dispatched to
   [`implement_one_task`](../catalog/rdagent/components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task)
   — meaning a "full re-evolve" round frequently does far less LLM work than its name suggests.

3. **Evaluation runs interleaved with evolution, not after it.**
   [`multistep_evolve`](../catalog/rdagent/core/evolving_agent.md#RAGEvoAgent.multistep_evolve) primes
   the evaluator generator with `next(eva_iter)`, then for every `evolved_evo` yielded by `evo_iter` sends
   it straight into `eva_iter.send(evolved_evo)` to get a partial feedback back — this is the "lockstep
   generator pair" from the diagram above, not two sequential phases.

4. **One round's outcome is packaged, not just discarded.**
   [`_get_overall_feedback`](../catalog/rdagent/core/evolving_agent.md#RAGEvoAgent._get_overall_feedback)
   drains the evaluator generator (via the `StopIteration` its final `return` raises) to get one
   aggregated `Feedback`, which `multistep_evolve` packs together with the evolved subject and the
   queried knowledge into an [`EvoStep`](../catalog/rdagent/core/evolving_framework.md#EvoStep) appended
   to [`evolving_trace`](../catalog/rdagent/core/evolving_agent.md#RAGEvoAgent.evolving_trace) — this is
   the record every subsequent round's `query`/`generate_knowledge` call reads back.

5. **Knowledge optionally compounds across rounds *and* across tasks.** When `knowledge_self_gen` is on,
   the strategy calls
   [`load_dumped_knowledge_base`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.load_dumped_knowledge_base)
   (picking up anything a concurrent worker already persisted),
   [`generate_knowledge`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.generate_knowledge)
   (mining new `Knowledge` out of the trace so far), then
   [`dump_knowledge_base`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.dump_knowledge_base) —
   all three guarded by a file lock when `enable_filelock` is set, since multiple CoSTEER instances
   (e.g. parallel Trace branches, see the proposal page) can share one on-disk knowledge base.

## Key data structures

- [`EvoStep`](../catalog/rdagent/core/evolving_framework.md#EvoStep) — `(evolvable_subjects,
  queried_knowledge, feedback)`; a `@dataclass`, the atomic unit of the evolving trace.
- [`EvolvableSubjects`](../catalog/rdagent/core/evolving_framework.md#EvolvableSubjects) — the thing
  being mutated; its only defined behavior is `clone()` (a `deepcopy`).
  [`EvolvingItem`](../catalog/rdagent/components/coder/CoSTEER/evolvable_subjects.md#EvolvingItem) is the
  bridge type Co-STEER actually uses, inheriting from *both*
  [`Experiment`](../catalog/rdagent/core/experiment.md#Experiment) and `EvolvableSubjects` — so the object
  being evolved is literally the same `Experiment` the rest of the loop works with (see the experiment
  page), not a separate copy.
- [`knowledgebase`](../catalog/rdagent/core/evolving_framework.md#RAGStrategy.knowledgebase) — set once
  in `RAGStrategy.__init__` via an abstract `load_or_init_knowledge_base(...)`; every `query`/
  `generate_knowledge`/`analyze_component` call reads or writes through this one object.
- [`CoSTEERQueriedKnowledge`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge) /
  [`CoSTEERQueriedKnowledgeV2`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledgeV2) —
  the concrete payload behind the empty `QueriedKnowledge` base, keyed by task-information strings (see
  the experiment page's note on `Task.get_task_information()`).

## Dynamics (design intent)

Parallelism here happens at two independent grains. *Within* one evolve round,
[`evolve_iter`](../catalog/rdagent/components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter)
dispatches
[`implement_one_task`](../catalog/rdagent/components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task)
across sub-tasks concurrently via a process pool sized by `RD_AGENT_SETTINGS.multi_proc_n` (see the
config page). *Across* rounds,
[`multistep_evolve`](../catalog/rdagent/core/evolving_agent.md#RAGEvoAgent.multistep_evolve) is a plain
sequential `for` loop up to `max_loop` — round *N+1* always depends on round *N*'s feedback, so rounds
cannot themselves run concurrently. The loop can also exit before `max_loop` is reached: it breaks as
soon as the packed `EvoStep`'s feedback reports `finished()`, so `max_loop` is a ceiling, not a target
round count.

## Edge cases

- Because `QueriedKnowledge`'s base class carries no fields, any code that receives one only typed as the
  base (`QueriedKnowledge | None`) has no static guarantee about what's actually inside; every real
  consumer (`evaluate(...)`, `evolve_iter(...)`) implicitly expects the CoSTEER-specific subclass and
  will fail at attribute-access time, not at a type boundary, if handed something else.
- [`query`](../catalog/rdagent/components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV1.query)
  (the V1 strategy) still exists alongside the V2 strategy this page mostly describes — Co-STEER's
  constructor picks one or the other by an `evolving_version` flag, so the RAG strategy itself is a
  swappable, versioned component, not a fixed algorithm.
- `generate_knowledge` is only invoked when `knowledge_self_gen=True`; with it off, an
  `evolving_trace` still accumulates for the current `develop()` call (rounds still see each other's
  feedback) but nothing is written to the persistent knowledge base, so later, unrelated `develop()`
  calls gain nothing from this run.

## Open questions

- [`Repo`](../catalog/rdagent/app/CI/run.md#Repo) and
  [`CIEvoAgent`](../catalog/rdagent/app/CI/run.md#CIEvoAgent.multistep_evolve) reuse this exact same
  `EvolvableSubjects`/`EvoStep`/`EvoAgent` machinery to evolve an entire code repository's lint/CI state
  rather than one Co-STEER task — a second, generic instantiation of the framework this packet's subgraph
  confirms exists, but whose relationship to the main R&D loop (is it a standalone developer tool, or
  wired into any scenario's `develop()`?) isn't visible from these symbols alone.
- The exact criteria `Feedback.finished()` uses to end a `multistep_evolve` run early aren't in this
  packet's subgraph — the mechanism (early `break` on a finished step) is clear, but which feedback
  subclasses actually override `finished()` versus rely on the default `__bool__`-based implementation
  isn't.

## See also

- [Experiment, Workspace, and Task](rdagent-core-experiment.md) — `EvolvingItem`'s other parent class,
  and the `FBWorkspace.file_dict` that `implement_one_task` actually mutates.
- [Proposal: Hypothesis, Trace, and ExpGen](rdagent-core-proposal.md) — the outer, coarser-grained closed
  loop this page's engine nests inside.
- [Configuration](rdagent-core-conf.md) — `multi_proc_n`, the setting that sizes the process pool
  `evolve_iter` dispatches sub-task implementation across.
- [RD-Agent paper summary](../../../sources/rd-agent.md) — FC-Coding-Workflow, the paper-level name for
  what this page's `multistep_evolve` implements.
- [`research-development-loop`](../../../concepts/research-development-loop.md),
  [`closed-loop-experiment-design`](../../../concepts/closed-loop-experiment-design.md) — cross-repo
  concept pages this page connects to.
