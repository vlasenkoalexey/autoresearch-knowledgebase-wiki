---
title: 'Module: test/utils/test_ws.py'
type: catalog
provenance: extracted
module: test/utils/test_ws.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.utils.test_ws`/TestFBWorkspace#
symbols:
  TestFBWorkspace.test_checkpoint_roundtrip: test_checkpoint_roundtrip().
  TestFBWorkspace.tmp_path: tmp_path.
  TestFBWorkspace.tearDown: tearDown().
  TestFBWorkspace._tmp_dir: _tmp_dir.
  TestFBWorkspace: ''
  TestFBWorkspace.setUp: setUp().
---
# Module: [`test/utils/test_ws.py`](../../../../../../raw/code/rd-agent/test/utils/test_ws.py)

## Classes
### `TestFBWorkspace`  ·  implements/extends TestCase
- def: [`test/utils/test_ws.py:9`](../../../../../../raw/code/rd-agent/test/utils/test_ws.py#L9)
- doc: Unit-tests for `FBWorkspace`.
- signature: `class TestFBWorkspace(unittest.TestCase):`
- members:
  - `setUp(self)` — [`L14`](../../../../../../raw/code/rd-agent/test/utils/test_ws.py#L14) — Create an isolated temporary directory for each test case.
  - `tearDown(self)` — [`L21`](../../../../../../raw/code/rd-agent/test/utils/test_ws.py#L21) — Clean up the temporary directory created in :py:meth:`setUp`.
  - `test_checkpoint_roundtrip(self)` — [`L27`](../../../../../../raw/code/rd-agent/test/utils/test_ws.py#L27) — Verify that ``create_ws_ckp`` captures the current workspace state and
  - `tmp_path` — [`L19`](../../../../../../raw/code/rd-agent/test/utils/test_ws.py#L19)
- protocol/private: `_tmp_dir`[`L18`](../../../../../../raw/code/rd-agent/test/utils/test_ws.py#L18)
- uses (calls/refs, reference-scoped): [`FBWorkspace`](../../rdagent/core/experiment.md#FBWorkspace), [`workspace_path`](../../rdagent/core/experiment.md#FBWorkspace.workspace_path), [`RD_AGENT_SETTINGS`](../../rdagent/core/conf.md#RD_AGENT_SETTINGS), [`inject_files`](../../rdagent/core/experiment.md#FBWorkspace.inject_files), [`create_ws_ckp`](../../rdagent/core/experiment.md#FBWorkspace.create_ws_ckp), [`prepare`](../../rdagent/core/experiment.md#FBWorkspace.prepare), [`recover_ws_ckp`](../../rdagent/core/experiment.md#FBWorkspace.recover_ws_ckp), [`ws_ckp`](../../rdagent/core/experiment.md#FBWorkspace.ws_ckp), [`workspace_ckp_size_limit`](../../rdagent/core/conf.md#RDAgentSettings.workspace_ckp_size_limit)

