---
title: 'Module: rdagent/scenarios/kaggle/knowledge_management/vector_base.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/knowledge_management/vector_base.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.knowledge_management.vector_base`/
symbols:
  KaggleExperienceBase.add: KaggleExperienceBase#add().
  KGKnowledgeDocument.from_dict: KGKnowledgeDocument#from_dict().
  KaggleExperienceBase.add_experience_to_vector_base: KaggleExperienceBase#add_experience_to_vector_base().
  KGKnowledgeDocument.__repr__: KGKnowledgeDocument#__repr__().
  kaggle_base: kaggle_base.
  KaggleExperienceBase.search_experience: KaggleExperienceBase#search_experience().
  KaggleExperienceBase.load_kaggle_experience: KaggleExperienceBase#load_kaggle_experience().
  KaggleExperienceBase.refine_with_LLM: KaggleExperienceBase#refine_with_LLM().
  similarity: similarity.
  KGKnowledgeDocument.trunks_embedding: KGKnowledgeDocument#trunks_embedding.
  KaggleExperienceBase.save: KaggleExperienceBase#save().
  KGKnowledgeDocument.trunks: KGKnowledgeDocument#trunks.
  KaggleExperienceBase.kaggle_experience_data: KaggleExperienceBase#kaggle_experience_data.
  KGKnowledgeDocument: KGKnowledgeDocument#
  similarities: similarities.
  KaggleExperienceBase: KaggleExperienceBase#
  KGDocument: KGDocument.
  KaggleExperienceBase.vector_df: KaggleExperienceBase#vector_df.
  KGKnowledgeDocument.competition_name: KGKnowledgeDocument#competition_name.
  KGKnowledgeDocument.task_category: KGKnowledgeDocument#task_category.
  KGKnowledgeDocument.field: KGKnowledgeDocument#field.
  KGKnowledgeDocument.ranking: KGKnowledgeDocument#ranking.
  KGKnowledgeDocument.score: KGKnowledgeDocument#score.
  result: result.
  KGKnowledgeDocument.__init__: KGKnowledgeDocument#__init__().
  KaggleExperienceBase.__init__: KaggleExperienceBase#__init__().
  KGKnowledgeDocument.entities: KGKnowledgeDocument#entities.
  KGKnowledgeDocument.relations: KGKnowledgeDocument#relations.
  KGKnowledgeDocument.split_into_trunk: KGKnowledgeDocument#split_into_trunk().
  KGKnowledgeDocument.split_string_into_chunks: KGKnowledgeDocument#split_string_into_chunks().
  search_results: search_results.
  KaggleExperienceBase.kaggle_experience_path: KaggleExperienceBase#kaggle_experience_path.
---
# Module: [`rdagent/scenarios/kaggle/knowledge_management/vector_base.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py)

