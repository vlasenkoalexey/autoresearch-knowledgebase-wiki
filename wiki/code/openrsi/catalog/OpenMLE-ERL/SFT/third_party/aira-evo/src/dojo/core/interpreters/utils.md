---
title: 'Module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.third_party.aira-evo.src.dojo.core.interpreters.utils`/
symbols:
  logger: logger.
  extract_all_archives: extract_all_archives().
  prepare_configuration: prepare_configuration().
  copy_contents: copy_contents().
  _resolve_path: _resolve_path().
  _copy_file: _copy_file().
  _copy_directory: _copy_directory().
  remove_unwanted_items: remove_unwanted_items().
  extract_zip_file: extract_zip_file().
  flatten_directory_structure: flatten_directory_structure().
  get_next_log_index: get_next_log_index().
  display_configuration: display_configuration().
  get_custom_process_name: get_custom_process_name().
---
# Module: [`OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py)

## Functions
- `_copy_directory(src: Path, dst_dir: Path, use_symlinks: bool)` — [`L90`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L90) — Merge contents of the source directory into the destination directory.
- `_copy_file(src: Path, dst_dir: Path, use_symlinks: bool)` — [`L63`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L63) — Copy a single file to the destination directory.
- `_resolve_path(path_str: Union[str, Path], relative_to_parent: bool = False)` — [`L298`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L298) — Resolve a string or Path to an absolute Path.
- `copy_contents(source: Path, destination: Path, use_symlinks: bool = True)` — [`L41`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L41) — Copy contents from source to destination. If the source is a file, copy the file.
- `display_configuration(cfg: OmegaConf)` — [`L322`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L322) — Display the configuration in a formatted YAML style using rich.
- `extract_all_archives(path: Path)` — [`L193`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L193) — Extract all zip archives within the specified path and clean up the directories.
- `extract_zip_file(zip_path: Path, extract_to: Path)` — [`L146`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L146) — Extract a single zip file to the specified directory.
- `flatten_directory_structure(zip_output_dir: Path, expected_name: str)` — [`L166`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L166) — Flatten the directory structure if the extracted content is nested within a single directory.
- `get_custom_process_name()` — [`L35`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L35) — Simple function to extract id and rename process
- `get_next_log_index(directory: Path)` — [`L231`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L231) — Determine the next available index for naming log or workspace directories.
- `prepare_configuration(cfg: OmegaConf)` — [`L254`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L254) — Prepare and validate the configuration.
- `remove_unwanted_items(path: Path, patterns: Optional[list] = None)` — [`L122`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L122) — Remove unwanted files and directories based on specified patterns.

## Module values
- `logger` — [`L28`](../../../../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/third_party/aira-evo/src/dojo/core/interpreters/utils.py#L28)

