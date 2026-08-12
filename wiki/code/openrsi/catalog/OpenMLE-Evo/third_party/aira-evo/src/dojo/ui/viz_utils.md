---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.ui.viz_utils`/
symbols:
  create_config_comparison: create_config_comparison().
  flatten_dict: flatten_dict().
  create_config_comparison.extract_keys: create_config_comparison().extract_keys().
  create_config_graph: create_config_graph().
  create_config_diff_viz: create_config_diff_viz().
  load_yaml_config: load_yaml_config().
  visualize_config_graph: visualize_config_graph().
  create_plotly_config_graph: create_plotly_config_graph().
  visualize_parameter_heatmap: visualize_parameter_heatmap().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py)

## Functions
- `create_config_comparison(config_paths: List[str], config_dir: str)` — [`L174`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L174) — Create a comparison dataframe for multiple configurations.
- `create_config_diff_viz(config1: Dict, config2: Dict)` — [`L269`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L269) — Create a visualization showing differences between two configs.
- `create_config_graph(config_dir: str, configs: Dict[str, List[str]])` — [`L31`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L31) — Create a directed graph of configuration dependencies.
- `create_plotly_config_graph(G: nx.DiGraph)` — [`L100`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L100) — Create an interactive Plotly graph of the configuration dependencies.
- `extract_keys(data, prefix="")` — [`L186`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L186)
- `flatten_dict(config: Dict, parent_key: str = "", sep: str = ".")` — [`L257`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L257) — Flatten a nested dictionary.
- `load_yaml_config(file_path: str)` — [`L21`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L21) — Load YAML configuration file.
- `visualize_config_graph(G: nx.DiGraph)` — [`L70`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L70) — Visualize the config graph using matplotlib.
- `visualize_parameter_heatmap(df: pd.DataFrame)` — [`L228`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/viz_utils.py#L228) — Create a heatmap visualization of parameter differences.

