---
title: 'Module: rdagent/components/coder/CoSTEER/knowledge_management.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/CoSTEER/knowledge_management.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.CoSTEER.knowledge_management`/CoSTEER
symbols:
  CoSTEERQueriedKnowledge: QueriedKnowledge#
  CoSTEERRAGStrategyV2.query: RAGStrategyV2#query().
  CoSTEERKnowledgeBaseV2.graph: KnowledgeBaseV2#graph.
  CoSTEERRAGStrategyV2.generate_knowledge: RAGStrategyV2#generate_knowledge().
  CoSTEERKnowledgeBaseV2.update_success_task: KnowledgeBaseV2#update_success_task().
  CoSTEERRAGStrategyV2.analyze_component: RAGStrategyV2#analyze_component().
  CoSTEERRAGStrategyV2.former_trace_query: RAGStrategyV2#former_trace_query().
  CoSTEERRAGStrategyV2.component_query: RAGStrategyV2#component_query().
  CoSTEERRAGStrategyV2.error_query: RAGStrategyV2#error_query().
  CoSTEERQueriedKnowledgeV2: QueriedKnowledgeV2#
  CoSTEERQueriedKnowledgeV1.task_to_similar_task_successful_knowledge: QueriedKnowledgeV1#task_to_similar_task_successful_knowledge.
  CoSTEERRAGStrategy.load_dumped_knowledge_base: RAGStrategy#load_dumped_knowledge_base().
  CoSTEERRAGStrategy.dump_knowledge_base: RAGStrategy#dump_knowledge_base().
  CoSTEERRAGStrategy: RAGStrategy#
  CoSTEERRAGStrategy.dump_knowledge_base_path: RAGStrategy#dump_knowledge_base_path.
  CoSTEERKnowledge.__init__: Knowledge#__init__().
  CoSTEERKnowledge.get_implementation_and_feedback_str: Knowledge#get_implementation_and_feedback_str().
  CoSTEERRAGStrategy.load_or_init_knowledge_base: RAGStrategy#load_or_init_knowledge_base().
  CoSTEERRAGStrategyV1.query: RAGStrategyV1#query().
  CoSTEERQueriedKnowledgeV2.task_to_similar_error_successful_knowledge: QueriedKnowledgeV2#task_to_similar_error_successful_knowledge.
  CoSTEERKnowledgeBaseV2.graph_get_node_by_content: KnowledgeBaseV2#graph_get_node_by_content().
  CoSTEERKnowledgeBaseV2.graph_query_by_content: KnowledgeBaseV2#graph_query_by_content().
  CoSTEERKnowledgeBaseV2.graph_query_by_node: KnowledgeBaseV2#graph_query_by_node().
  CoSTEERKnowledgeBaseV2.graph_query_by_intersection: KnowledgeBaseV2#graph_query_by_intersection().
  CoSTEERQueriedKnowledge.failed_task_info_set: QueriedKnowledge#failed_task_info_set.
  CoSTEERRAGStrategyV2.analyze_error: RAGStrategyV2#analyze_error().
  CoSTEERQueriedKnowledge.success_task_to_knowledge_dict: QueriedKnowledge#success_task_to_knowledge_dict.
  CoSTEERQueriedKnowledgeV1: QueriedKnowledgeV1#
  CoSTEERQueriedKnowledgeV1.task_to_former_failed_traces: QueriedKnowledgeV1#task_to_former_failed_traces.
  CoSTEERRAGStrategyV2.settings: RAGStrategyV2#settings.
  CoSTEERRAGStrategyV1.__init__: RAGStrategyV1#__init__().
  CoSTEERRAGStrategyV1.generate_knowledge: RAGStrategyV1#generate_knowledge().
  CoSTEERRAGStrategyV2.__init__: RAGStrategyV2#__init__().
  CoSTEERKnowledgeBaseV2.get_all_nodes_by_label: KnowledgeBaseV2#get_all_nodes_by_label().
  CoSTEERKnowledge: Knowledge#
  CoSTEERRAGStrategy.__init__: RAGStrategy#__init__().
  CoSTEERRAGStrategyV1: RAGStrategyV1#
  CoSTEERRAGStrategyV2: RAGStrategyV2#
  CoSTEERKnowledgeBaseV1: KnowledgeBaseV1#
  CoSTEERKnowledgeBaseV2: KnowledgeBaseV2#
  CoSTEERKnowledge.implementation: Knowledge#implementation.
  CoSTEERRAGStrategyV2.current_generated_trace_count: RAGStrategyV2#current_generated_trace_count.
  CoSTEERKnowledgeBaseV1.implementation_trace: KnowledgeBaseV1#implementation_trace.
  CoSTEERKnowledgeBaseV1.task_to_embedding: KnowledgeBaseV1#task_to_embedding.
  CoSTEERKnowledgeBaseV1.query: KnowledgeBaseV1#query().
  CoSTEERKnowledgeBaseV2.working_trace_error_analysis: KnowledgeBaseV2#working_trace_error_analysis.
  CoSTEERKnowledgeBaseV2.node_to_implementation_knowledge_dict: KnowledgeBaseV2#node_to_implementation_knowledge_dict.
  CoSTEERKnowledge.feedback: Knowledge#feedback.
  CoSTEERQueriedKnowledge.__init__: QueriedKnowledge#__init__().
  CoSTEERQueriedKnowledgeV1.__init__: QueriedKnowledgeV1#__init__().
  CoSTEERKnowledgeBaseV2.working_trace_knowledge: KnowledgeBaseV2#working_trace_knowledge.
  CoSTEERKnowledgeBaseV2.task_to_component_nodes: KnowledgeBaseV2#task_to_component_nodes.
  CoSTEERKnowledge.target_task: Knowledge#target_task.
  CoSTEERKnowledgeBaseV1.__init__: KnowledgeBaseV1#__init__().
  CoSTEERKnowledgeBaseV1.success_task_info_set: KnowledgeBaseV1#success_task_info_set.
  CoSTEERRAGStrategyV1.current_generated_trace_count: RAGStrategyV1#current_generated_trace_count.
  CoSTEERRAGStrategyV1.settings: RAGStrategyV1#settings.
  CoSTEERQueriedKnowledgeV2.__init__: QueriedKnowledgeV2#__init__().
  CoSTEERKnowledgeBaseV2.__init__: KnowledgeBaseV2#__init__().
  CoSTEERKnowledgeBaseV2.success_task_to_knowledge_dict: KnowledgeBaseV2#success_task_to_knowledge_dict.
  CoSTEERKnowledgeBaseV2.query: KnowledgeBaseV2#query().
