---
title: 'Module: rdagent/scenarios/kaggle/knowledge_management/graph.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/knowledge_management/graph.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.knowledge_management.graph`/
symbols:
  KGKnowledgeGraph.load_from_documents: KGKnowledgeGraph#load_from_documents().
  KGKnowledgeGraph.analyze_one_document: KGKnowledgeGraph#analyze_one_document().
  KGKnowledgeGraph.path: KGKnowledgeGraph#path.
  KGKnowledgeGraph.__init__: KGKnowledgeGraph#__init__().
  KGKnowledgeGraph.add_document: KGKnowledgeGraph#add_document().
  KGKnowledgeGraph: KGKnowledgeGraph#
  graph: graph.
---
# Module: [`rdagent/scenarios/kaggle/knowledge_management/graph.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/graph.py)

## Classes
### `KGKnowledgeGraph`  ·  implements/extends UndirectedGraph
- def: [`rdagent/scenarios/kaggle/knowledge_management/graph.py:20`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/graph.py#L20)
- signature: `class KGKnowledgeGraph(UndirectedGraph):`
- members:
  - `add_document(self, document_content: str, scenario: KGScenario | None)` — [`L37`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/graph.py#L37)
  - `analyze_one_document(self, document_content: str, scenario: KGScenario | None)` — [`L41`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/graph.py#L41)
  - `load_from_documents(self, documents: List[str], scenario: KGScenario | None)` — [`L60`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/graph.py#L60)
  - `path` — [`L25`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/graph.py#L25)
- protocol/private: `__init__`[`L21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/graph.py#L21)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`RD_AGENT_SETTINGS`](../../../core/conf.md#RD_AGENT_SETTINGS), [`UndirectedNode`](../../../components/knowledge_management/graph.md#UndirectedNode), [`build_chat_completion`](../../../oai/backend/base.md#ChatSession.build_chat_completion), [`KAGGLE_IMPLEMENT_SETTING`](../../../app/kaggle/conf.md#KAGGLE_IMPLEMENT_SETTING), [`add_node`](../../../components/knowledge_management/graph.md#UndirectedGraph.add_node), [`multiprocessing_wrapper`](../../../core/utils.md#multiprocessing_wrapper), [`batch_embedding`](../../../components/knowledge_management/graph.md#Graph.batch_embedding), [`build_chat_session`](../../../oai/backend/base.md#APIBackend.build_chat_session), [`KGScenario`](../experiment/scenario.md#KGScenario), [`UndirectedGraph`](../../../components/knowledge_management/graph.md#UndirectedGraph), [`get_scenario_all_desc`](../experiment/scenario.md#KGScenario.get_scenario_all_desc), [`dump`](../../../core/knowledge_base.md#KnowledgeBase.dump), [`__init__`](../../../components/knowledge_management/graph.md#UndirectedGraph.__init__), [`multi_proc_n`](../../../core/conf.md#RDAgentSettings.multi_proc_n), [`load`](../../../core/knowledge_base.md#KnowledgeBase.load), [`domain_knowledge_path`](../../../app/kaggle/conf.md#KaggleBasePropSetting.domain_knowledge_path)
- used by: [`UndirectedGraph`](../../../components/knowledge_management/graph.md#UndirectedGraph), [`KGTrace`](../proposal/proposal.md#KGTrace), [`graph`](graph.md#graph)

## Module values
- `graph` — [`L115`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/graph.py#L115)

