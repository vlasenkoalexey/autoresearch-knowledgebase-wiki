---
title: 'Module: rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.proposal.exp_gen.idea_pool`/DS
symbols:
  DSKnowledgeBase.sample_ideas: KnowledgeBase#sample_ideas().
  DSKnowledgeBase.add_idea: KnowledgeBase#add_idea().
  DSKnowledgeBase.build_idea_pool: KnowledgeBase#build_idea_pool().
  DSIdea.__str__: Idea#__str__().
  DSIdea.to_formatted_str: Idea#to_formatted_str().
  DSIdea: Idea#
  DSKnowledgeBase.used_idea_id_set: KnowledgeBase#used_idea_id_set.
  DSKnowledgeBase: KnowledgeBase#
  DSIdea.idea: Idea#idea.
  DSIdea.method: Idea#method.
  DSIdea.context: Idea#context.
  DSIdea.hypothesis: Idea#hypothesis.
  DSKnowledgeBase.__init__: KnowledgeBase#__init__().
  DSKnowledgeBase.update_pickled_problem: KnowledgeBase#update_pickled_problem().
  DSIdea.competition: Idea#competition.
  DSIdea.__init__: Idea#__init__().
---
# Module: [`rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py)

## Classes
### `DSIdea`
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py:18`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L18)
- signature: `class DSIdea:`
- members:
  - `__init__(self, raw_knowledge: Dict | str)` — [`L19`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L19) — {
  - `to_formatted_str(self)` — [`L52`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L52)
  - `competition` — [`L35`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L35)
  - `context` — [`L38`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L38)
  - `hypothesis` — [`L39`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L39)
  - `idea` — [`L36`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L36)
  - `method` — [`L37`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L37)
- protocol/private: `__str__`[`L41`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L41)
- used by: [`hypothesis_gen`](proposal.md#DSProposalV2ExpGen.hypothesis_gen), [`generate_feedback`](../../dev/feedback.md#DSExperiment2Feedback.generate_feedback), [`sample_ideas`](idea_pool.md#DSKnowledgeBase.sample_ideas), [`add_idea`](idea_pool.md#DSKnowledgeBase.add_idea), [`build_idea_pool`](idea_pool.md#DSKnowledgeBase.build_idea_pool)

### `DSKnowledgeBase`  ·  implements/extends UndirectedGraph
- def: [`rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py:56`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L56)
- signature: `class DSKnowledgeBase(UndirectedGraph):`
- members:
  - `add_idea(self, idea: List[DSIdea] | DSIdea)` — [`L64`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L64)
  - `build_idea_pool(self, idea_pool_json_path: str | Path)` — [`L97`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L97)
  - `sample_ideas(self, problems: Dict, scenario_desc: str, exp_feedback_list_desc: str, sota_exp_desc: str, competition_desc: str)` — [`L116`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L116)
  - `update_pickled_problem(self, problems: Dict, pickled_problem_name: str)` — [`L182`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L182)
  - `used_idea_id_set` — [`L59`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L59)
- protocol/private: `__init__`[`L57`](../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/proposal/exp_gen/idea_pool.py#L57)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`warning`](../../../../log/logger.md#RDAgentLog.warning), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`UndirectedNode`](../../../../components/knowledge_management/graph.md#UndirectedNode), [`batch_embedding`](../../../../components/knowledge_management/graph.md#Graph.batch_embedding), [`get_nodes_within_steps`](../../../../components/knowledge_management/graph.md#UndirectedGraph.get_nodes_within_steps), [`id`](../../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.id), [`semantic_search`](../../../../components/knowledge_management/graph.md#UndirectedGraph.semantic_search), [`UndirectedGraph`](../../../../components/knowledge_management/graph.md#UndirectedGraph), [`dump`](../../../../core/knowledge_base.md#KnowledgeBase.dump), [`neighbors`](../../../../components/knowledge_management/graph.md#UndirectedNode.neighbors), [`add_nodes`](../../../../components/knowledge_management/graph.md#UndirectedGraph.add_nodes), [`__init__`](../../../../components/knowledge_management/graph.md#UndirectedGraph.__init__), [`get_node_by_content`](../../../../components/knowledge_management/graph.md#UndirectedGraph.get_node_by_content), [`DSIdea`](idea_pool.md#DSIdea), [`vector_base`](../../../../components/knowledge_management/graph.md#UndirectedGraph.vector_base), [`idea`](idea_pool.md#DSIdea.idea), [`context`](idea_pool.md#DSIdea.context), [`hypothesis`](idea_pool.md#DSIdea.hypothesis), [`method`](idea_pool.md#DSIdea.method), [`competition`](idea_pool.md#DSIdea.competition), [`appendix`](../../../../components/knowledge_management/graph.md#UndirectedNode.appendix)
- used by: [`load`](../../loop.md#DataScienceRDLoop.load), [`docdev`](../../loop.md#DataScienceRDLoop.docdev), [`UndirectedGraph`](../../../../components/knowledge_management/graph.md#UndirectedGraph)

