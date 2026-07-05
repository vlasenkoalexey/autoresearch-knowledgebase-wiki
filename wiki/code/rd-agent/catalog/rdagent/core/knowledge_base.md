---
title: 'Module: rdagent/core/knowledge_base.py'
type: catalog
provenance: extracted
module: rdagent/core/knowledge_base.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.knowledge_base`/KnowledgeBase#
symbols:
  KnowledgeBase: ''
  KnowledgeBase.dump: dump().
  KnowledgeBase.path: path.
  KnowledgeBase.__init__: __init__().
  KnowledgeBase.load: load().
---
# Module: [`rdagent/core/knowledge_base.py`](../../../../../../raw/code/rd-agent/rdagent/core/knowledge_base.py)

## Classes
### `KnowledgeBase`
- def: [`rdagent/core/knowledge_base.py:8`](../../../../../../raw/code/rd-agent/rdagent/core/knowledge_base.py#L8)
- signature: `class KnowledgeBase:`
- members:
  - `dump(self)` — [`L22`](../../../../../../raw/code/rd-agent/rdagent/core/knowledge_base.py#L22)
  - `load(self)` — [`L13`](../../../../../../raw/code/rd-agent/rdagent/core/knowledge_base.py#L13)
  - `path` — [`L10`](../../../../../../raw/code/rd-agent/rdagent/core/knowledge_base.py#L10)
- protocol/private: `__init__`[`L9`](../../../../../../raw/code/rd-agent/rdagent/core/knowledge_base.py#L9)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../log/__init__.md#rdagent_logger.rdagent_logger), [`warning`](../log/logger.md#RDAgentLog.warning), [`VectorBase`](../components/knowledge_management/vector_base.md#VectorBase), [`EvolvingKnowledgeBase`](evolving_framework.md#EvolvingKnowledgeBase), [`Graph`](../components/knowledge_management/graph.md#Graph)
- used by: [`record`](../scenarios/data_science/loop.md#DataScienceRDLoop.record), [`DSTrace`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace), [`if_using_vector_rag`](../scenarios/kaggle/experiment/scenario.md#KGScenario.if_using_vector_rag), [`FTTrace`](../scenarios/finetune/proposal/trace.md#FTTrace), [`path`](../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.path), [`VectorBase`](../components/knowledge_management/vector_base.md#VectorBase), [`EvolvingKnowledgeBase`](evolving_framework.md#EvolvingKnowledgeBase), [`__init__`](../scenarios/data_science/proposal/exp_gen/base.md#DSTrace.__init__), [`__init__`](../scenarios/finetune/proposal/trace.md#FTTrace.__init__), [`__init__`](../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.__init__), [`add_document`](../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.add_document), [`RLTrace`](../scenarios/rl/proposal/trace.md#RLTrace), [`used_idea_id_set`](../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.used_idea_id_set), [`Graph`](../components/knowledge_management/graph.md#Graph), [`ASpecificKB`](proposal.md#ASpecificKB), [`__init__`](../components/knowledge_management/graph.md#Graph.__init__), [`__init__`](../components/knowledge_management/vector_base.md#PDVectorBase.__init__), [`task_to_embedding`](../components/coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV1.task_to_embedding)

