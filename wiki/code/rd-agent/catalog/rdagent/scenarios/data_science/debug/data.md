---
title: 'Module: rdagent/scenarios/data_science/debug/data.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/data_science/debug/data.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.data_science.debug.data`/
symbols:
  DefaultSampler.sample: DefaultSampler#sample().
  map_competition: map_competition().
  DataReducer: DataReducer#
  DataReducer.reduce: DataReducer#reduce().
  DataSampler.data_folder: DataSampler#data_folder.
  UniqueIDDataReducer.reduce: UniqueIDDataReducer#reduce().
  FolderSampler.sample: FolderSampler#sample().
  JsonReducer.reduce: JsonReducer#reduce().
  DataSampler: DataSampler#
  DataReducer.min_frac: DataReducer#min_frac.
  DataSampler.sample_folder: DataSampler#sample_folder.
  DataSampler.data_reducer: DataSampler#data_reducer.
  SingleFilePerFolderSampler.sample: SingleFilePerFolderSampler#sample().
  DataReducer.min_num: DataReducer#min_num.
  create_debug_data: create_debug_data().
  RandDataReducer.reduce: RandDataReducer#reduce().
  DataSampler.sample: DataSampler#sample().
  JsonReducer._find_all_lists: JsonReducer#_find_all_lists().
  FolderSampler: FolderSampler#
  JsonReducer._sample_list: JsonReducer#_sample_list().
  copy_file: copy_file().
  SingleFileReducer: SingleFileReducer#
  SingleFilePerFolderSampler: SingleFilePerFolderSampler#
  FolderReducer.reduce: FolderReducer#reduce().
  FileReducer.reduce: FileReducer#reduce().
  FileKeepReducer.reduce: FileKeepReducer#reduce().
  FolderReducer: FolderReducer#
  DataSampler.data_handler: DataSampler#data_handler.
  DataHandler: DataHandler#
  GenericDataHandler: GenericDataHandler#
  RandDataReducer: RandDataReducer#
  FileReducer: FileReducer#
  FileKeepReducer: FileKeepReducer#
  UniqueIDDataReducer: UniqueIDDataReducer#
  JsonReducer: JsonReducer#
  DefaultSampler: DefaultSampler#
  DataReducer.sampled_files: DataReducer#sampled_files.
  DataSampler.included_extensions: DataSampler#included_extensions.
  DataHandler.load: DataHandler#load().
  DataHandler.dump: DataHandler#dump().
  SingleFileReducer.reduce: SingleFileReducer#reduce().
  UniqueIDDataReducer.is_valid_label: UniqueIDDataReducer#is_valid_label().
  GenericDataHandler.load: GenericDataHandler#load().
  GenericDataHandler.dump: GenericDataHandler#dump().
  JsonReducer.extract_filename: JsonReducer#extract_filename().
  copy_folder: copy_folder().
  count_files_in_folder: count_files_in_folder().
  DataReducer.__init__: DataReducer#__init__().
  DataSampler.__init__: DataSampler#__init__().
---
# Module: [`rdagent/scenarios/data_science/debug/data.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py)

## Classes
### `DataHandler`
- def: [`rdagent/scenarios/data_science/debug/data.py:18`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L18)
- doc: Base DataHandler interface.
- signature: `class DataHandler:`
- members:
  - `dump(self, df: pd.DataFrame, path)` — [`L24`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L24)
  - `load(self, path)` — [`L21`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L21)
