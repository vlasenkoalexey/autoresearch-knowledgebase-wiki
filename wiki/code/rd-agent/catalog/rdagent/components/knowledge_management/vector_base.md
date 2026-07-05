---
title: 'Module: rdagent/components/knowledge_management/vector_base.py'
type: catalog
provenance: extracted
module: rdagent/components/knowledge_management/vector_base.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.knowledge_management.vector_base`/
symbols:
  PDVectorBase.add: PDVectorBase#add().
  KnowledgeMetaData.id: KnowledgeMetaData#id.
  KnowledgeMetaData.content: KnowledgeMetaData#content.
  KnowledgeMetaData.split_into_trunk: KnowledgeMetaData#split_into_trunk().
  KnowledgeMetaData.create_embedding: KnowledgeMetaData#create_embedding().
  Document: Document.
  PDVectorBase.search: PDVectorBase#search().
  KnowledgeMetaData.label: KnowledgeMetaData#label.
  PDVectorBase: PDVectorBase#
  KnowledgeMetaData.embedding: KnowledgeMetaData#embedding.
  VectorBase: VectorBase#
  KnowledgeMetaData: KnowledgeMetaData#
  KnowledgeMetaData.__repr__: KnowledgeMetaData#__repr__().
  contents_to_documents: contents_to_documents().
  VectorBase.add: VectorBase#add().
  PDVectorBase.vector_df: PDVectorBase#vector_df.
  VectorBase.search: VectorBase#search().
  KnowledgeMetaData.from_dict: KnowledgeMetaData#from_dict().
  PDVectorBase.__init__: PDVectorBase#__init__().
  PDVectorBase.shape: PDVectorBase#shape().
  KnowledgeMetaData.trunks: KnowledgeMetaData#trunks.
  KnowledgeMetaData.__init__: KnowledgeMetaData#__init__().
  KnowledgeMetaData.trunks_embedding: KnowledgeMetaData#trunks_embedding.
  KnowledgeMetaData.split_string_into_chunks: KnowledgeMetaData#split_string_into_chunks().
---
# Module: [`rdagent/components/knowledge_management/vector_base.py`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py)

## Classes
### `KnowledgeMetaData`
- def: [`rdagent/components/knowledge_management/vector_base.py:13`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L13)
- signature: `class KnowledgeMetaData:`
- members:
  - `create_embedding(self)` — [`L40`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L40) — create content's embedding
  - `from_dict(self, data: dict)` — [`L50`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L50)
  - `split_into_trunk(self, size: int = 1000, overlap: int = 0)` — [`L22`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L22) — split content into trunks and create embedding by trunk
  - `split_string_into_chunks(string: str, chunk_size: int)` — [`L30`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L30)
  - `content` — [`L16`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L16) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `embedding` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L18) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `id` — [`L17`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L17)
  - `label` — [`L15`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L15) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `trunks` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L19)
  - `trunks_embedding` — [`L20`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L20)
- protocol/private: `__init__`[`L14`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L14), `__repr__`[`L55`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L55)
- uses (calls/refs, reference-scoped): [`APIBackend`](../../oai/llm_utils.md#APIBackend), [`UndirectedNode`](graph.md#UndirectedNode), [`from_dict`](../../scenarios/kaggle/knowledge_management/vector_base.md#KGKnowledgeDocument.from_dict), [`create_embedding`](../../oai/backend/base.md#APIBackend.create_embedding), [`KGKnowledgeDocument`](../../scenarios/kaggle/knowledge_management/vector_base.md#KGKnowledgeDocument), [`split_into_trunk`](../../scenarios/kaggle/knowledge_management/vector_base.md#KGKnowledgeDocument.split_into_trunk)
- used by: [`sample_ideas`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.sample_ideas), [`add`](../../scenarios/kaggle/knowledge_management/vector_base.md#KaggleExperienceBase.add), [`add_node`](graph.md#UndirectedGraph.add_node), [`add`](vector_base.md#PDVectorBase.add), [`update_success_task`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.update_success_task), [`from_dict`](../../scenarios/kaggle/knowledge_management/vector_base.md#KGKnowledgeDocument.from_dict), [`batch_embedding`](graph.md#Graph.batch_embedding), [`get_nodes_within_steps`](graph.md#UndirectedGraph.get_nodes_within_steps), [`add_experience_to_vector_base`](../../scenarios/kaggle/knowledge_management/vector_base.md#KaggleExperienceBase.add_experience_to_vector_base), [`__repr__`](../../scenarios/kaggle/knowledge_management/vector_base.md#KGKnowledgeDocument.__repr__), [`Document`](vector_base.md#Document), [`search_experience`](../../scenarios/kaggle/knowledge_management/vector_base.md#KaggleExperienceBase.search_experience), [`semantic_search`](graph.md#UndirectedGraph.semantic_search), [`search`](vector_base.md#PDVectorBase.search), [`__repr__`](graph.md#UndirectedNode.__repr__), [`__str__`](graph.md#UndirectedNode.__str__), [`Node`](graph.md#Node), [`trunks`](../../scenarios/kaggle/knowledge_management/vector_base.md#KGKnowledgeDocument.trunks), [`cal_distance`](graph.md#UndirectedGraph.cal_distance), [`filter_label`](graph.md#UndirectedGraph.filter_label), [`__init__`](graph.md#UndirectedNode.__init__), [`__init__`](../../scenarios/kaggle/knowledge_management/vector_base.md#KGKnowledgeDocument.__init__)

### `PDVectorBase`  ·  implements/extends VectorBase
- def: [`rdagent/components/knowledge_management/vector_base.py:106`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L106)
- doc: Implement of VectorBase using Pandas
- signature: `class PDVectorBase(VectorBase):`
- members:
  - `add(self, document: Union[Document, List[Document]])` — [`L118`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L118) — add new node to vector_df
  - `search(self, content: str, topk_k: int | None = None, similarity_threshold: float = 0, constraint_labels: list[str] | None = None)` — [`L158`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L158) — Search vector by node's embedding.
  - `shape(self)` — [`L115`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L115)
  - `vector_df` — [`L112`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L112)
- protocol/private: `__init__`[`L111`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L111)
- uses (calls/refs, reference-scoped): [`add`](../../scenarios/kaggle/knowledge_management/vector_base.md#KaggleExperienceBase.add), [`id`](vector_base.md#KnowledgeMetaData.id), [`content`](vector_base.md#KnowledgeMetaData.content), [`create_embedding`](vector_base.md#KnowledgeMetaData.create_embedding), [`Document`](vector_base.md#Document), [`label`](vector_base.md#KnowledgeMetaData.label), [`VectorBase`](vector_base.md#VectorBase), [`embedding`](vector_base.md#KnowledgeMetaData.embedding), [`KaggleExperienceBase`](../../scenarios/kaggle/knowledge_management/vector_base.md#KaggleExperienceBase), [`__init__`](../../core/knowledge_base.md#KnowledgeBase.__init__), [`from_dict`](vector_base.md#KnowledgeMetaData.from_dict), [`trunks`](vector_base.md#KnowledgeMetaData.trunks), [`trunks_embedding`](vector_base.md#KnowledgeMetaData.trunks_embedding)
- used by: [`kaggle_base`](../../scenarios/kaggle/knowledge_management/vector_base.md#kaggle_base), [`search_experience`](../../scenarios/kaggle/knowledge_management/vector_base.md#KaggleExperienceBase.search_experience), [`clear`](graph.md#UndirectedGraph.clear), [`__init__`](graph.md#UndirectedGraph.__init__), [`VectorBase`](vector_base.md#VectorBase), [`add`](vector_base.md#VectorBase.add), [`search`](vector_base.md#VectorBase.search), [`KaggleExperienceBase`](../../scenarios/kaggle/knowledge_management/vector_base.md#KaggleExperienceBase), [`__init__`](../../scenarios/kaggle/knowledge_management/vector_base.md#KaggleExperienceBase.__init__)

### `VectorBase`  ·  implements/extends KnowledgeBase
- def: [`rdagent/components/knowledge_management/vector_base.py:72`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L72)
- doc: This class is used for handling vector storage and query
- signature: `class VectorBase(KnowledgeBase):`
- members:
  - `add(self, document: Union[Document, List[Document]])` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L77) — add new node to vector_df
  - `search(self, content: str, topk_k: int | None = None, similarity_threshold: float = 0)` — [`L90`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L90) — search vector_df by node
- uses (calls/refs, reference-scoped): [`add`](vector_base.md#PDVectorBase.add), [`KnowledgeBase`](../../core/knowledge_base.md#KnowledgeBase), [`Document`](vector_base.md#Document), [`search`](vector_base.md#PDVectorBase.search), [`PDVectorBase`](vector_base.md#PDVectorBase)
- used by: [`add_node`](graph.md#UndirectedGraph.add_node), [`KnowledgeBase`](../../core/knowledge_base.md#KnowledgeBase), [`semantic_search`](graph.md#UndirectedGraph.semantic_search), [`PDVectorBase`](vector_base.md#PDVectorBase), [`clear`](graph.md#UndirectedGraph.clear), [`__init__`](graph.md#UndirectedGraph.__init__)

## Functions
- `contents_to_documents(contents: List[str], label: str = None)` — [`L62`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L62)

## Module values
- `Document` — [`L59`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/vector_base.py#L59) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)

