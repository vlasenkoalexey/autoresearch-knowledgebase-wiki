---
title: 'Module: rdagent/scenarios/data_science/scen/utils.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/scen/utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.scen.utils`/
symbols:
  DataFolderDescriptor.describe_folder: DataFolderDescriptor#describe_folder().
  FileTreeGenerator.generate_tree: FileTreeGenerator#generate_tree().
  FileTreeGenerator._process_directory: FileTreeGenerator#_process_directory().
  FileTreeGenerator._add_line: FileTreeGenerator#_add_line().
  describe_data_folder_v2: describe_data_folder_v2().
  FileTreeGenerator._process_single_directory: FileTreeGenerator#_process_single_directory().
  FileTreeGenerationError: FileTreeGenerationError#
  MaxLinesExceededError: MaxLinesExceededError#
  FileTreeGenerator._process_subdirectories: FileTreeGenerator#_process_subdirectories().
  FileTreeGenerator._process_files: FileTreeGenerator#_process_files().
  _walk: _walk().
  FileTreeGenerator: FileTreeGenerator#
  FileTreeGenerator.lines: FileTreeGenerator#lines.
  FileTreeGenerator._lookup_set: FileTreeGenerator#_lookup_set.
  FileTreeGenerator._build_lookup_set: FileTreeGenerator#_build_lookup_set().
  file_tree_v2: file_tree_v2().
  plaintext_files: plaintext_files.
  DirectoryPermissionError: DirectoryPermissionError#
  FileTreeGenerator.line_count: FileTreeGenerator#line_count.
  get_file_len_size: get_file_len_size().
  preview_csv: preview_csv().
  preview_parquet: preview_parquet().
  FileTreeGenerator._categorize_files: FileTreeGenerator#_categorize_files().
  DataFolderDescriptor.tree_generator: DataFolderDescriptor#tree_generator.
  DataFolderDescriptor._select_files_for_preview: DataFolderDescriptor#_select_files_for_preview().
  FileTreeGenerator.max_lines: FileTreeGenerator#max_lines.
  DataFolderDescriptor.__init__: DataFolderDescriptor#__init__().
  code_files: code_files.
  system_names: system_names.
  preview_df: preview_df().
  FileTreeGenerator.allowed_paths: FileTreeGenerator#allowed_paths.
  FileTreeGenerator._get_size_str: FileTreeGenerator#_get_size_str().
  preview_json: preview_json().
  FileTreeGenerator.priority_files: FileTreeGenerator#priority_files.
  FileTreeGenerator.hide_base_name: FileTreeGenerator#hide_base_name.
  DataFolderDescriptor: DataFolderDescriptor#
  FileTreeGenerator.__init__: FileTreeGenerator#__init__().
---
# Module: [`rdagent/scenarios/data_science/scen/utils.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py)

## Classes
### `DataFolderDescriptor`
- def: [`rdagent/scenarios/data_science/scen/utils.py:558`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L558)
- doc: Generate detailed descriptions of data folders including file previews.
- signature: `class DataFolderDescriptor:`
- members:
  - `__init__(self, tree_generator: FileTreeGenerator = None)` — [`L563`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L563) — Initialize the data folder descriptor.
  - `_select_files_for_preview(self, base_path: Path, max_files_per_group: int = 1, threshold: int = 10)` — [`L647`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L647) — Intelligently select a representative subset of files for detailed preview.
  - `describe_folder(self, base_path: Union[str, Path], include_file_details: bool = True, simple: bool = False, show_nan_columns: bool = False, max_length: int = 10000)` — [`L572`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L572) — Generate a textual preview of a directory, including an overview of the directory
  - `tree_generator` — [`L570`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L570)
