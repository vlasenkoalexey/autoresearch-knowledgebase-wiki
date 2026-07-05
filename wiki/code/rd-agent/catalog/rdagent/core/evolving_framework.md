---
title: 'Module: rdagent/core/evolving_framework.py'
type: catalog
provenance: extracted
module: rdagent/core/evolving_framework.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.evolving_framework`/
symbols:
  RAGStrategy.knowledgebase: RAGStrategy#knowledgebase.
  QueriedKnowledge: QueriedKnowledge#
  EvolvableSubjects: EvolvableSubjects#
  EvoStep: EvoStep#
  EvolvingStrategy: EvolvingStrategy#
  EvolvingStrategy.scen: EvolvingStrategy#scen.
  EvoStep.feedback: EvoStep#feedback.
  EvolvingStrategy.evolve_iter: EvolvingStrategy#evolve_iter().
  RAGStrategy.query: RAGStrategy#query().
  RAGStrategy.generate_knowledge: RAGStrategy#generate_knowledge().
  ASpecificEvolvableSubjects: ASpecificEvolvableSubjects.
  Knowledge: Knowledge#
  RAGStrategy: RAGStrategy#
  EvolvingKnowledgeBase: EvolvingKnowledgeBase#
  IterEvaluator.evaluate_iter: IterEvaluator#evaluate_iter().
  EvolvingKnowledgeBase.query: EvolvingKnowledgeBase#query().
  IterEvaluator.evaluate: IterEvaluator#evaluate().
  IterEvaluator: IterEvaluator#
  RAGStrategy.__init__: RAGStrategy#__init__().
  RAGStrategy.load_or_init_knowledge_base: RAGStrategy#load_or_init_knowledge_base().
  EvoStep.evolvable_subjects: EvoStep#evolvable_subjects.
  EvolvingStrategy.__init__: EvolvingStrategy#__init__().
  RAGStrategy.dump_knowledge_base: RAGStrategy#dump_knowledge_base().
  RAGStrategy.load_dumped_knowledge_base: RAGStrategy#load_dumped_knowledge_base().
  EvolvableSubjects.clone: EvolvableSubjects#clone().
  EvoStep.queried_knowledge: EvoStep#queried_knowledge.
---
# Module: [`rdagent/core/evolving_framework.py`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py)

## Classes
### `EvoStep`  ·  implements/extends Generic
- def: [`rdagent/core/evolving_framework.py:44`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L44) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
- doc: At a specific step,
- signature: `class EvoStep(Generic[ASpecificEvolvableSubjects]):`
- members:
  - `evolvable_subjects` — [`L55`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L55)
  - `feedback` — [`L58`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L58) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
  - `queried_knowledge` — [`L57`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L57)
- uses (calls/refs, reference-scoped): [`Feedback`](evaluation.md#Feedback), [`QueriedKnowledge`](evolving_framework.md#QueriedKnowledge), [`ASpecificEvolvableSubjects`](evolving_framework.md#ASpecificEvolvableSubjects)
- used by: [`responses`](../app/CI/run.md#CIEvoStr.evolve.CodeFixGroup.responses), [`multistep_evolve`](evolving_agent.md#RAGEvoAgent.multistep_evolve), [`_generate_code`](../components/coder/rl/costeer.md#RLEvolvingStrategy._generate_code), [`evolve_iter`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter), [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query), [`generate_knowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.generate_knowledge), [`multistep_evolve`](../app/CI/run.md#CIEvoAgent.multistep_evolve), [`evolve_iter`](../components/coder/rl/costeer.md#RLEvolvingStrategy.evolve_iter), [`develop`](../components/coder/factor_coder/__init__.md#FactorCoSTEER.develop), [`evolve_iter`](evolving_framework.md#EvolvingStrategy.evolve_iter), [`generate_knowledge`](evolving_framework.md#RAGStrategy.generate_knowledge), [`query`](evolving_framework.md#RAGStrategy.query), [`evolving_trace`](evolving_agent.md#RAGEvoAgent.evolving_trace), [`_get_last_fb`](../components/coder/CoSTEER/__init__.md#CoSTEER._get_last_fb), [`evaluate_iter`](evolving_agent.md#RAGEvaluator.evaluate_iter), [`evolve`](../app/CI/run.md#CIEvoStr.evolve), [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV1.query), [`generate_knowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV1.generate_knowledge)

### `EvolvableSubjects`  ·  implements/extends EvaluableObj
- def: [`rdagent/core/evolving_framework.py:33`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L33) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- doc: The target object to be evolved
- signature: `class EvolvableSubjects(EvaluableObj):`
- members:
  - `clone(self)` — [`L36`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L36)
- uses (calls/refs, reference-scoped): [`EvolvingItem`](../components/coder/CoSTEER/evolvable_subjects.md#EvolvingItem), [`Repo`](../app/CI/run.md#Repo), [`EvaluableObj`](evaluation.md#EvaluableObj)
- used by: [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query), [`component_query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.component_query), [`error_query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.error_query), [`former_trace_query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query), [`EvolvingItem`](../components/coder/CoSTEER/evolvable_subjects.md#EvolvingItem), [`_get_overall_feedback`](evolving_agent.md#RAGEvoAgent._get_overall_feedback), [`Repo`](../app/CI/run.md#Repo), [`ASpecificEvolvableSubjects`](evolving_agent.md#ASpecificEvolvableSubjects), [`EvaluableObj`](evaluation.md#EvaluableObj), [`ASpecificEvolvableSubjects`](evolving_framework.md#ASpecificEvolvableSubjects), [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV1.query)

### `EvolvingKnowledgeBase`  ·  implements/extends KnowledgeBase
- def: [`rdagent/core/evolving_framework.py:25`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L25)
- signature: `class EvolvingKnowledgeBase(KnowledgeBase):`
- members:
  - `query(self)` — [`L27`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L27)
- uses (calls/refs, reference-scoped): [`QueriedKnowledge`](evolving_framework.md#QueriedKnowledge), [`KnowledgeBase`](knowledge_base.md#KnowledgeBase), [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV1.query), [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.query)
- used by: [`KnowledgeBase`](knowledge_base.md#KnowledgeBase), [`load_or_init_knowledge_base`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.load_or_init_knowledge_base), [`__init__`](evolving_framework.md#RAGStrategy.__init__), [`load_or_init_knowledge_base`](evolving_framework.md#RAGStrategy.load_or_init_knowledge_base), [`CoSTEERKnowledgeBaseV1`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV1), [`CoSTEERKnowledgeBaseV2`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2)

### `EvolvingStrategy`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/evolving_framework.py:61`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L61)
- signature: `class EvolvingStrategy(ABC, Generic[ASpecificEvolvableSubjects]):`
- members:
  - `evolve_iter(self, evo: ASpecificEvolvableSubjects, queried_knowledge: QueriedKnowledge | None = None, evolving_trace: list[EvoStep] | None = None)` — [`L66`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L66) — The evolving trace is a list of (evolvable_subjects, feedback) ordered — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
  - `scen` — [`L63`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L63)
- protocol/private: `__init__`[`L62`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L62)
- uses (calls/refs, reference-scoped): [`Scenario`](scenario.md#Scenario), [`MultiProcessEvolvingStrategy`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`evolve_iter`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter), [`QueriedKnowledge`](evolving_framework.md#QueriedKnowledge), [`EvoStep`](evolving_framework.md#EvoStep), [`evolve_iter`](../components/coder/rl/costeer.md#RLEvolvingStrategy.evolve_iter), [`ASpecificEvolvableSubjects`](evolving_framework.md#ASpecificEvolvableSubjects), [`CIEvoStr`](../app/CI/run.md#CIEvoStr), [`RLEvolvingStrategy`](../components/coder/rl/costeer.md#RLEvolvingStrategy)
- used by: [`implement_data`](../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`multistep_evolve`](evolving_agent.md#RAGEvoAgent.multistep_evolve), [`MultiProcessEvolvingStrategy`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../components/coder/data_science/pipeline/__init__.md#PipelineMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`_generate_llamafactory_config_with_llm`](../components/coder/finetune/__init__.md#LLMFinetuneEvolvingStrategy._generate_llamafactory_config_with_llm), [`implement_one_task`](../components/coder/data_science/model/__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/ensemble/__init__.md#EnsembleMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/feature/__init__.md#FeatureMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/data_science/workflow/__init__.md#WorkflowMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../components/coder/model_coder/evolving_strategy.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`error_summary`](../components/coder/factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.error_summary), [`__init__`](../components/coder/CoSTEER/__init__.md#CoSTEER.__init__), [`__init__`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.__init__), [`__init__`](evolving_agent.md#RAGEvoAgent.__init__), [`CIEvoStr`](../app/CI/run.md#CIEvoStr), [`__init__`](evolving_agent.md#EvoAgent.__init__), [`RLEvolvingStrategy`](../components/coder/rl/costeer.md#RLEvolvingStrategy)

### `IterEvaluator`  ·  implements/extends Evaluator
- def: [`rdagent/core/evolving_framework.py:94`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L94)
- doc: Some evolving implementation (i.e. evolve_iter) will iteratively implement partial solutions before a complete final solution.
- signature: `class IterEvaluator(Evaluator):`
- members:
  - `evaluate(self, eo: EvaluableObj)` — [`L101`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L101) — Default implementation that runs evaluate_iter to completion.
  - `evaluate_iter(self)` — [`L115`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L115) — 1) It will yield a evaluation for each implement part and yield the feedback for that part.
- uses (calls/refs, reference-scoped): [`Feedback`](evaluation.md#Feedback), [`Evaluator`](evaluation.md#Evaluator), [`RAGEvaluator`](evolving_agent.md#RAGEvaluator), [`evaluate_iter`](evolving_agent.md#RAGEvaluator.evaluate_iter), [`EvaluableObj`](evaluation.md#EvaluableObj)
- used by: [`Evaluator`](evaluation.md#Evaluator), [`evaluate`](evaluation.md#Evaluator.evaluate), [`RAGEvaluator`](evolving_agent.md#RAGEvaluator)

### `Knowledge`
- def: [`rdagent/core/evolving_framework.py:17`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L17)
- signature: `class Knowledge:`
- uses (calls/refs, reference-scoped): [`CoSTEERKnowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledge)
- used by: [`generate_knowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.generate_knowledge), [`generate_knowledge`](evolving_framework.md#RAGStrategy.generate_knowledge), [`evolve`](../app/CI/run.md#CIEvoStr.evolve), [`generate_knowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV1.generate_knowledge), [`CoSTEERKnowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledge)

### `QueriedKnowledge`
- def: [`rdagent/core/evolving_framework.py:21`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L21) — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
- signature: `class QueriedKnowledge:`
- uses (calls/refs, reference-scoped): [`CoSTEERQueriedKnowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge)
- used by: [`evaluate`](../scenarios/data_science/dev/runner/eval.md#DSRunnerEvaluator.evaluate), [`evaluate`](../scenarios/finetune/train/eval.md#FTRunnerEvaluator.evaluate), [`evaluate`](../components/coder/finetune/eval.md#FTCoderEvaluator.evaluate), [`evaluate`](../components/coder/data_science/workflow/eval.md#WorkflowGeneralCaseSpecEvaluator.evaluate), [`evaluate`](../components/coder/data_science/model/eval.md#ModelGeneralCaseSpecEvaluator.evaluate), [`evaluate`](../components/coder/data_science/ensemble/eval.md#EnsembleCoSTEEREvaluator.evaluate), [`evaluate`](../components/coder/data_science/feature/eval.md#FeatureCoSTEEREvaluator.evaluate), [`evaluate`](../components/coder/finetune/eval.md#FTDataEvaluator.evaluate), [`_generate_llm_feedback`](../components/coder/finetune/eval.md#FTDataEvaluator._generate_llm_feedback), [`evaluate`](../components/coder/factor_coder/evaluators.md#FactorEvaluatorForCoder.evaluate), [`CoSTEERQueriedKnowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`evaluate`](../components/coder/model_coder/evaluators.md#ModelCoSTEEREvaluator.evaluate), [`implement_one_task`](../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`evaluate_iter`](../components/coder/CoSTEER/evaluators.md#CoSTEERMultiEvaluator.evaluate_iter), [`evolve_iter`](evolving_framework.md#EvolvingStrategy.evolve_iter), [`query`](evolving_framework.md#RAGStrategy.query), [`query`](evolving_framework.md#EvolvingKnowledgeBase.query), [`queried_knowledge`](evolving_framework.md#EvoStep.queried_knowledge)

### `RAGStrategy`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/evolving_framework.py:141`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L141)
- doc: Retrieval Augmentation Generation Strategy
- signature: `class RAGStrategy(ABC, Generic[ASpecificEvolvableSubjects]):`
- members:
  - `dump_knowledge_base(self, *args: Any, **kwargs: Any)` — [`L179`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L179)
  - `generate_knowledge(self, evolving_trace: list[EvoStep[ASpecificEvolvableSubjects]], *, return_knowledge: bool = False, **kwargs: Any)` — [`L165`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L165) — Generating new knowledge based on the evolving trace. — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
  - `load_dumped_knowledge_base(self, *args: Any, **kwargs: Any)` — [`L183`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L183) — This is to load the dumped knowledge base.
  - `load_or_init_knowledge_base(self, *args: Any, **kwargs: Any)` — [`L148`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L148)
  - `query(self, evo: ASpecificEvolvableSubjects, evolving_trace: list[EvoStep], **kwargs: Any)` — [`L156`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L156) — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
  - `knowledgebase` — [`L145`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L145) — documented in [rdagent-core-evolving_framework](../../../concepts/rdagent-core-evolving_framework.md)
- protocol/private: `__init__`[`L144`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L144)
- uses (calls/refs, reference-scoped): [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query), [`QueriedKnowledge`](evolving_framework.md#QueriedKnowledge), [`generate_knowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.generate_knowledge), [`EvoStep`](evolving_framework.md#EvoStep), [`load_dumped_knowledge_base`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.load_dumped_knowledge_base), [`ASpecificEvolvableSubjects`](evolving_framework.md#ASpecificEvolvableSubjects), [`dump_knowledge_base`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.dump_knowledge_base), [`CoSTEERRAGStrategy`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy), [`Knowledge`](evolving_framework.md#Knowledge), [`EvolvingKnowledgeBase`](evolving_framework.md#EvolvingKnowledgeBase), [`load_or_init_knowledge_base`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.load_or_init_knowledge_base), [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV1.query), [`generate_knowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV1.generate_knowledge)
- used by: [`multistep_evolve`](evolving_agent.md#RAGEvoAgent.multistep_evolve), [`query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.query), [`generate_knowledge`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.generate_knowledge), [`analyze_component`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.analyze_component), [`component_query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.component_query), [`error_query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.error_query), [`former_trace_query`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query), [`load_dumped_knowledge_base`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.load_dumped_knowledge_base), [`dump_knowledge_base`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.dump_knowledge_base), [`CoSTEERRAGStrategy`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy), [`__init__`](evolving_agent.md#RAGEvoAgent.__init__), [`analyze_error`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.analyze_error), [`__init__`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategy.__init__)

## Module values
- `ASpecificEvolvableSubjects` — [`L40`](../../../../../../raw/code/rd-agent/rdagent/core/evolving_framework.py#L40)

