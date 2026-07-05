---
title: 'Module: utils/docker_utils.py'
type: catalog
provenance: extracted
module: utils/docker_utils.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `utils.docker_utils`/
symbols:
  safe_log: safe_log().
  log_container_output: log_container_output().
  copy_to_container: copy_to_container().
  setup_logger: setup_logger().
  cleanup_container: cleanup_container().
  copy_from_container: copy_from_container().
  remove_existing_container: remove_existing_container().
  build_dgm_container: build_dgm_container().
  get_thread_logger: get_thread_logger().
  _thread_local: _thread_local.
  create_archive: create_archive().
---
# Module: [`utils/docker_utils.py`](../../../../../raw/code/dgm/utils/docker_utils.py)

## Functions
- `build_dgm_container(client, repo_path='./', image_name='app', container_name='app-container', force_rebuild=False)` — [`L104`](../../../../../raw/code/dgm/utils/docker_utils.py#L104) — Build the Docker image for the dgm app and start a container from it. — documented in [self_improve_step](../../concepts/self_improve_step.md)
- `cleanup_container(container)` — [`L140`](../../../../../raw/code/dgm/utils/docker_utils.py#L140) — Stops and removes the specified Docker container. — documented in [self_improve_step](../../concepts/self_improve_step.md)
- `copy_from_container(container, source_path: Union[str, Path], dest_path: Union[str, Path])` — [`L196`](../../../../../raw/code/dgm/utils/docker_utils.py#L196) — Copy a file or directory from a Docker container to the local system. — documented in [self_improve_step](../../concepts/self_improve_step.md)
- `copy_to_container(container, source_path: Union[str, Path], dest_path: Union[str, Path])` — [`L149`](../../../../../raw/code/dgm/utils/docker_utils.py#L149) — Copy a file or directory from the local system to a Docker container. — documented in [self_improve_step](../../concepts/self_improve_step.md)
- `create_archive(path: Union[str, Path], data: Optional[bytes] = None)` — [`L77`](../../../../../raw/code/dgm/utils/docker_utils.py#L77) — Create a tar archive containing either file data or a directory structure.
- `get_thread_logger()` — [`L12`](../../../../../raw/code/dgm/utils/docker_utils.py#L12) — Get the logger instance specific to the current thread.
- `log_container_output(exec_result)` — [`L259`](../../../../../raw/code/dgm/utils/docker_utils.py#L259) — Log output from a Docker container execution, handling both streaming and non-streaming cases.
- `remove_existing_container(client, container_name)` — [`L61`](../../../../../raw/code/dgm/utils/docker_utils.py#L61) — Check if a container with the specified name exists, and remove it if so. — documented in [self_improve_step](../../concepts/self_improve_step.md)
- `safe_log(message: str, level: int = logging.INFO)` — [`L53`](../../../../../raw/code/dgm/utils/docker_utils.py#L53) — Thread-safe logging function.
- `setup_logger(log_file)` — [`L16`](../../../../../raw/code/dgm/utils/docker_utils.py#L16) — Set up a thread-safe logger with file handler.

## Module values
- `_thread_local` — [`L10`](../../../../../raw/code/dgm/utils/docker_utils.py#L10)

