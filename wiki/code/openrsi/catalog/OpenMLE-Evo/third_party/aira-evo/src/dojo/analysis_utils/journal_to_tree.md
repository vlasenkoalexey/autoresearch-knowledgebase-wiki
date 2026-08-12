---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.analysis_utils.journal_to_tree`/
symbols:
  journal_into_tree: journal_into_tree().
  json_into_tree: json_into_tree().
  main: main().
  log_to_tree: log_to_tree().
  save_journal_log_as_json: save_journal_log_as_json().
  visualise_all_trees: visualise_all_trees().
  main_menu: main_menu().
  setup_curses: setup_curses().
  journal_log_into_json: journal_log_into_json().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py)

## Functions
- `journal_into_tree(journal: Journal, exp_folder: Union[str, Path], tree_path: Optional[Union[str, Path]] = None)` — [`L110`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L110) — Generates and exports a visualization of the journal tree from a journal instance.
- `journal_log_into_json(file_path: Union[str, Path], seconds_cutoff: Optional[float | int] = None)` — [`L22`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L22) — Parse a JSONL journal and return all nodes whose timestamp is within
- `json_into_tree(json_data: Dict[str, Any], exp_folder: Union[str, Path], tree_path: Optional[Union[str, Path]] = None)` — [`L137`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L137) — Generates and exports a visualization of the journal tree from JSON data.
- `log_to_tree(exp_folder: Path)` — [`L155`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L155)
- `main()` — [`L237`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L237)
- `main_menu(stdscr)` — [`L191`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L191)
- `save_journal_log_as_json(file_path: Union[str, Path], output_dir: Optional[Union[str, Path]] = None, output_filename: str = "journal.json", seconds_cutoff: Optional[float] = None)` — [`L73`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L73) — Reads a journal JSONL file, parses it into a structured tree, and saves it as a JSON file.
- `setup_curses(stdscr)` — [`L232`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L232)
- `visualise_all_trees(meta_experiment_path: Path)` — [`L162`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/analysis_utils/journal_to_tree.py#L162) — Concurrently processes multiple experiments and visualises trees.

