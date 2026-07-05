---
title: 'Module: polyglot/docker_utils.py'
type: catalog
provenance: extracted
module: polyglot/docker_utils.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `polyglot.docker_utils`/
symbols:
  remove_image: remove_image().
  clean_images: clean_images().
  cleanup_container: cleanup_container().
  exec_run_with_timeout: exec_run_with_timeout().
  list_images: list_images().
  copy_to_container: copy_to_container().
  should_remove: should_remove().
  write_to_container: write_to_container().
  HEREDOC_DELIMITER: HEREDOC_DELIMITER.
  find_dependent_images: find_dependent_images().
  exec_run_with_timeout.run_command: exec_run_with_timeout().run_command().
---
# Module: [`polyglot/docker_utils.py`](../../../../../raw/code/dgm/polyglot/docker_utils.py)

## Functions
- `clean_images(client: docker.DockerClient, prior_images: set, cache_level: str, clean: bool)` — [`L269`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L269) — Clean Docker images based on cache level and clean flag.
- `cleanup_container(client, container, logger)` — [`L103`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L103) — Stop and remove a Docker container. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `copy_to_container(container: Container, src: Path, dst: Path)` — [`L19`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L19) — Copy a file from local to a docker container
- `exec_run_with_timeout(container, cmd, timeout: int | None = 60)` — [`L178`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L178) — Run a command in a container with a timeout.
- `find_dependent_images(client: docker.DockerClient, image_name: str)` — [`L223`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L223) — Find all images that are built upon `image_name` image — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `list_images(client: docker.DockerClient)` — [`L261`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L261) — List all images from the Docker client.
- `remove_image(client, image_id, logger=None)` — [`L64`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L64) — Remove a Docker image by ID.
- `run_command()` — [`L194`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L194)
- `should_remove(image_name: str, cache_level: str, clean: bool, prior_images: set)` — [`L301`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L301) — Determine if an image should be removed based on cache level and clean flag.
- `write_to_container(container: Container, data: str, dst: Path)` — [`L55`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L55) — Write a string to a file in a docker container

## Module values
- `HEREDOC_DELIMITER` — [`L17`](../../../../../raw/code/dgm/polyglot/docker_utils.py#L17)

