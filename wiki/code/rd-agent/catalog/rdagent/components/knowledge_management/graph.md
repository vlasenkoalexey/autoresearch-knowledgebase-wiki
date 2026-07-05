---
title: 'Module: rdagent/components/knowledge_management/graph.py'
type: catalog
provenance: extracted
module: rdagent/components/knowledge_management/graph.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.knowledge_management.graph`/
symbols:
  UndirectedNode: UndirectedNode#
  UndirectedGraph.add_node: UndirectedGraph#add_node().
  Graph.batch_embedding: Graph#batch_embedding().
  UndirectedGraph.get_nodes_within_steps: UndirectedGraph#get_nodes_within_steps().
  UndirectedGraph.semantic_search: UndirectedGraph#semantic_search().
  UndirectedGraph: UndirectedGraph#
  UndirectedNode.neighbors: UndirectedNode#neighbors.
  Graph.nodes: Graph#nodes.
  UndirectedNode.__str__: UndirectedNode#__str__().
  UndirectedNode.__repr__: UndirectedNode#__repr__().
  UndirectedGraph.add_nodes: UndirectedGraph#add_nodes().
  UndirectedGraph.clear: UndirectedGraph#clear().
  Node: Node.
  UndirectedGraph.__init__: UndirectedGraph#__init__().
  UndirectedGraph.query_by_node: UndirectedGraph#query_by_node().
  UndirectedGraph.get_node: UndirectedGraph#get_node().
  UndirectedGraph.get_node_by_content: UndirectedGraph#get_node_by_content().
  UndirectedGraph.get_nodes_intersection: UndirectedGraph#get_nodes_intersection().
  UndirectedGraph.query_by_content: UndirectedGraph#query_by_content().
  Graph.get_node: Graph#get_node().
  Graph.find_node: Graph#find_node().
  UndirectedNode.add_neighbor: UndirectedNode#add_neighbor().
  Graph: Graph#
  UndirectedGraph.cal_distance: UndirectedGraph#cal_distance().
  UndirectedNode.remove_neighbor: UndirectedNode#remove_neighbor().
  UndirectedNode.get_neighbors: UndirectedNode#get_neighbors().
  Graph.get_all_nodes: Graph#get_all_nodes().
  Graph.get_all_nodes_by_label_list: Graph#get_all_nodes_by_label_list().
  UndirectedGraph.vector_base: UndirectedGraph#vector_base.
  UndirectedGraph.filter_label: UndirectedGraph#filter_label().
  Graph.__init__: Graph#__init__().
  Graph.size: Graph#size().
  UndirectedGraph.intersection: UndirectedGraph#intersection().
  UndirectedNode.__init__: UndirectedNode#__init__().
  Graph.add_node: Graph#add_node().
  Graph.__str__: Graph#__str__().
  UndirectedGraph.__str__: UndirectedGraph#__str__().
  UndirectedGraph.different: UndirectedGraph#different().
  UndirectedNode.appendix: UndirectedNode#appendix.
  graph_to_edges: graph_to_edges().
  assign_random_coordinate_to_node: assign_random_coordinate_to_node().
  assign_isometric_coordinate_to_node: assign_isometric_coordinate_to_node().
  curly_node_coordinate: curly_node_coordinate().
---
# Module: [`rdagent/components/knowledge_management/graph.py`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py)

## Classes
### `Graph`  ·  implements/extends KnowledgeBase
- def: [`rdagent/components/knowledge_management/graph.py:54`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L54)
- doc: base Graph class for Knowledge Graph Search
- signature: `class Graph(KnowledgeBase):`
- members:
  - `add_node(self, **kwargs: Any)` — [`L69`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L69)
  - `batch_embedding(nodes: list[Node])` — [`L85`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L85) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `find_node(self, content: str, label: str)` — [`L78`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L78) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `get_all_nodes(self)` — [`L72`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L72)
  - `get_all_nodes_by_label_list(self, label_list: list[str])` — [`L75`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L75)
  - `get_node(self, node_id: str)` — [`L66`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L66)
  - `size(self)` — [`L63`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L63)
  - `nodes` — [`L60`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L60) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
- protocol/private: `__init__`[`L59`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L59), `__str__`[`L104`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L104)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../oai/llm_utils.md#APIBackend), [`add_node`](graph.md#UndirectedGraph.add_node), [`KnowledgeBase`](../../core/knowledge_base.md#KnowledgeBase), [`content`](vector_base.md#KnowledgeMetaData.content), [`UndirectedGraph`](graph.md#UndirectedGraph), [`create_embedding`](../../oai/backend/base.md#APIBackend.create_embedding), [`Node`](graph.md#Node), [`embedding`](vector_base.md#KnowledgeMetaData.embedding), [`get_node`](graph.md#UndirectedGraph.get_node), [`__init__`](../../core/knowledge_base.md#KnowledgeBase.__init__)
- used by: [`graph`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph), [`add_node`](graph.md#UndirectedGraph.add_node), [`KnowledgeBase`](../../core/knowledge_base.md#KnowledgeBase), [`load_from_documents`](../../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.load_from_documents), [`add_idea`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.add_idea), [`UndirectedGraph`](graph.md#UndirectedGraph), [`clear`](graph.md#UndirectedGraph.clear), [`__init__`](graph.md#UndirectedGraph.__init__), [`get_node`](graph.md#UndirectedGraph.get_node), [`__str__`](graph.md#UndirectedGraph.__str__)

### `UndirectedGraph`  ·  implements/extends Graph
- def: [`rdagent/components/knowledge_management/graph.py:108`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L108) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
- doc: Undirected Graph which edges have no relationship
- signature: `class UndirectedGraph(Graph):`
- members:
  - `add_node(self, node: UndirectedNode, neighbor: UndirectedNode = None, same_node_threshold: float = 0.95)` — [`L120`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L120) — add node and neighbor to the Graph — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
  - `add_nodes(self, node: UndirectedNode, neighbors: list[UndirectedNode])` — [`L169`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L169) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `cal_distance(node1: UndirectedNode, node2: UndirectedNode)` — [`L438`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L438)
  - `clear(self)` — [`L314`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L314)
  - `different(nodes1: list[UndirectedNode], nodes2: list[UndirectedNode])` — [`L434`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L434)
  - `filter_label(nodes: list[UndirectedNode], labels: list[str])` — [`L442`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L442)
  - `get_node(self, node_id: str)` — [`L176`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L176) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `get_node_by_content(self, content: str)` — [`L179`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L179) — Get node by semantic distance — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `get_nodes_intersection(self, nodes: list[UndirectedNode], steps: int = 1, constraint_labels: list[str] | None = None)` — [`L235`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L235) — Get the intersection with nodes connected within n steps of nodes — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `get_nodes_within_steps(self, start_node: UndirectedNode, steps: int = 1, constraint_labels: list[str] | None = None, *, block: bool = False)` — [`L197`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L197) — Returns the nodes in the graph whose distance from node is less than or equal to step — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `intersection(nodes1: list[UndirectedNode], nodes2: list[UndirectedNode])` — [`L430`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L430)
  - `query_by_content(self, content: str | list[str], topk_k: int = 5, step: int = 1, constraint_labels: list[str] | None = None, constraint_node: UndirectedNode | None = None, similarity_threshold: float = 0, constraint_distance: float = 0, *, block: bool = False)` — [`L356`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L356) — Search graph by content similarity and connection relationship, return empty — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `query_by_node(self, node: UndirectedNode, step: int = 1, constraint_labels: list[str] | None = None, constraint_node: UndirectedNode | None = None, constraint_distance: float = 0, *, block: bool = False)` — [`L318`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L318) — search graph by connection, return empty list if nodes' chain without node near to constraint_node — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `semantic_search(self, node: UndirectedNode | str, similarity_threshold: float = 0, topk_k: int = None, constraint_labels: list[str] | None = None)` — [`L275`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L275) — Semantic search by node's embedding. — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
  - `vector_base` — [`L114`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L114)
- protocol/private: `__init__`[`L113`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L113), `__str__`[`L117`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L117)
- uses (calls/refs, reference-scoped): [`UndirectedNode`](graph.md#UndirectedNode), [`id`](vector_base.md#KnowledgeMetaData.id), [`content`](vector_base.md#KnowledgeMetaData.content), [`create_embedding`](vector_base.md#KnowledgeMetaData.create_embedding), [`neighbors`](graph.md#UndirectedNode.neighbors), [`label`](vector_base.md#KnowledgeMetaData.label), [`nodes`](graph.md#Graph.nodes), [`PDVectorBase`](vector_base.md#PDVectorBase), [`VectorBase`](vector_base.md#VectorBase), [`embedding`](vector_base.md#KnowledgeMetaData.embedding), [`add`](vector_base.md#VectorBase.add), [`find_node`](graph.md#Graph.find_node), [`Graph`](graph.md#Graph), [`add_neighbor`](graph.md#UndirectedNode.add_neighbor), [`search`](vector_base.md#VectorBase.search), [`DSKnowledgeBase`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase), [`KGKnowledgeGraph`](../../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph), [`__init__`](graph.md#Graph.__init__)
- used by: [`sample_ideas`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.sample_ideas), [`graph`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph), [`update_success_task`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.update_success_task), [`load_from_documents`](../../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.load_from_documents), [`add_idea`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.add_idea), [`build_idea_pool`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.build_idea_pool), [`__init__`](../../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.__init__), [`get_node`](graph.md#Graph.get_node), [`graph_get_node_by_content`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph_get_node_by_content), [`graph_query_by_content`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph_query_by_content), [`graph_query_by_intersection`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph_query_by_intersection), [`graph_query_by_node`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph_query_by_node), [`Graph`](graph.md#Graph), [`DSKnowledgeBase`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase), [`KGKnowledgeGraph`](../../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph), [`__init__`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.__init__), [`add_node`](graph.md#Graph.add_node)

### `UndirectedNode`  ·  implements/extends KnowledgeMetaData
- def: [`rdagent/components/knowledge_management/graph.py:22`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L22) — documented in [rdagent-components-coder-CoSTEER-knowledge_management](../../../../concepts/rdagent-components-coder-CoSTEER-knowledge_management.md)
- signature: `class UndirectedNode(Node):`
- members:
  - `add_neighbor(self, node: UndirectedNode)` — [`L29`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L29)
  - `get_neighbors(self)` — [`L38`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L38)
  - `remove_neighbor(self, node: UndirectedNode)` — [`L33`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L33)
  - `appendix` — [`L26`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L26)
  - `neighbors` — [`L25`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L25) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)
- protocol/private: `__init__`[`L23`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L23), `__repr__`[`L47`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L47), `__str__`[`L41`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L41)
- uses (calls/refs, reference-scoped): [`id`](vector_base.md#KnowledgeMetaData.id), [`content`](vector_base.md#KnowledgeMetaData.content), [`label`](vector_base.md#KnowledgeMetaData.label), [`Node`](graph.md#Node), [`__init__`](vector_base.md#KnowledgeMetaData.__init__)
- used by: [`generate_feedback`](../../scenarios/kaggle/developer/feedback.md#KGExperiment2Feedback.generate_feedback), [`sample_ideas`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.sample_ideas), [`graph`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph), [`add_node`](graph.md#UndirectedGraph.add_node), [`update_success_task`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.update_success_task), [`analyze_component`](../coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.analyze_component), [`load_from_documents`](../../scenarios/kaggle/knowledge_management/graph.md#KGKnowledgeGraph.load_from_documents), [`error_query`](../coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.error_query), [`get_nodes_within_steps`](graph.md#UndirectedGraph.get_nodes_within_steps), [`add_idea`](../../scenarios/data_science/proposal/exp_gen/idea_pool.md#DSKnowledgeBase.add_idea), [`semantic_search`](graph.md#UndirectedGraph.semantic_search), [`add_nodes`](graph.md#UndirectedGraph.add_nodes), [`query_by_node`](graph.md#UndirectedGraph.query_by_node), [`get_node`](graph.md#UndirectedGraph.get_node), [`get_node_by_content`](graph.md#UndirectedGraph.get_node_by_content), [`get_nodes_intersection`](graph.md#UndirectedGraph.get_nodes_intersection), [`query_by_content`](graph.md#UndirectedGraph.query_by_content), [`KnowledgeMetaData`](vector_base.md#KnowledgeMetaData), [`graph_get_node_by_content`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph_get_node_by_content), [`graph_query_by_content`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph_query_by_content), [`graph_query_by_intersection`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph_query_by_intersection), [`graph_query_by_node`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.graph_query_by_node), [`analyze_error`](../coder/CoSTEER/knowledge_management.md#CoSTEERRAGStrategyV2.analyze_error), [`cal_distance`](graph.md#UndirectedGraph.cal_distance), [`filter_label`](graph.md#UndirectedGraph.filter_label), [`get_all_nodes_by_label`](../coder/CoSTEER/knowledge_management.md#CoSTEERKnowledgeBaseV2.get_all_nodes_by_label), [`intersection`](graph.md#UndirectedGraph.intersection), [`different`](graph.md#UndirectedGraph.different)

## Functions
- `assign_isometric_coordinate_to_node(nodes: list, x_step: float = 1, x_origin: float = 0, y_origin: float = 0)` — [`L472`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L472)
- `assign_random_coordinate_to_node(nodes: list[str], scope: float = 1, origin: tuple[float, float] = (0, 0))` — [`L458`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L458)
- `curly_node_coordinate(coordinates: dict, center_y: float = 1, r: float = 1)` — [`L488`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L488)
- `graph_to_edges(graph: dict[str, list[str]])` — [`L446`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L446)

## Module values
- `Node` — [`L19`](../../../../../../../raw/code/rd-agent/rdagent/components/knowledge_management/graph.py#L19) — documented in [rdagent-components-knowledge_management-graph](../../../../concepts/rdagent-components-knowledge_management-graph.md)

