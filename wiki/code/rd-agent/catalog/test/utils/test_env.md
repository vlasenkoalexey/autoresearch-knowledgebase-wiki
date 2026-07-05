---
title: 'Module: test/utils/test_env.py'
type: catalog
provenance: extracted
module: test/utils/test_env.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.utils.test_env`/
symbols:
  EnvUtils.test_local_simple: EnvUtils#test_local_simple().
  EnvUtils.test_conda_simple: EnvUtils#test_conda_simple().
  EnvUtils.test_conda_error: EnvUtils#test_conda_error().
  EnvUtils.test_run: EnvUtils#test_run().
  EnvUtils.test_local: EnvUtils#test_local().
  EnvUtils.test_docker_mem: EnvUtils#test_docker_mem().
  DIRNAME: DIRNAME.
  EnvUtils.test_docker: EnvUtils#test_docker().
  EnvUtils.test_workspace: EnvUtils#test_workspace.
  EnvUtils.setUp: EnvUtils#setUp().
  QlibLocalEnv: QlibLocalEnv#
  QlibLocalEnv.prepare: QlibLocalEnv#prepare().
  EnvUtils.tearDown: EnvUtils#tearDown().
  EnvUtils.test_cleanup_container_import: EnvUtils#test_cleanup_container_import().
  EnvUtils: EnvUtils#
---
# Module: [`test/utils/test_env.py`](../../../../../../raw/code/rd-agent/test/utils/test_env.py)

## Classes
### `EnvUtils`  ·  implements/extends TestCase
- def: [`test/utils/test_env.py:32`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L32)
- signature: `class EnvUtils(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L33`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L33)
  - `tearDown(self)` — [`L37`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L37)
  - `test_cleanup_container_import(self)` — [`L146`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L146) — Test that cleanup_container function can be imported and has correct interface.
  - `test_conda_error(self)` — [`L78`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L78) — documented in [rdagent-utils-env](../../../concepts/rdagent-utils-env.md)
  - `test_conda_simple(self)` — [`L69`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L69)
  - `test_docker(self)` — [`L89`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L89) — We will mount `env_tpl` into the docker image.
  - `test_docker_mem(self)` — [`L129`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L129)
  - `test_local(self)` — [`L43`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L43)
  - `test_local_simple(self)` — [`L55`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L55)
  - `test_run(self)` — [`L106`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L106) — Test the run method of QTDockerEnv with both valid and invalid commands. — documented in [rdagent-utils-env](../../../concepts/rdagent-utils-env.md)
  - `test_workspace` — [`L34`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L34)
- uses (calls/refs, reference-scoped): [`run`](../../rdagent/utils/env.md#Env.run), [`exit_code`](../../rdagent/utils/env.md#EnvResult.exit_code), [`stdout`](../../rdagent/utils/env.md#EnvResult.stdout), [`LocalEnv`](../../rdagent/utils/env.md#LocalEnv), [`check_output`](../../rdagent/utils/env.md#Env.check_output), [`CondaConf`](../../rdagent/utils/env.md#CondaConf), [`prepare`](../../rdagent/utils/env.md#QTDockerEnv.prepare), [`QTDockerEnv`](../../rdagent/utils/env.md#QTDockerEnv), [`cleanup_container`](../../rdagent/utils/env.md#cleanup_container), [`prepare`](../../rdagent/utils/env.md#LocalEnv.prepare), [`QlibDockerConf`](../../rdagent/utils/env.md#QlibDockerConf), [`LocalConf`](../../rdagent/utils/env.md#LocalConf), [`running_time`](../../rdagent/utils/env.md#EnvResult.running_time), [`bin_path`](../../rdagent/utils/env.md#LocalConf.bin_path), [`conda_env_name`](../../rdagent/utils/env.md#CondaConf.conda_env_name), [`extra_volumes`](../../rdagent/utils/env.md#EnvConf.extra_volumes), [`mem_limit`](../../rdagent/utils/env.md#DockerConf.mem_limit), [`running_timeout_period`](../../rdagent/utils/env.md#DockerConf.running_timeout_period), [`default_entry`](../../rdagent/utils/env.md#EnvConf.default_entry), [`default_entry`](../../rdagent/utils/env.md#CondaConf.default_entry)  (3 test-only)

### `QlibLocalEnv`  ·  implements/extends LocalEnv
- def: [`test/utils/test_env.py:22`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L22)
- signature: `class QlibLocalEnv(LocalEnv):`
- members:
  - `prepare(self)` — [`L23`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L23)
- uses (calls/refs, reference-scoped): [`LocalEnv`](../../rdagent/utils/env.md#LocalEnv), [`check_output`](../../rdagent/utils/env.md#Env.check_output)
- used by: [`LocalEnv`](../../rdagent/utils/env.md#LocalEnv), [`prepare`](../../rdagent/utils/env.md#LocalEnv.prepare)  (1 test-only)

## Module values
- `DIRNAME` — [`L19`](../../../../../../raw/code/rd-agent/test/utils/test_env.py#L19)

