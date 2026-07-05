---
title: 'Module: rdagent/core/evolving_agent.py'
type: catalog
provenance: extracted
module: rdagent/core/evolving_agent.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.evolving_agent`/
symbols:
  RAGEvoAgent.multistep_evolve: RAGEvoAgent#multistep_evolve().
  RAGEvoAgent._get_overall_feedback: RAGEvoAgent#_get_overall_feedback().
  RAGEvoAgent.evolving_trace: RAGEvoAgent#evolving_trace.
  EvoAgent: EvoAgent#
  ASpecificEvolvableSubjects: ASpecificEvolvableSubjects.
  RAGEvaluator: RAGEvaluator#
  RAGEvaluator.evaluate_iter: RAGEvaluator#evaluate_iter().
  EvoAgent.multistep_evolve: EvoAgent#multistep_evolve().
  RAGEvoAgent: RAGEvoAgent#
  RAGEvoAgent.__init__: RAGEvoAgent#__init__().
  RAGEvoAgent.rag: RAGEvoAgent#rag.
  ASpecificEvaluator: ASpecificEvaluator.
  EvoAgent.__init__: EvoAgent#__init__().
  EvoAgent.evolving_strategy: EvoAgent#evolving_strategy.
  RAGEvoAgent.stop_eval_chain_on_fail: RAGEvoAgent#stop_eval_chain_on_fail.
  EvoAgent.max_loop: EvoAgent#max_loop.
  RAGEvoAgent.with_knowledge: RAGEvoAgent#with_knowledge.
  RAGEvoAgent.knowledge_self_gen: RAGEvoAgent#knowledge_self_gen.
  RAGEvoAgent.enable_filelock: RAGEvoAgent#enable_filelock.
  RAGEvoAgent.filelock_path: RAGEvoAgent#filelock_path.
---
# Module: [`rdagent/core/evolving_agent.py`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py)

## Classes
### `EvoAgent`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/evolving_agent.py:26`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L26)
- signature: `class EvoAgent(ABC, Generic[ASpecificEvaluator, ASpecificEvolvableSubjects]):`
- members:
  - `multistep_evolve(self, evo: ASpecificEvolvableSubjects, eva: ASpecificEvaluator)` — [`L33`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L33) — yield EvolvableSubjects for caller for easier process control and logging.
  - `evolving_strategy` — [`L30`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L30)
  - `max_loop` — [`L29`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L29)