- uses (calls/refs, reference-scoped): [`generate_tree`](utils.md#FileTreeGenerator.generate_tree), [`FileTreeGenerator`](utils.md#FileTreeGenerator), [`_walk`](utils.md#_walk), [`plaintext_files`](utils.md#plaintext_files), [`get_file_len_size`](utils.md#get_file_len_size), [`preview_csv`](utils.md#preview_csv), [`preview_parquet`](utils.md#preview_parquet), [`code_files`](utils.md#code_files), [`preview_json`](utils.md#preview_json)
- used by: [`describe_data_folder_v2`](utils.md#describe_data_folder_v2)

### `DirectoryPermissionError`  ·  implements/extends FileTreeGenerationError
- def: [`rdagent/scenarios/data_science/scen/utils.py:103`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L103)
- doc: Raised when directory access is denied
- signature: `class DirectoryPermissionError(FileTreeGenerationError):`
- uses (calls/refs, reference-scoped): [`FileTreeGenerationError`](utils.md#FileTreeGenerationError)
- used by: [`_process_directory`](utils.md#FileTreeGenerator._process_directory), [`FileTreeGenerationError`](utils.md#FileTreeGenerationError)

### `FileTreeGenerationError`  ·  implements/extends Exception
- def: [`rdagent/scenarios/data_science/scen/utils.py:91`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L91)
- doc: File tree generation related errors
- signature: `class FileTreeGenerationError(Exception):`
- uses (calls/refs, reference-scoped): [`MaxLinesExceededError`](utils.md#MaxLinesExceededError), [`DirectoryPermissionError`](utils.md#DirectoryPermissionError)
- used by: [`generate_tree`](utils.md#FileTreeGenerator.generate_tree), [`_process_directory`](utils.md#FileTreeGenerator._process_directory), [`MaxLinesExceededError`](utils.md#MaxLinesExceededError), [`DirectoryPermissionError`](utils.md#DirectoryPermissionError)

### `FileTreeGenerator`
- def: [`rdagent/scenarios/data_science/scen/utils.py:292`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L292)
- doc: Smart file tree generator with symlink handling and intelligent truncation.
- signature: `class FileTreeGenerator:`
- members:
  - `__init__(self, max_lines: int = 200, priority_files: Set[str] = None, hide_base_name: bool = True, allowed_paths: Set[Path] | None = None)` — [`L297`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L297) — Initialize the file tree generator.
  - `_add_line(self, text: str)` — [`L409`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L409) — Add a line to the output.
  - `_build_lookup_set(self)` — [`L322`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L322) — Build the lookup set for allowed paths.
  - `_categorize_files(self, files: List[Path])` — [`L533`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L533) — Categorize files into priority and other groups.
  - `_get_size_str(self, file_path: Path)` — [`L549`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L549) — Get file size string.
  - `_process_directory(self, path: Path, depth: int, prefix: str, base_path: Path)` — [`L424`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L424) — Process a single directory.
  - `_process_files(self, all_files: List[Path], depth: int, prefix: str)` — [`L513`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L513) — Process files with proper truncation logic.
  - `_process_single_directory(self, d: Path, depth: int, prefix: str, base_path: Path)` — [`L491`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L491) — Process a single directory entry.
  - `_process_subdirectories(self, dirs: List[Path], depth: int, prefix: str, base_path: Path)` — [`L471`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L471) — Process subdirectories with proper truncation logic.
  - `generate_tree(self, path: Union[str, Path])` — [`L338`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L338) — Generate a tree structure of files in a directory.
  - `allowed_paths` — [`L319`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L319)
  - `hide_base_name` — [`L318`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L318)
  - `line_count` — [`L317`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L317)
  - `lines` — [`L316`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L316)
  - `max_lines` — [`L314`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L314)
  - `priority_files` — [`L315`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L315)
- protocol/private: `_lookup_set`[`L320`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L320)
- uses (calls/refs, reference-scoped): [`FileTreeGenerationError`](utils.md#FileTreeGenerationError), [`MaxLinesExceededError`](utils.md#MaxLinesExceededError), [`DirectoryPermissionError`](utils.md#DirectoryPermissionError), [`system_names`](utils.md#system_names)
- used by: [`evaluate`](../../../components/coder/data_science/share/eval.md#ModelDumpEvaluator.evaluate), [`describe_folder`](utils.md#DataFolderDescriptor.describe_folder), [`_generate_file_tree`](../../finetune/scen/utils.md#FinetuneDatasetDescriptor._generate_file_tree), [`file_tree_v2`](utils.md#file_tree_v2), [`tree_generator`](utils.md#DataFolderDescriptor.tree_generator), [`__init__`](utils.md#DataFolderDescriptor.__init__)

### `MaxLinesExceededError`  ·  implements/extends FileTreeGenerationError
- def: [`rdagent/scenarios/data_science/scen/utils.py:97`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L97)
- doc: Raised when max lines limit is exceeded
- signature: `class MaxLinesExceededError(FileTreeGenerationError):`
- uses (calls/refs, reference-scoped): [`FileTreeGenerationError`](utils.md#FileTreeGenerationError)
- used by: [`generate_tree`](utils.md#FileTreeGenerator.generate_tree), [`_process_directory`](utils.md#FileTreeGenerator._process_directory), [`_add_line`](utils.md#FileTreeGenerator._add_line), [`_process_single_directory`](utils.md#FileTreeGenerator._process_single_directory), [`FileTreeGenerationError`](utils.md#FileTreeGenerationError), [`_process_files`](utils.md#FileTreeGenerator._process_files), [`_process_subdirectories`](utils.md#FileTreeGenerator._process_subdirectories)

## Functions
- `_walk(path: Path)` — [`L272`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L272) — Recursively walk a directory (analogous to os.walk but for pathlib.Path)
- `describe_data_folder_v2(base_path: Union[str, Path], include_file_details: bool = True, simple: bool = False, show_nan_columns: bool = False, max_length: int = 10000)` — [`L695`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L695) — Generate a data folder description using DataFolderDescriptor.
- `file_tree_v2(path: Union[str, Path], max_lines: int = 200, priority_files: Set[str] = None)` — [`L689`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L689) — Generate a file tree using FileTreeGenerator.
- `get_file_len_size(f: Path)` — [`L109`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L109) — Calculate the size of a file (#lines for plaintext files, otherwise #bytes)
- `preview_csv(p: Path, file_name: str, simple=True, show_nan_columns=False)` — [`L177`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L177) — Generate a textual preview of a csv file
- `preview_df(df: pd.DataFrame, file_name: str, simple=True, show_nan_columns=False)` — [`L122`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L122) — Generate a textual preview of a dataframe
- `preview_json(p: Path, file_name: str)` — [`L189`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L189) — Generate a textual preview of a json file using reprlib for compact object display
- `preview_parquet(p: Path, file_name: str, simple=True, show_nan_columns=False)` — [`L183`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L183) — Generate a textual preview of a parquet file

## Module values
- `code_files` — [`L84`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L84)
- `plaintext_files` — [`L86`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L86)
- `system_names` — [`L88`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/scen/utils.py#L88)

