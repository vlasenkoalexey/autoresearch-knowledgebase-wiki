---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.analysis_utils.meta_tree_analysis`/
symbols:
  calculate_tree_statistics: calculate_tree_statistics().
  write_tree_reports: write_tree_reports().
  generate_journal_report: generate_journal_report().
  generate_tree_reports_and_stats: generate_tree_reports_and_stats().
  calculate_tree_statistics.calculate_depth: calculate_tree_statistics().calculate_depth().
  create_client: create_client().
  client: client.
  dict_to_markdown: dict_to_markdown().
  prettify_key: prettify_key().
  plot_aggregate_stats: plot_aggregate_stats().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py)

## Functions
- `calculate_depth(node_id, node_dict, depth=0)` — [`L103`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L103)
- `calculate_tree_statistics(journal: Journal)` — [`L69`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L69) — Calculates statistical metrics from a Journal tree structure.
- `create_client(api: str = "gdm", model_id: str = "gemini-2.0-flash", provider: str = "gdm")` — [`L27`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L27) — Creates and returns a configured GDM client.
- `dict_to_markdown(data: dict)` — [`L185`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L185) — Formats a dictionary into markdown.
- `generate_journal_report(journal: Journal, task_description: str, include_code: bool = False)` — [`L40`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L40) — Generates a structured technical markdown report from a journal.
- `generate_tree_reports_and_stats(meta_experiment_path: Path)` — [`L304`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L304) — Concurrently processes multiple experiments and aggregates statistics.
- `plot_aggregate_stats(stats_list: List[Dict[str, Union[int, float]]], comp_name: str, meta_exp_dir: Path)` — [`L214`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L214) — Plots various distributions (boxplot, histogram, and bar chart) of all numerical
- `prettify_key(key: str)` — [`L180`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L180) — Converts a snake_case or camelCase key to a human-readable format.
- `write_tree_reports(experiment_path: Path)` — [`L190`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L190) — Writes detailed markdown reports and statistics based on an experiment's journal.

## Module values
- `client` — [`L37`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/meta_tree_analysis.py#L37)