---
# Module: [`rdagent/components/coder/CoSTEER/knowledge_management.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py)

## Classes
### `CoSTEERKnowledge`  ·  implements/extends Knowledge
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:36`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L36)
- signature: `class CoSTEERKnowledge(Knowledge):`
- members:
  - `get_implementation_and_feedback_str(self)` — [`L47`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L47)
  - `feedback` — [`L45`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L45)
  - `implementation` — [`L44`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L44)
  - `target_task` — [`L43`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L43)
- protocol/private: `__init__`[`L37`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L37)
- uses (calls/refs, reference-scoped): [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`Task`](../../../core/experiment.md#Task), [`Feedback`](../../../core/evaluation.md#Feedback), [`all_codes`](../../../core/experiment.md#FBWorkspace.all_codes), [`Knowledge`](../../../core/evolving_framework.md#Knowledge), [`copy`](../../../core/experiment.md#FBWorkspace.copy)
- used by: [`generate_knowledge`](knowledge_management.md#CoSTEERRAGStrategyV2.generate_knowledge), [`Knowledge`](../../../core/evolving_framework.md#Knowledge), [`implementation_trace`](knowledge_management.md#CoSTEERKnowledgeBaseV1.implementation_trace)

### `CoSTEERKnowledgeBaseV1`
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:140`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L140)
- members:
  - `query(self)` — [`L148`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L148) — Query the knowledge base to get the queried knowledge. So far is handled in RAG strategy.
  - `implementation_trace` — [`L142`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L142)
  - `success_task_info_set` — [`L143`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L143)
  - `task_to_embedding` — [`L145`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L145)