## Classes
### `KGKnowledgeDocument`  ·  implements/extends KnowledgeMetaData
- def: [`rdagent/scenarios/kaggle/knowledge_management/vector_base.py:16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L16)
- doc: Class for handling Kaggle competition specific metadata
- signature: `class KGKnowledgeDocument(Document):`
- members:
  - `__init__(self, content: str = "", label: str = None, embedding=None, identity=None, competition_name=None, task_category=None, field=None, ranking=None, score=None, entities=None, relations=None)` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L21) — Initialize KGKnowledgeMetaData for Kaggle competition posts
  - `from_dict(self, data: dict)` — [`L82`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L82) — Load Kaggle post data from a dictionary
  - `split_into_trunk(self, size: int = 1000, overlap: int = 0)` — [`L66`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L66) — Split content into trunks and create embeddings by trunk
  - `split_string_into_chunks(string: str, chunk_size: int)` — [`L72`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L72)
  - `competition_name` — [`L56`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L56)
  - `entities` — [`L63`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L63)
  - `field` — [`L58`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L58)
  - `ranking` — [`L59`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L59)
  - `relations` — [`L64`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L64)
  - `score` — [`L61`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L61)
  - `task_category` — [`L57`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L57)
  - `trunks` — [`L79`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L79)
  - `trunks_embedding` — [`L80`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L80)
- protocol/private: `__repr__`[`L96`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L96)
- uses (calls/refs, reference-scoped): [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`id`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.id), [`content`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.content), [`Document`](../../../components/knowledge_management/vector_base.md#Document), [`create_embedding`](../../../oai/backend/base.md#APIBackend.create_embedding), [`label`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.label), [`from_dict`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.from_dict), [`__init__`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.__init__)
- used by: [`add`](vector_base.md#KaggleExperienceBase.add), [`add_experience_to_vector_base`](vector_base.md#KaggleExperienceBase.add_experience_to_vector_base), [`split_into_trunk`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.split_into_trunk), [`search_experience`](vector_base.md#KaggleExperienceBase.search_experience), [`KnowledgeMetaData`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData), [`KGDocument`](vector_base.md#KGDocument), [`from_dict`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.from_dict)

### `KaggleExperienceBase`  ·  implements/extends PDVectorBase
- def: [`rdagent/scenarios/kaggle/knowledge_management/vector_base.py:106`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L106)
- doc: Class for handling Kaggle competition experience posts and organizing them for reference
- signature: `class KaggleExperienceBase(PDVectorBase):`
- members:
  - `__init__(self, vector_df_path: Union[str, Path] = None, kaggle_experience_path: Union[str, Path] = None)` — [`L111`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L111) — Initialize the KaggleExperienceBase class
  - `add(self, document: Union[KGDocument, List[KGDocument]])` — [`L128`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L128)
  - `add_experience_to_vector_base(self, experiment_feedback=None)` — [`L179`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L179) — Process Kaggle experience data or experiment feedback and add relevant information to the vector base.
  - `load_kaggle_experience(self, kaggle_experience_path: Union[str, Path])` — [`L162`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L162) — Load Kaggle experience posts from a JSON or text file
  - `refine_with_LLM(self, target: str, text: str)` — [`L270`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L270)
  - `save(self, vector_df_path: Union[str, Path])` — [`L282`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L282) — Save the vector DataFrame to a file
  - `search_experience(self, target: str, query: str, topk_k: int = 5, similarity_threshold: float = 0.1)` — [`L228`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L228) — Search for Kaggle experience posts related to the query, initially filtered by the target.
  - `kaggle_experience_data` — [`L124`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L124)
  - `kaggle_experience_path` — [`L123`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L123)
  - `vector_df` — [`L160`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L160)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`error`](../../../log/logger.md#RDAgentLog.error), [`from_dict`](vector_base.md#KGKnowledgeDocument.from_dict), [`id`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.id), [`content`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.content), [`create_embedding`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.create_embedding), [`search`](../../../components/knowledge_management/vector_base.md#PDVectorBase.search), [`extract_knowledge_from_feedback`](extract_knowledge.md#extract_knowledge_from_feedback), [`label`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.label), [`PDVectorBase`](../../../components/knowledge_management/vector_base.md#PDVectorBase), [`embedding`](../../../components/knowledge_management/vector_base.md#KnowledgeMetaData.embedding), [`trunks_embedding`](vector_base.md#KGKnowledgeDocument.trunks_embedding), [`trunks`](vector_base.md#KGKnowledgeDocument.trunks), [`KGKnowledgeDocument`](vector_base.md#KGKnowledgeDocument), [`KGDocument`](vector_base.md#KGDocument), [`competition_name`](vector_base.md#KGKnowledgeDocument.competition_name), [`field`](vector_base.md#KGKnowledgeDocument.field), [`ranking`](vector_base.md#KGKnowledgeDocument.ranking), [`score`](vector_base.md#KGKnowledgeDocument.score), [`task_category`](vector_base.md#KGKnowledgeDocument.task_category), [`__init__`](../../../components/knowledge_management/vector_base.md#PDVectorBase.__init__), [`split_into_trunk`](vector_base.md#KGKnowledgeDocument.split_into_trunk)
- used by: [`generate_RAG_content`](../proposal/proposal.md#generate_RAG_content), [`add`](../../../components/knowledge_management/vector_base.md#PDVectorBase.add), [`if_using_vector_rag`](../experiment/scenario.md#KGScenario.if_using_vector_rag), [`kaggle_base`](vector_base.md#kaggle_base), [`PDVectorBase`](../../../components/knowledge_management/vector_base.md#PDVectorBase), [`similarities`](vector_base.md#similarities)

## Module values
- `KGDocument` — [`L103`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L103)
- `kaggle_base` — [`L296`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L296)
- `result` — [`L308`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L308)
- `search_results` — [`L306`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L306)
- `similarities` — [`L306`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L306)
- `similarity` — [`L308`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/knowledge_management/vector_base.py#L308)