- uses (calls/refs, reference-scoped): [`GenericDataHandler`](data.md#GenericDataHandler), [`dump`](data.md#GenericDataHandler.dump), [`load`](data.md#GenericDataHandler.load)
- used by: [`GenericDataHandler`](data.md#GenericDataHandler)

### `DataReducer`
- def: [`rdagent/scenarios/data_science/debug/data.py:93`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L93)
- doc: Base DataReducer interface.
- signature: `class DataReducer:`
- members:
  - `reduce(self, df: pd.DataFrame)` — [`L101`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L101)
  - `min_frac` — [`L97`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L97)
  - `min_num` — [`L98`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L98)
  - `sampled_files` — [`L99`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L99)
- protocol/private: `__init__`[`L96`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L96)
- uses (calls/refs, reference-scoped): [`reduce`](data.md#UniqueIDDataReducer.reduce), [`reduce`](data.md#JsonReducer.reduce), [`reduce`](data.md#RandDataReducer.reduce), [`SingleFileReducer`](data.md#SingleFileReducer), [`reduce`](data.md#FileKeepReducer.reduce), [`reduce`](data.md#FileReducer.reduce), [`reduce`](data.md#FolderReducer.reduce), [`FolderReducer`](data.md#FolderReducer), [`FileKeepReducer`](data.md#FileKeepReducer), [`FileReducer`](data.md#FileReducer), [`JsonReducer`](data.md#JsonReducer), [`RandDataReducer`](data.md#RandDataReducer), [`UniqueIDDataReducer`](data.md#UniqueIDDataReducer), [`reduce`](data.md#SingleFileReducer.reduce)
- used by: [`sample`](data.md#DefaultSampler.sample), [`map_competition`](data.md#map_competition), [`reduce`](data.md#UniqueIDDataReducer.reduce), [`reduce`](data.md#JsonReducer.reduce), [`reduce`](data.md#RandDataReducer.reduce), [`_sample_list`](data.md#JsonReducer._sample_list), [`SingleFileReducer`](data.md#SingleFileReducer), [`reduce`](data.md#FileKeepReducer.reduce), [`reduce`](data.md#FileReducer.reduce), [`reduce`](data.md#FolderReducer.reduce), [`FolderReducer`](data.md#FolderReducer), [`FileKeepReducer`](data.md#FileKeepReducer), [`FileReducer`](data.md#FileReducer), [`JsonReducer`](data.md#JsonReducer), [`RandDataReducer`](data.md#RandDataReducer), [`UniqueIDDataReducer`](data.md#UniqueIDDataReducer), [`reduce`](data.md#SingleFileReducer.reduce)

### `DataSampler`
- def: [`rdagent/scenarios/data_science/debug/data.py:306`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L306)
- doc: Base DataSampler interface.
- signature: `class DataSampler:`
- members:
  - `sample(self)` — [`L316`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L316)
  - `data_folder` — [`L310`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L310)
  - `data_handler` — [`L314`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L314)
  - `data_reducer` — [`L312`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L312)
  - `included_extensions` — [`L313`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L313)
  - `sample_folder` — [`L311`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L311)
- protocol/private: `__init__`[`L309`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L309)
- uses (calls/refs, reference-scoped): [`sample`](data.md#DefaultSampler.sample), [`sample`](data.md#FolderSampler.sample), [`sample`](data.md#SingleFilePerFolderSampler.sample), [`FolderSampler`](data.md#FolderSampler), [`SingleFilePerFolderSampler`](data.md#SingleFilePerFolderSampler), [`DefaultSampler`](data.md#DefaultSampler), [`GenericDataHandler`](data.md#GenericDataHandler)
- used by: [`sample`](data.md#DefaultSampler.sample), [`map_competition`](data.md#map_competition), [`sample`](data.md#FolderSampler.sample), [`sample`](data.md#SingleFilePerFolderSampler.sample), [`FolderSampler`](data.md#FolderSampler), [`SingleFilePerFolderSampler`](data.md#SingleFilePerFolderSampler), [`DefaultSampler`](data.md#DefaultSampler)

### `DefaultSampler`  ·  implements/extends DataSampler
- def: [`rdagent/scenarios/data_science/debug/data.py:320`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L320)
- signature: `class DefaultSampler(DataSampler):`
- members:
  - `sample(self)` — [`L321`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L321)
- uses (calls/refs, reference-scoped): [`data_folder`](data.md#DataSampler.data_folder), [`reduce`](data.md#JsonReducer.reduce), [`DataSampler`](data.md#DataSampler), [`min_frac`](data.md#DataReducer.min_frac), [`sample_folder`](data.md#DataSampler.sample_folder), [`data_reducer`](data.md#DataSampler.data_reducer), [`min_num`](data.md#DataReducer.min_num), [`copy_file`](data.md#copy_file), [`data_handler`](data.md#DataSampler.data_handler), [`JsonReducer`](data.md#JsonReducer), [`included_extensions`](data.md#DataSampler.included_extensions), [`sampled_files`](data.md#DataReducer.sampled_files), [`count_files_in_folder`](data.md#count_files_in_folder), [`dump`](data.md#GenericDataHandler.dump), [`load`](data.md#GenericDataHandler.load)
- used by: [`map_competition`](data.md#map_competition), [`DataSampler`](data.md#DataSampler), [`sample`](data.md#DataSampler.sample)

### `FileKeepReducer`  ·  implements/extends DataReducer
- def: [`rdagent/scenarios/data_science/debug/data.py:158`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L158)
- doc: Sample file from a large number of files, keep min_num of files for each folder.
- signature: `class FileKeepReducer(DataReducer):`
- members:
  - `reduce(self, files: list[Path])` — [`L163`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L163)
- uses (calls/refs, reference-scoped): [`DataReducer`](data.md#DataReducer), [`min_frac`](data.md#DataReducer.min_frac), [`min_num`](data.md#DataReducer.min_num)
- used by: [`map_competition`](data.md#map_competition), [`DataReducer`](data.md#DataReducer), [`reduce`](data.md#DataReducer.reduce)

### `FileReducer`  ·  implements/extends DataReducer
- def: [`rdagent/scenarios/data_science/debug/data.py:141`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L141)
- doc: Sample file from a large number of files, keep min_num of files for each folder.
- signature: `class FileReducer(DataReducer):`
- members:
  - `reduce(self, files: list[Path])` — [`L146`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L146)
- uses (calls/refs, reference-scoped): [`DataReducer`](data.md#DataReducer), [`min_frac`](data.md#DataReducer.min_frac), [`min_num`](data.md#DataReducer.min_num)
- used by: [`map_competition`](data.md#map_competition), [`DataReducer`](data.md#DataReducer), [`reduce`](data.md#DataReducer.reduce)

### `FolderReducer`  ·  implements/extends DataReducer
- def: [`rdagent/scenarios/data_science/debug/data.py:119`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L119)
- doc: Sample folder from a large number of folders.
- signature: `class FolderReducer(DataReducer):`
- members:
  - `reduce(self, array: list, frac: float = None)` — [`L124`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L124)
- uses (calls/refs, reference-scoped): [`DataReducer`](data.md#DataReducer), [`min_frac`](data.md#DataReducer.min_frac), [`min_num`](data.md#DataReducer.min_num)
- used by: [`map_competition`](data.md#map_competition), [`DataReducer`](data.md#DataReducer), [`reduce`](data.md#DataReducer.reduce)

### `FolderSampler`  ·  implements/extends DataSampler
- def: [`rdagent/scenarios/data_science/debug/data.py:467`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L467)
- doc: Sample data from a large number of folders.
- signature: `class FolderSampler(DataSampler):`
- members:
  - `sample(self)` — [`L472`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L472)
- uses (calls/refs, reference-scoped): [`data_folder`](data.md#DataSampler.data_folder), [`DataSampler`](data.md#DataSampler), [`sample_folder`](data.md#DataSampler.sample_folder), [`data_reducer`](data.md#DataSampler.data_reducer), [`copy_file`](data.md#copy_file), [`copy_folder`](data.md#copy_folder)
- used by: [`map_competition`](data.md#map_competition), [`DataSampler`](data.md#DataSampler), [`sample`](data.md#DataSampler.sample)

### `GenericDataHandler`  ·  implements/extends DataHandler
- def: [`rdagent/scenarios/data_science/debug/data.py:28`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L28)
- doc: A generic data handler that automatically detects file type based on suffix
- signature: `class GenericDataHandler(DataHandler):`
- members:
  - `dump(self, df: pd.DataFrame | dict, path)` — [`L65`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L65)
  - `load(self, path)` — [`L34`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L34)
- uses (calls/refs, reference-scoped): [`DataHandler`](data.md#DataHandler)
- used by: [`sample`](data.md#DefaultSampler.sample), [`data_handler`](data.md#DataSampler.data_handler), [`DataHandler`](data.md#DataHandler), [`dump`](data.md#DataHandler.dump), [`load`](data.md#DataHandler.load)

### `JsonReducer`  ·  implements/extends DataReducer
- def: [`rdagent/scenarios/data_science/debug/data.py:237`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L237)
- signature: `class JsonReducer(DataReducer):`
- members:
  - `_find_all_lists(self, current: Any, parent: Union[Dict, List, None], key: Union[str, int, None], out: List[Tuple[Union[Dict, List], Union[str, int], List[Any]]])` — [`L274`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L274) — out => (parent_container, key_or_index, the_list)。
  - `extract_filename(self, item: Any)` — [`L239`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L239)
  - `reduce(self, data: dict)` — [`L255`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L255) — 1. 找到最大列表
- protocol/private: `_sample_list`[`L299`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L299)
- uses (calls/refs, reference-scoped): [`DataReducer`](data.md#DataReducer), [`min_frac`](data.md#DataReducer.min_frac), [`min_num`](data.md#DataReducer.min_num), [`sampled_files`](data.md#DataReducer.sampled_files)
- used by: [`sample`](data.md#DefaultSampler.sample), [`DataReducer`](data.md#DataReducer), [`reduce`](data.md#DataReducer.reduce)

### `RandDataReducer`  ·  implements/extends DataReducer
- def: [`rdagent/scenarios/data_science/debug/data.py:105`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L105)
- doc: Example random sampler: ensures at least `min_num` rows
- signature: `class RandDataReducer(DataReducer):`
- members:
  - `reduce(self, df: pd.DataFrame, frac: float = None)` — [`L111`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L111)
- uses (calls/refs, reference-scoped): [`DataReducer`](data.md#DataReducer), [`min_frac`](data.md#DataReducer.min_frac), [`min_num`](data.md#DataReducer.min_num)
- used by: [`DataReducer`](data.md#DataReducer), [`reduce`](data.md#DataReducer.reduce), [`reduce`](data.md#UniqueIDDataReducer.reduce)

### `SingleFilePerFolderSampler`  ·  implements/extends DataSampler
- def: [`rdagent/scenarios/data_science/debug/data.py:520`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L520)
- doc: For each leaf (final) subfolder under data_folder, keep exactly one file (randomly chosen).
- signature: `class SingleFilePerFolderSampler(DataSampler):`
- members:
  - `sample(self)` — [`L526`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L526)
- uses (calls/refs, reference-scoped): [`data_folder`](data.md#DataSampler.data_folder), [`DataSampler`](data.md#DataSampler), [`sample_folder`](data.md#DataSampler.sample_folder), [`data_reducer`](data.md#DataSampler.data_reducer), [`copy_file`](data.md#copy_file)
- used by: [`map_competition`](data.md#map_competition), [`DataSampler`](data.md#DataSampler), [`sample`](data.md#DataSampler.sample)

### `SingleFileReducer`  ·  implements/extends DataReducer
- def: [`rdagent/scenarios/data_science/debug/data.py:181`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L181)
- doc: Sample file from a large number of files, keep at least 1 file.
- signature: `class SingleFileReducer(DataReducer):`
- members:
  - `reduce(self, files: list[Path])` — [`L186`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L186)
- uses (calls/refs, reference-scoped): [`DataReducer`](data.md#DataReducer), [`min_frac`](data.md#DataReducer.min_frac)
- used by: [`map_competition`](data.md#map_competition), [`DataReducer`](data.md#DataReducer), [`reduce`](data.md#DataReducer.reduce)

### `UniqueIDDataReducer`  ·  implements/extends DataReducer
- def: [`rdagent/scenarios/data_science/debug/data.py:191`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L191)
- signature: `class UniqueIDDataReducer(DataReducer):`
- members:
  - `is_valid_label(column)` — [`L200`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L200)
  - `reduce(self, df: pd.DataFrame)` — [`L192`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L192)
- uses (calls/refs, reference-scoped): [`DataReducer`](data.md#DataReducer), [`min_frac`](data.md#DataReducer.min_frac), [`min_num`](data.md#DataReducer.min_num), [`reduce`](data.md#RandDataReducer.reduce), [`RandDataReducer`](data.md#RandDataReducer)
- used by: [`map_competition`](data.md#map_competition), [`DataReducer`](data.md#DataReducer), [`reduce`](data.md#DataReducer.reduce)

## Functions
- `copy_file(src_fp, target_folder, data_folder)` — [`L558`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L558) — Construct the target file path based on the file's relative location from data_folder,
- `copy_folder(src_fp, target_folder, data_folder)` — [`L569`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L569) — Copy a folder recursively.
- `count_files_in_folder(files_to_process)` — [`L579`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L579) — Count the number of each file type in a folder, including files in subfolders.
- `create_debug_data(competition: str, dataset_path: str | Path, min_frac=0.01, min_num=5, sample_path=None)` — [`L605`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L605) — Reads the original data file, creates a reduced sample,
- `map_competition(competition: str)` — [`L592`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/data_science/debug/data.py#L592)

