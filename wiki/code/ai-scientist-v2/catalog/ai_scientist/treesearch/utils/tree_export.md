---
title: 'Module: ai_scientist/treesearch/utils/tree_export.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/utils/tree_export.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.utils.tree_export`/
symbols:
  cfg_to_tree_struct: cfg_to_tree_struct().
  generate: generate().
  get_edges: get_edges().
  create_unified_viz: create_unified_viz().
  get_completed_stages: get_completed_stages().
  generate_layout: generate_layout().
  normalize_layout: normalize_layout().
  generate_html: generate_html().
---
# Module: [`ai_scientist/treesearch/utils/tree_export.py`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py)

## Functions
- `cfg_to_tree_struct(cfg, jou: Journal, out_path: Path = None)` — [`L76`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py#L76) — documented in [ai_scientist-treesearch-journal](../../../../concepts/ai_scientist-treesearch-journal.md)
- `create_unified_viz(cfg, current_stage_viz_path)` — [`L414`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py#L414) — Create a unified visualization that shows all completed stages in a tabbed interface.
- `generate(cfg, jou: Journal, out_path: Path)` — [`L376`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py#L376)
- `generate_html(tree_graph_str: str)` — [`L362`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py#L362)
- `generate_layout(n_nodes, edges, layout_type="rt")` — [`L20`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py#L20) — Generate visual layout of graph
- `get_completed_stages(log_dir)` — [`L43`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py#L43) — Determine completed stages by checking for the existence of stage directories
- `get_edges(journal: Journal)` — [`L14`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py#L14)
- `normalize_layout(layout: np.ndarray)` — [`L34`](../../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/utils/tree_export.py#L34) — Normalize layout to [0, 1]

