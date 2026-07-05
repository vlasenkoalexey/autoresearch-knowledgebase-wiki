---
title: 'Module: polyglot/docker_build.py'
type: catalog
provenance: extracted
module: polyglot/docker_build.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `polyglot.docker_build`/
symbols:
  build_instance_image: build_instance_image().
  build_container: build_container().
  build_env_images: build_env_images().
  get_env_configs_to_build: get_env_configs_to_build().
  build_instance_images: build_instance_images().
  build_base_images: build_base_images().
  build_image: build_image().
  BuildImageError: BuildImageError#
  BuildImageError.__str__: BuildImageError#__str__().
  setup_logger: setup_logger().
  close_logger: close_logger().
  BuildImageError.image_name: BuildImageError#image_name.
  ansi_escape: ansi_escape.
  BuildImageError.super_str: BuildImageError#super_str.
  BuildImageError.__init__: BuildImageError#__init__().
  BuildImageError.logger: BuildImageError#logger.
---
# Module: [`polyglot/docker_build.py`](../../../../../raw/code/dgm/polyglot/docker_build.py)

## Classes
### `BuildImageError`  ·  implements/extends Exception
- def: [`polyglot/docker_build.py:35`](../../../../../raw/code/dgm/polyglot/docker_build.py#L35) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- signature: `class BuildImageError(Exception):`
- members:
  - `image_name` — [`L39`](../../../../../raw/code/dgm/polyglot/docker_build.py#L39) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `logger` — [`L41`](../../../../../raw/code/dgm/polyglot/docker_build.py#L41)
  - `super_str` — [`L38`](../../../../../raw/code/dgm/polyglot/docker_build.py#L38)
- protocol/private: `__init__`[`L36`](../../../../../raw/code/dgm/polyglot/docker_build.py#L36), `__str__`[`L43`](../../../../../raw/code/dgm/polyglot/docker_build.py#L43)
- used by: [`build_instance_image`](docker_build.md#build_instance_image), [`build_container`](docker_build.md#build_container), [`build_env_images`](docker_build.md#build_env_images), [`run_instance`](run_evaluation.md#run_instance), [`build_instance_images`](docker_build.md#build_instance_images), [`build_image`](docker_build.md#build_image)

## Functions
- `build_base_images(client: docker.DockerClient, dataset: list, force_rebuild: bool = False)` — [`L171`](../../../../../raw/code/dgm/polyglot/docker_build.py#L171) — Builds the base images required for the dataset if they do not already exist. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `build_container(test_spec: TestSpec, client: docker.DockerClient, run_id: str, logger: logging.Logger, nocache: bool, force_rebuild: bool = False)` — [`L499`](../../../../../raw/code/dgm/polyglot/docker_build.py#L499) — Builds the instance image for the given test spec and creates a container from the image. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `build_env_images(client: docker.DockerClient, dataset: list, force_rebuild: bool = False, max_workers: int = 4)` — [`L274`](../../../../../raw/code/dgm/polyglot/docker_build.py#L274) — Builds the environment images required for the dataset if they do not already exist. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `build_image(image_name: str, setup_scripts: dict, dockerfile: str, platform: str, client: docker.DockerClient, build_dir: Path, repo: str = None, nocache: bool = False)` — [`L74`](../../../../../raw/code/dgm/polyglot/docker_build.py#L74) — Builds a docker image with the given name, setup scripts, dockerfile, and platform. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `build_instance_image(test_spec: TestSpec, client: docker.DockerClient, logger: logging.Logger | None, nocache: bool)` — [`L424`](../../../../../raw/code/dgm/polyglot/docker_build.py#L424) — Builds the instance image for the given test spec if it does not already exist. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `build_instance_images(client: docker.DockerClient, dataset: list, force_rebuild: bool = False, max_workers: int = 4)` — [`L349`](../../../../../raw/code/dgm/polyglot/docker_build.py#L349) — Builds the instance images required for the dataset if they do not already exist. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `close_logger(logger)` — [`L67`](../../../../../raw/code/dgm/polyglot/docker_build.py#L67) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `get_env_configs_to_build(client: docker.DockerClient, dataset: list)` — [`L219`](../../../../../raw/code/dgm/polyglot/docker_build.py#L219) — Returns a dictionary of image names to build scripts and dockerfiles for environment images. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `setup_logger(instance_id: str, log_file: Path, mode="w")` — [`L50`](../../../../../raw/code/dgm/polyglot/docker_build.py#L50) — This logger is used for logging the build process of images and containers. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)

## Module values
- `ansi_escape` — [`L32`](../../../../../raw/code/dgm/polyglot/docker_build.py#L32)

