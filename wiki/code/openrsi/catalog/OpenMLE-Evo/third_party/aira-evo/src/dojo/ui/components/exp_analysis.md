---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.ui.components.exp_analysis`/
symbols:
  RUAMEL_AVAILABLE: RUAMEL_AVAILABLE.
  analyze_meta_experiment: analyze_meta_experiment().
  execute_utility: execute_utility().
  ruamel_yaml: ruamel_yaml.
  list_experiments: list_experiments().
  ACE_AVAILABLE: ACE_AVAILABLE.
  list_files_recursive: list_files_recursive().
  display_file_content: display_file_content().
  display_image: display_image().
  find_log_files: find_log_files().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py)

## Functions
- `analyze_meta_experiment(meta_exp_path: Path)` — [`L108`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L108) — Generate basic statistics about a meta experiment.
- `display_file_content(file_path: Path, max_lines: int = 1000, mode: str = "head")` — [`L221`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L221) — Display the content of a file, supporting head, tail, or full (truncated) views.
- `display_image(file_path: Path)` — [`L280`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L280) — Display an image file using Streamlit's image component.
- `execute_utility(utility_name: str, meta_exp_path: Path, output_dir: Optional[Path] = None)` — [`L163`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L163) — Execute a utility script on the meta experiment data.
- `find_log_files(exp_path: Path, pattern: str = "*.jsonl")` — [`L102`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L102) — Find all log files matching a pattern in the experiment directory.
- `list_experiments(meta_exp_path: Path)` — [`L69`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L69) — List all experiment folders within a meta experiment directory.
- `list_files_recursive(directory: Path, max_depth: int = 3, current_depth: int = 0)` — [`L79`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L79) — Recursively list files and folders in a directory up to max_depth.

## Module values
- `ACE_AVAILABLE` — [`L63`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L63)
- `RUAMEL_AVAILABLE` — [`L45`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L45)
- `ruamel_yaml` — [`L40`](../../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/ui/components/exp_analysis.py#L40)

