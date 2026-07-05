---
title: 'Module: polyglot/test_spec.py'
type: catalog
provenance: extracted
module: polyglot/test_spec.py
status: fresh
symbol_base: scip-python python dgm 0.0.0 `polyglot.test_spec`/
symbols:
  make_test_spec: make_test_spec().
  TestSpec.env_image_key: TestSpec#env_image_key().
  TestSpec.instance_id: TestSpec#instance_id.
  TestSpec: TestSpec#
  TestSpec.instance_image_key: TestSpec#instance_image_key().
  TestSpec.platform: TestSpec#platform().
  TestSpec.arch: TestSpec#arch.
  get_test_specs_from_dataset: get_test_specs_from_dataset().
  TestSpec.base_image_key: TestSpec#base_image_key().
  TestSpec.base_dockerfile: TestSpec#base_dockerfile().
  TestSpec.env_dockerfile: TestSpec#env_dockerfile().
  TestSpec.instance_dockerfile: TestSpec#instance_dockerfile().
  make_eval_script_list: make_eval_script_list().
  TestSpec.get_instance_container_name: TestSpec#get_instance_container_name().
  TestSpec.setup_env_script: TestSpec#setup_env_script().
  TestSpec.install_repo_script: TestSpec#install_repo_script().
  make_repo_script_list: make_repo_script_list().
  make_env_script_list: make_env_script_list().
  TestSpec.env_script_list: TestSpec#env_script_list.
  TestSpec.eval_script: TestSpec#eval_script().
  TestSpec.repo: TestSpec#repo.
  TestSpec.repo_script_list: TestSpec#repo_script_list.
  TestSpec.eval_script_list: TestSpec#eval_script_list.
  DIFF_MODIFIED_FILE_REGEX: DIFF_MODIFIED_FILE_REGEX.
  replace_uninstallable_packages_requirements_txt: replace_uninstallable_packages_requirements_txt().
---
# Module: [`polyglot/test_spec.py`](../../../../../raw/code/dgm/polyglot/test_spec.py)

## Classes
### `TestSpec`
- def: [`polyglot/test_spec.py:33`](../../../../../raw/code/dgm/polyglot/test_spec.py#L33) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- doc: A dataclass that represents a test specification for a single instance of polyglot.
- signature: `class TestSpec:`
- members:
  - `base_dockerfile(self)` — [`L85`](../../../../../raw/code/dgm/polyglot/test_spec.py#L85) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `base_image_key(self)` — [`L58`](../../../../../raw/code/dgm/polyglot/test_spec.py#L58) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `env_dockerfile(self)` — [`L89`](../../../../../raw/code/dgm/polyglot/test_spec.py#L89) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `env_image_key(self)` — [`L62`](../../../../../raw/code/dgm/polyglot/test_spec.py#L62) — The key for the environment image is based on the hash of the environment script list. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `eval_script(self)` — [`L49`](../../../../../raw/code/dgm/polyglot/test_spec.py#L49)
  - `get_instance_container_name(self, run_id=None)` — [`L79`](../../../../../raw/code/dgm/polyglot/test_spec.py#L79) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `install_repo_script(self)` — [`L54`](../../../../../raw/code/dgm/polyglot/test_spec.py#L54) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `instance_dockerfile(self)` — [`L93`](../../../../../raw/code/dgm/polyglot/test_spec.py#L93)
  - `instance_image_key(self)` — [`L76`](../../../../../raw/code/dgm/polyglot/test_spec.py#L76) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `platform(self)` — [`L97`](../../../../../raw/code/dgm/polyglot/test_spec.py#L97)
  - `setup_env_script(self)` — [`L45`](../../../../../raw/code/dgm/polyglot/test_spec.py#L45) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `arch` — [`L42`](../../../../../raw/code/dgm/polyglot/test_spec.py#L42)
  - `env_script_list` — [`L41`](../../../../../raw/code/dgm/polyglot/test_spec.py#L41)
  - `eval_script_list` — [`L40`](../../../../../raw/code/dgm/polyglot/test_spec.py#L40)
  - `instance_id` — [`L37`](../../../../../raw/code/dgm/polyglot/test_spec.py#L37)
  - `repo` — [`L38`](../../../../../raw/code/dgm/polyglot/test_spec.py#L38) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
  - `repo_script_list` — [`L39`](../../../../../raw/code/dgm/polyglot/test_spec.py#L39)
- uses (calls/refs, reference-scoped): [`get_dockerfile_base`](dockerfiles.md#get_dockerfile_base), [`get_dockerfile_env`](dockerfiles.md#get_dockerfile_env), [`get_dockerfile_instance`](dockerfiles.md#get_dockerfile_instance)
- used by: [`build_instance_image`](docker_build.md#build_instance_image), [`process_entry`](harness.md#process_entry), [`build_container`](docker_build.md#build_container), [`build_env_images`](docker_build.md#build_env_images), [`get_env_configs_to_build`](docker_build.md#get_env_configs_to_build), [`build_instance_images`](docker_build.md#build_instance_images), [`build_base_images`](docker_build.md#build_base_images)  (2 test-only)

## Functions
- `get_test_specs_from_dataset(dataset: Union[list[dict], list[TestSpec]])` — [`L106`](../../../../../raw/code/dgm/polyglot/test_spec.py#L106) — Idempotent function that converts a list of SWEbenchInstance objects to a list of TestSpec objects. — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `make_env_script_list(instance: dict, specs: dict, env_name: str)` — [`L165`](../../../../../raw/code/dgm/polyglot/test_spec.py#L165) — Creates the list of commands to set up the conda environment for testing.
- `make_eval_script_list(instance, specs, env_name, repo_directory, base_commit, test_patch)` — [`L233`](../../../../../raw/code/dgm/polyglot/test_spec.py#L233) — Applies the test patch and runs the tests.
- `make_repo_script_list(specs, repo, repo_directory, base_commit, env_name)` — [`L115`](../../../../../raw/code/dgm/polyglot/test_spec.py#L115) — Create a list of bash commands to set up the repository for testing.
- `make_test_spec(instance: dict)` — [`L290`](../../../../../raw/code/dgm/polyglot/test_spec.py#L290) — documented in [polyglot-docker_build](../../concepts/polyglot-docker_build.md)
- `replace_uninstallable_packages_requirements_txt(requirement_str: str)` — [`L144`](../../../../../raw/code/dgm/polyglot/test_spec.py#L144) — Replaces certain packages in a requirements.txt-like string.

## Module values
- `DIFF_MODIFIED_FILE_REGEX` — [`L29`](../../../../../raw/code/dgm/polyglot/test_spec.py#L29)