- protocol/private: `__init__`[`L141`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L141)
- uses (calls/refs, reference-scoped): [`CoSTEERQueriedKnowledge`](knowledge_management.md#CoSTEERQueriedKnowledge), [`EvolvingKnowledgeBase`](../../../core/evolving_framework.md#EvolvingKnowledgeBase), [`__init__`](../../../core/knowledge_base.md#KnowledgeBase.__init__), [`CoSTEERKnowledge`](knowledge_management.md#CoSTEERKnowledge)
- used by: [`load_or_init_knowledge_base`](knowledge_management.md#CoSTEERRAGStrategy.load_or_init_knowledge_base), [`query`](../../../core/evolving_framework.md#EvolvingKnowledgeBase.query)

### `CoSTEERKnowledgeBaseV2`
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:852`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L852)
- members:
  - `__init__(self, init_component_list=None, path: str | Path = None)` — [`L853`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L853) — Load knowledge, offer brief information of knowledge and common handle interfaces
  - `get_all_nodes_by_label(self, label: str)` — [`L881`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L881)
  - `graph_get_node_by_content(self, content: str)` — [`L929`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L929) — documented in [rdagent-components-knowledge_management-graph](../../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `graph_query_by_content(self, content: Union[str, list[str]], topk_k: int = 5, step: int = 1, constraint_labels: list[str] = None, constraint_node: UndirectedNode = None, similarity_threshold: float = 0, constraint_distance: float = 0, block: bool = False)` — [`L932`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L932) — search graph by content similarity and connection relationship, return empty list if nodes' chain without node — documented in [rdagent-components-knowledge_management-graph](../../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `graph_query_by_intersection(self, nodes: list[UndirectedNode], steps: int = 1, constraint_labels: list[str] = None, output_intersection_origin: bool = False)` — [`L1009`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L1009) — search graph by node intersection, node intersected by a higher frequency has a prior order in the list — documented in [rdagent-components-knowledge_management-graph](../../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `graph_query_by_node(self, node: UndirectedNode, step: int = 1, constraint_labels: list[str] = None, constraint_node: UndirectedNode = None, constraint_distance: float = 0, block: bool = False)` — [`L974`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L974) — search graph by connection, return empty list if nodes' chain without node near to constraint_node — documented in [rdagent-components-knowledge_management-graph](../../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `query(self)` — [`L926`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L926)
  - `update_success_task(self, success_task_info: str)` — [`L884`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L884) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `graph` — [`L857`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L857) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `node_to_implementation_knowledge_dict` — [`L876`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L876)
  - `success_task_to_knowledge_dict` — [`L873`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L873)
  - `task_to_component_nodes` — [`L879`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L879)
  - `working_trace_error_analysis` — [`L870`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L870)
  - `working_trace_knowledge` — [`L867`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L867)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`UndirectedNode`](../../knowledge_management/graph.md#UndirectedNode), [`add_node`](../../knowledge_management/graph.md#UndirectedGraph.add_node), [`id`](../../knowledge_management/vector_base.md#KnowledgeMetaData.id), [`UndirectedGraph`](../../knowledge_management/graph.md#UndirectedGraph), [`add_nodes`](../../knowledge_management/graph.md#UndirectedGraph.add_nodes), [`query_by_node`](../../knowledge_management/graph.md#UndirectedGraph.query_by_node), [`get_node_by_content`](../../knowledge_management/graph.md#UndirectedGraph.get_node_by_content), [`EvolvingKnowledgeBase`](../../../core/evolving_framework.md#EvolvingKnowledgeBase), [`get_nodes_intersection`](../../knowledge_management/graph.md#UndirectedGraph.get_nodes_intersection), [`query_by_content`](../../knowledge_management/graph.md#UndirectedGraph.query_by_content), [`size`](../../knowledge_management/graph.md#Graph.size)
- used by: [`load_or_init_knowledge_base`](knowledge_management.md#CoSTEERRAGStrategy.load_or_init_knowledge_base), [`query`](../../../core/evolving_framework.md#EvolvingKnowledgeBase.query)

### `CoSTEERQueriedKnowledge`  ·  implements/extends QueriedKnowledge
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:102`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L102) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
- doc: Data container for knowledge retrieved from the CoSTEER knowledge base during a query operation.
- signature: `class CoSTEERQueriedKnowledge(QueriedKnowledge):`
- members:
  - `failed_task_info_set` — [`L137`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L137)
  - `success_task_to_knowledge_dict` — [`L136`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L136)
- protocol/private: `__init__`[`L135`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L135)
- uses (calls/refs, reference-scoped): [`QueriedKnowledge`](../../../core/evolving_framework.md#QueriedKnowledge), [`CoSTEERQueriedKnowledgeV1`](knowledge_management.md#CoSTEERQueriedKnowledgeV1)
- used by: [`evaluate`](../data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`implement_data`](../finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_data), [`evaluate`](../data_science/raw_data_loader/eval.md#DataLoaderCoSTEEREvaluator.evaluate), [`implement_one_task`](../../../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../data_science/pipeline/__init__.md#PipelineMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../data_science/model/__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../data_science/ensemble/__init__.md#EnsembleMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../data_science/feature/__init__.md#FeatureMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../data_science/workflow/__init__.md#WorkflowMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../model_coder/evolving_strategy.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`evolve_iter`](evolving_strategy.md#MultiProcessEvolvingStrategy.evolve_iter), [`query`](knowledge_management.md#CoSTEERRAGStrategyV2.query), [`QueriedKnowledge`](../../../core/evolving_framework.md#QueriedKnowledge), [`implement_lf_config`](../finetune/__init__.md#LLMFinetuneEvolvingStrategy.implement_lf_config), [`component_query`](knowledge_management.md#CoSTEERRAGStrategyV2.component_query), [`error_query`](knowledge_management.md#CoSTEERRAGStrategyV2.error_query), [`former_trace_query`](knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query), [`evaluate`](../rl/costeer.md#RLCoderEvaluator.evaluate), [`implement_one_task`](../../../scenarios/finetune/train/runner.md#FTRunnerEvolvingStrategy.implement_one_task), [`evolve_iter`](../rl/costeer.md#RLEvolvingStrategy.evolve_iter), [`task_to_similar_task_successful_knowledge`](knowledge_management.md#CoSTEERQueriedKnowledgeV1.task_to_similar_task_successful_knowledge), [`query`](knowledge_management.md#CoSTEERRAGStrategyV1.query), [`CoSTEERQueriedKnowledgeV1`](knowledge_management.md#CoSTEERQueriedKnowledgeV1), [`query`](knowledge_management.md#CoSTEERKnowledgeBaseV1.query)

### `CoSTEERQueriedKnowledgeV1`  ·  implements/extends CoSTEERQueriedKnowledge
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:155`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L155)
- signature: `class CoSTEERQueriedKnowledgeV1(CoSTEERQueriedKnowledge):`
- members:
  - `task_to_former_failed_traces` — [`L163`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L163)
  - `task_to_similar_task_successful_knowledge` — [`L164`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L164)
- protocol/private: `__init__`[`L156`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L156)
- uses (calls/refs, reference-scoped): [`CoSTEERQueriedKnowledge`](knowledge_management.md#CoSTEERQueriedKnowledge), [`CoSTEERQueriedKnowledgeV2`](knowledge_management.md#CoSTEERQueriedKnowledgeV2), [`__init__`](knowledge_management.md#CoSTEERQueriedKnowledge.__init__)
- used by: [`evaluate`](../data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`implement_one_task`](../factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`CoSTEERQueriedKnowledge`](knowledge_management.md#CoSTEERQueriedKnowledge), [`component_query`](knowledge_management.md#CoSTEERRAGStrategyV2.component_query), [`error_query`](knowledge_management.md#CoSTEERRAGStrategyV2.error_query), [`former_trace_query`](knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query), [`CoSTEERQueriedKnowledgeV2`](knowledge_management.md#CoSTEERQueriedKnowledgeV2), [`task_to_similar_error_successful_knowledge`](knowledge_management.md#CoSTEERQueriedKnowledgeV2.task_to_similar_error_successful_knowledge)

### `CoSTEERQueriedKnowledgeV2`  ·  implements/extends CoSTEERQueriedKnowledgeV1
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:281`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L281) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
- doc: Aggregation subclass of `CoSTEERQueriedKnowledgeV1` that extends the queried knowledge to also
- signature: `class CoSTEERQueriedKnowledgeV2(CoSTEERQueriedKnowledgeV1):`
- members:
  - `task_to_similar_error_successful_knowledge` — [`L346`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L346)
- protocol/private: `__init__`[`L339`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L339)
- uses (calls/refs, reference-scoped): [`CoSTEERQueriedKnowledgeV1`](knowledge_management.md#CoSTEERQueriedKnowledgeV1), [`__init__`](knowledge_management.md#CoSTEERQueriedKnowledgeV1.__init__)
- used by: [`evaluate`](../data_science/pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`evaluate`](../data_science/raw_data_loader/eval.md#DataLoaderCoSTEEREvaluator.evaluate), [`implement_one_task`](../factor_coder/evolving_strategy.md#FactorMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../model_coder/evolving_strategy.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`query`](knowledge_management.md#CoSTEERRAGStrategyV2.query), [`component_query`](knowledge_management.md#CoSTEERRAGStrategyV2.component_query), [`error_query`](knowledge_management.md#CoSTEERRAGStrategyV2.error_query), [`former_trace_query`](knowledge_management.md#CoSTEERRAGStrategyV2.former_trace_query), [`CoSTEERQueriedKnowledgeV1`](knowledge_management.md#CoSTEERQueriedKnowledgeV1)

### `CoSTEERRAGStrategy`  ·  implements/extends RAGStrategy
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:55`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L55)
- signature: `class CoSTEERRAGStrategy(RAGStrategy):`
- members:
  - `dump_knowledge_base(self)` — [`L82`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L82) — documented in [rdagent-core-evolving_framework](../../../../../concepts/rdagent-core-evolving_framework.md)
  - `load_dumped_knowledge_base(self, *args, **kwargs)` — [`L91`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L91) — documented in [rdagent-core-evolving_framework](../../../../../concepts/rdagent-core-evolving_framework.md)
  - `load_or_init_knowledge_base(self, former_knowledge_base_path: Path = None, component_init_list: list = [], evolving_version: int = 2)` — [`L60`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L60)
  - `dump_knowledge_base_path` — [`L58`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L58)
- protocol/private: `__init__`[`L56`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L56)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`knowledgebase`](../../../core/evolving_framework.md#RAGStrategy.knowledgebase), [`RAGStrategy`](../../../core/evolving_framework.md#RAGStrategy), [`EvolvingKnowledgeBase`](../../../core/evolving_framework.md#EvolvingKnowledgeBase), [`__init__`](../../../core/evolving_framework.md#RAGStrategy.__init__), [`CoSTEERKnowledgeBaseV1`](knowledge_management.md#CoSTEERKnowledgeBaseV1), [`CoSTEERKnowledgeBaseV2`](knowledge_management.md#CoSTEERKnowledgeBaseV2), [`CoSTEERRAGStrategyV1`](knowledge_management.md#CoSTEERRAGStrategyV1), [`CoSTEERRAGStrategyV2`](knowledge_management.md#CoSTEERRAGStrategyV2)
- used by: [`RAGStrategy`](../../../core/evolving_framework.md#RAGStrategy), [`load_or_init_knowledge_base`](../../../core/evolving_framework.md#RAGStrategy.load_or_init_knowledge_base), [`__init__`](knowledge_management.md#CoSTEERRAGStrategyV1.__init__), [`__init__`](knowledge_management.md#CoSTEERRAGStrategyV2.__init__), [`CoSTEERRAGStrategyV1`](knowledge_management.md#CoSTEERRAGStrategyV1), [`CoSTEERRAGStrategyV2`](knowledge_management.md#CoSTEERRAGStrategyV2), [`dump_knowledge_base`](../../../core/evolving_framework.md#RAGStrategy.dump_knowledge_base), [`load_dumped_knowledge_base`](../../../core/evolving_framework.md#RAGStrategy.load_dumped_knowledge_base)

### `CoSTEERRAGStrategyV1`  ·  implements/extends CoSTEERRAGStrategy
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:168`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L168)
- doc: it is deprecated
- signature: `class CoSTEERRAGStrategyV1(CoSTEERRAGStrategy):`
- members:
  - `generate_knowledge(self, evolving_trace: list[EvoStep], *, return_knowledge: bool = False)` — [`L176`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L176)
  - `query(self, evo: EvolvableSubjects, evolving_trace: list[EvoStep])` — [`L219`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L219) — documented in [rdagent-core-evolving_framework](../../../../../concepts/rdagent-core-evolving_framework.md)
  - `current_generated_trace_count` — [`L173`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L173)
  - `settings` — [`L174`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L174)
- protocol/private: `__init__`[`L171`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L171)
- uses (calls/refs, reference-scoped): [`CoSTEERQueriedKnowledge`](knowledge_management.md#CoSTEERQueriedKnowledge), [`CoSTEERSettings`](config.md#CoSTEERSettings), [`EvoStep`](../../../core/evolving_framework.md#EvoStep), [`EvolvableSubjects`](../../../core/evolving_framework.md#EvolvableSubjects), [`CoSTEERRAGStrategy`](knowledge_management.md#CoSTEERRAGStrategy), [`Knowledge`](../../../core/evolving_framework.md#Knowledge), [`__init__`](knowledge_management.md#CoSTEERRAGStrategy.__init__)
- used by: [`generate_knowledge`](../../../core/evolving_framework.md#RAGStrategy.generate_knowledge), [`query`](../../../core/evolving_framework.md#RAGStrategy.query), [`rag`](__init__.md#CoSTEER.rag), [`CoSTEERRAGStrategy`](knowledge_management.md#CoSTEERRAGStrategy)

### `CoSTEERRAGStrategyV2`  ·  implements/extends CoSTEERRAGStrategy
- def: [`rdagent/components/coder/CoSTEER/knowledge_management.py:354`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L354)
- signature: `class CoSTEERRAGStrategyV2(CoSTEERRAGStrategy):`
- members:
  - `analyze_component(self, target_task_information)` — [`L457`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L457) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `analyze_error(self, single_feedback, feedback_type="execution")` — [`L488`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L488)
  - `component_query(self, evo: EvolvableSubjects, queried_knowledge_v2: CoSTEERQueriedKnowledgeV2, v2_query_component_limit: int = 5, knowledge_sampler: float = 1)` — [`L593`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L593) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `error_query(self, evo: EvolvableSubjects, queried_knowledge_v2: CoSTEERQueriedKnowledgeV2, v2_query_error_limit: int = 5, knowledge_sampler: float = 1)` — [`L723`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L723) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `former_trace_query(self, evo: EvolvableSubjects, queried_knowledge_v2: CoSTEERQueriedKnowledgeV2, v2_query_former_trace_limit: int = 5, v2_add_fail_attempt_to_latest_successful_execution: bool = False)` — [`L530`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L530) — Query the former trace knowledge of the working trace, and find all the failed task information which tried more than fail_task_trial_limit times — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `generate_knowledge(self, evolving_trace: list[EvoStep], *, return_knowledge: bool = False)` — [`L360`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L360) — documented in [rdagent-components-coder-CoSTEER-evaluators](../../../../../concepts/rdagent-components-coder-CoSTEER-evaluators.md)
  - `query(self, evo: EvolvableSubjects, evolving_trace: list[EvoStep])` — [`L431`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L431) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `current_generated_trace_count` — [`L357`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L357)
  - `settings` — [`L358`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L358)
- protocol/private: `__init__`[`L355`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/CoSTEER/knowledge_management.py#L355)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`warning`](../../../log/logger.md#RDAgentLog.warning), [`CoSTEERSingleFeedback`](evaluators.md#CoSTEERSingleFeedback), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`UndirectedNode`](../../knowledge_management/graph.md#UndirectedNode), [`final_decision`](evaluators.md#CoSTEERSingleFeedback.final_decision), [`knowledgebase`](../../../core/evolving_framework.md#RAGStrategy.knowledgebase), [`CoSTEERQueriedKnowledge`](knowledge_management.md#CoSTEERQueriedKnowledge), [`CoSTEERSettings`](config.md#CoSTEERSettings), [`return_checking`](evaluators.md#CoSTEERSingleFeedback.return_checking), [`EvoStep`](../../../core/evolving_framework.md#EvoStep), [`EvolvableSubjects`](../../../core/evolving_framework.md#EvolvableSubjects), [`execution`](evaluators.md#CoSTEERSingleFeedback.execution), [`CoSTEERQueriedKnowledgeV2`](knowledge_management.md#CoSTEERQueriedKnowledgeV2), [`feedback`](../../../core/evolving_framework.md#EvoStep.feedback), [`task_to_similar_task_successful_knowledge`](knowledge_management.md#CoSTEERQueriedKnowledgeV1.task_to_similar_task_successful_knowledge), [`CoSTEERRAGStrategy`](knowledge_management.md#CoSTEERRAGStrategy), [`Knowledge`](../../../core/evolving_framework.md#Knowledge), [`calculate_embedding_distance_between_str_list`](../../../oai/llm_utils.md#calculate_embedding_distance_between_str_list), [`task_to_similar_error_successful_knowledge`](knowledge_management.md#CoSTEERQueriedKnowledgeV2.task_to_similar_error_successful_knowledge), [`failed_task_info_set`](knowledge_management.md#CoSTEERQueriedKnowledge.failed_task_info_set), [`task_to_former_failed_traces`](knowledge_management.md#CoSTEERQueriedKnowledgeV1.task_to_former_failed_traces), [`CoSTEERKnowledge`](knowledge_management.md#CoSTEERKnowledge), [`__init__`](knowledge_management.md#CoSTEERRAGStrategy.__init__), [`evolvable_subjects`](../../../core/evolving_framework.md#EvoStep.evolvable_subjects), [`fail_task_trial_limit`](config.md#CoSTEERSettings.fail_task_trial_limit), [`v2_add_fail_attempt_to_latest_successful_execution`](config.md#CoSTEERSettings.v2_add_fail_attempt_to_latest_successful_execution), [`v2_knowledge_sampler`](config.md#CoSTEERSettings.v2_knowledge_sampler), [`v2_query_component_limit`](config.md#CoSTEERSettings.v2_query_component_limit), [`v2_query_error_limit`](config.md#CoSTEERSettings.v2_query_error_limit), [`v2_query_former_trace_limit`](config.md#CoSTEERSettings.v2_query_former_trace_limit)
- used by: [`generate_knowledge`](../../../core/evolving_framework.md#RAGStrategy.generate_knowledge), [`query`](../../../core/evolving_framework.md#RAGStrategy.query), [`rag`](__init__.md#CoSTEER.rag), [`CoSTEERRAGStrategy`](knowledge_management.md#CoSTEERRAGStrategy)

