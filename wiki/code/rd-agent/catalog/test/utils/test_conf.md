---
title: 'Module: test/utils/test_conf.py'
type: catalog
provenance: extracted
module: test/utils/test_conf.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.utils.test_conf`/ConfUtils#
symbols:
  ConfUtils.test_conf: test_conf().
  ConfUtils.test_ds_costeer_conf: test_ds_costeer_conf().
  ConfUtils: ''
---
# Module: [`test/utils/test_conf.py`](../../../../../../raw/code/rd-agent/test/utils/test_conf.py)

## Classes
### `ConfUtils`  ·  implements/extends TestCase
- def: [`test/utils/test_conf.py:10`](../../../../../../raw/code/rd-agent/test/utils/test_conf.py#L10)
- signature: `class ConfUtils(unittest.TestCase):`
- members:
  - `test_conf(self)` — [`L12`](../../../../../../raw/code/rd-agent/test/utils/test_conf.py#L12)
  - `test_ds_costeer_conf(self)` — [`L31`](../../../../../../raw/code/rd-agent/test/utils/test_conf.py#L31)
- uses (calls/refs, reference-scoped): [`DSCoderCoSTEERSettings`](../../rdagent/components/coder/data_science/conf.md#DSCoderCoSTEERSettings), [`QlibDockerConf`](../../rdagent/utils/env.md#QlibDockerConf), [`EnvConf`](../../rdagent/utils/env.md#EnvConf), [`DSRunnerCoSTEERSettings`](../../rdagent/scenarios/data_science/dev/runner/__init__.md#DSRunnerCoSTEERSettings), [`mem_limit`](../../rdagent/utils/env.md#DockerConf.mem_limit), [`running_timeout_period`](../../rdagent/utils/env.md#DockerConf.running_timeout_period), [`enable_cache`](../../rdagent/utils/env.md#EnvConf.enable_cache), [`enable_cache`](../../rdagent/utils/env.md#QlibDockerConf.enable_cache), [`max_seconds_multiplier`](../../rdagent/components/coder/data_science/conf.md#DSCoderCoSTEERSettings.max_seconds_multiplier), [`max_seconds_multiplier`](../../rdagent/scenarios/data_science/dev/runner/__init__.md#DSRunnerCoSTEERSettings.max_seconds_multiplier)

