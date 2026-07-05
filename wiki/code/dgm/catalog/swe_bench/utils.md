---
title: 'Module: swe_bench/utils.py'
type: catalog
provenance: extracted
module: swe_bench/utils.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `swe_bench.utils`/
symbols:
  copy_to_container: copy_to_container().
  log_container_output: log_container_output().
  safe_log: safe_log().
  copy_from_container: copy_from_container().
  setup_logger: setup_logger().
  remove_existing_container: remove_existing_container().
  get_thread_logger: get_thread_logger().
  _thread_local: _thread_local.
  create_archive: create_archive().
---
# Module: [`swe_bench/utils.py`](../../../../../raw/code/dgm/swe_bench/utils.py)

## Functions
- `copy_from_container(container, source_path: Union[str, Path], dest_path: Union[str, Path])` — [`L151`](../../../../../raw/code/dgm/swe_bench/utils.py#L151) — Copy a file or directory from a Docker container to the local system.
- `copy_to_container(container, source_path: Union[str, Path], dest_path: Union[str, Path])` — [`L104`](../../../../../raw/code/dgm/swe_bench/utils.py#L104) — Copy a file or directory from the local system to a Docker container.
- `create_archive(path: Union[str, Path], data: Optional[bytes] = None)` — [`L77`](../../../../../raw/code/dgm/swe_bench/utils.py#L77) — Create a tar archive containing either file data or a directory structure.
- `get_thread_logger()` — [`L12`](../../../../../raw/code/dgm/swe_bench/utils.py#L12) — Get the logger instance specific to the current thread.
- `log_container_output(exec_result, raise_error=True)` — [`L214`](../../../../../raw/code/dgm/swe_bench/utils.py#L214) — Log output from a Docker container execution, handling both streaming and non-streaming cases.
- `remove_existing_container(client, container_name)` — [`L61`](../../../../../raw/code/dgm/swe_bench/utils.py#L61) — Check if a container with the specified name exists, and remove it if so.
- `safe_log(message: str, level: int = logging.INFO)` — [`L53`](../../../../../raw/code/dgm/swe_bench/utils.py#L53) — Thread-safe logging function.
- `setup_logger(log_file)` — [`L16`](../../../../../raw/code/dgm/swe_bench/utils.py#L16) — Set up a thread-safe logger with file handler.

## Module values
- `_thread_local` — [`L10`](../../../../../raw/code/dgm/swe_bench/utils.py#L10)