- protocol/private: `__init__`[`L28`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L28)
- uses (calls/refs, reference-scoped): [`multistep_evolve`](evolving_agent.md#RAGEvoAgent.multistep_evolve), [`EvolvingStrategy`](evolving_framework.md#EvolvingStrategy), [`multistep_evolve`](../app/CI/run.md#CIEvoAgent.multistep_evolve), [`ASpecificEvolvableSubjects`](evolving_agent.md#ASpecificEvolvableSubjects), [`RAGEvoAgent`](evolving_agent.md#RAGEvoAgent), [`ASpecificEvaluator`](evolving_agent.md#ASpecificEvaluator), [`CIEvoAgent`](../app/CI/run.md#CIEvoAgent)
- used by: [`multistep_evolve`](evolving_agent.md#RAGEvoAgent.multistep_evolve), [`multistep_evolve`](../app/CI/run.md#CIEvoAgent.multistep_evolve), [`RAGEvoAgent`](evolving_agent.md#RAGEvoAgent), [`__init__`](evolving_agent.md#RAGEvoAgent.__init__), [`__init__`](../app/CI/run.md#CIEvoAgent.__init__), [`CIEvoAgent`](../app/CI/run.md#CIEvoAgent)

### `RAGEvaluator`  ·  implements/extends IterEvaluator
- def: [`rdagent/core/evolving_agent.py:43`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L43)
- signature: `class RAGEvaluator(IterEvaluator):`
- members:
  - `evaluate_iter(self, queried_knowledge: object | None = None, evolving_trace: list[EvoStep] | None = None)` — [`L46`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L46) — 1) It will yield a evaluation for each implement part and yield the feedback for that part. — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
- uses (calls/refs, reference-scoped): [`Feedback`](evaluation.md#Feedback), [`evaluate_iter`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiEvaluator.evaluate_iter), [`CoSTEERMultiEvaluator`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`EvoStep`](evolving_framework.md#EvoStep), [`EvaluableObj`](evaluation.md#EvaluableObj), [`IterEvaluator`](evolving_framework.md#IterEvaluator)
- used by: [`multistep_evolve`](evolving_agent.md#RAGEvoAgent.multistep_evolve), [`CoSTEERMultiEvaluator`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../components/coder/CoSTEER/__init__.md#CoSTEER.__init__), [`RAGEvoAgent`](evolving_agent.md#RAGEvoAgent), [`evaluate_iter`](evolving_framework.md#IterEvaluator.evaluate_iter), [`IterEvaluator`](evolving_framework.md#IterEvaluator)

### `RAGEvoAgent`  ·  implements/extends EvoAgent, Generic
- def: [`rdagent/core/evolving_agent.py:78`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L78)
- signature: `class RAGEvoAgent(EvoAgent[RAGEvaluator, ASpecificEvolvableSubjects], Generic[ASpecificEvolvableSubjects]):`
- members:
  - `__init__(self, max_loop: int, evolving_strategy: EvolvingStrategy, rag: RAGStrategy, *, with_knowledge: bool = False, knowledge_self_gen: bool = False, enable_filelock: bool = False, filelock_path: str | None = None, stop_eval_chain_on_fail: bool = False)` — [`L80`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L80) — Initialize a Retrieval-Augmented Generation (RAG) based evolutionary agent.
  - `_get_overall_feedback(self, eva_iter: Generator[Feedback, EvaluableObj | None, Feedback], evo: EvolvableSubjects, eval_failed_happened: bool)` — [`L120`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L120) — get overall feedback from eva_iter — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
  - `multistep_evolve(self, evo: ASpecificEvolvableSubjects, eva: RAGEvaluator)` — [`L140`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L140) — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
  - `enable_filelock` — [`L116`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L116)
  - `evolving_trace` — [`L113`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L113) — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
  - `filelock_path` — [`L117`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L117)
  - `knowledge_self_gen` — [`L115`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L115)
  - `rag` — [`L112`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L112)
  - `stop_eval_chain_on_fail` — [`L118`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L118)
  - `with_knowledge` — [`L114`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L114)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../log/logger.md#RDAgentLog.info), [`log_object`](../log/logger.md#RDAgentLog.log_object), [`Feedback`](evaluation.md#Feedback), [`EvoStep`](evolving_framework.md#EvoStep), [`EvolvableSubjects`](evolving_framework.md#EvolvableSubjects), [`EvolvingStrategy`](evolving_framework.md#EvolvingStrategy), [`evolve_iter`](evolving_framework.md#EvolvingStrategy.evolve_iter), [`feedback`](evolving_framework.md#EvoStep.feedback), [`generate_knowledge`](evolving_framework.md#RAGStrategy.generate_knowledge), [`query`](evolving_framework.md#RAGStrategy.query), [`EvoAgent`](evolving_agent.md#EvoAgent), [`ASpecificEvolvableSubjects`](evolving_agent.md#ASpecificEvolvableSubjects), [`RAGEvaluator`](evolving_agent.md#RAGEvaluator), [`evaluate_iter`](evolving_agent.md#RAGEvaluator.evaluate_iter), [`EvaluableObj`](evaluation.md#EvaluableObj), [`tag`](../log/logger.md#RDAgentLog.tag), [`RAGStrategy`](evolving_framework.md#RAGStrategy), [`finished`](evaluation.md#Feedback.finished), [`__init__`](evolving_agent.md#EvoAgent.__init__), [`dump_knowledge_base`](evolving_framework.md#RAGStrategy.dump_knowledge_base), [`load_dumped_knowledge_base`](evolving_framework.md#RAGStrategy.load_dumped_knowledge_base), [`EvaluatorDidNotTerminateError`](exception.md#EvaluatorDidNotTerminateError), [`evolving_strategy`](evolving_agent.md#EvoAgent.evolving_strategy), [`max_loop`](evolving_agent.md#EvoAgent.max_loop)
- used by: [`evolve_agent`](../components/coder/CoSTEER/__init__.md#CoSTEER.evolve_agent), [`develop`](../components/coder/factor_coder/__init__.md#FactorCoSTEER.develop), [`EvoAgent`](evolving_agent.md#EvoAgent), [`_get_last_fb`](../components/coder/CoSTEER/__init__.md#CoSTEER._get_last_fb), [`multistep_evolve`](evolving_agent.md#EvoAgent.multistep_evolve)

## Module values
- `ASpecificEvaluator` — [`L22`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L22)
- `ASpecificEvolvableSubjects` — [`L23`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_agent.py#L23)

