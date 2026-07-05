---
title: 'Module: test/utils/test_kaggle.py'
type: catalog
provenance: extracted
module: test/utils/test_kaggle.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `test.utils.test_kaggle`/TestTpl#
symbols:
  TestTpl.test_competition_template: test_competition_template().
  TestTpl: ''
---
# Module: [`test/utils/test_kaggle.py`](../../../../../../raw/code/rd-agent/test/utils/test_kaggle.py)

## Classes
### `TestTpl`  ·  implements/extends TestCase
- def: [`test/utils/test_kaggle.py:11`](../../../../../../raw/code/rd-agent/test/utils/test_kaggle.py#L11)
- signature: `class TestTpl(unittest.TestCase):`
- members:
  - `test_competition_template(self)` — [`L12`](../../../../../../raw/code/rd-agent/test/utils/test_kaggle.py#L12) — export KG_COMPETITION=<competition_name> before running this test
- uses (calls/refs, reference-scoped): [`workspace_path`](../../rdagent/core/experiment.md#FBWorkspace.workspace_path), [`KAGGLE_IMPLEMENT_SETTING`](../../rdagent/app/kaggle/conf.md#KAGGLE_IMPLEMENT_SETTING), [`execute`](../../rdagent/scenarios/kaggle/experiment/workspace.md#KGFBWorkspace.execute), [`download_data`](../../rdagent/scenarios/kaggle/kaggle_crawler.md#download_data), [`competition`](../../rdagent/app/kaggle/conf.md#KaggleBasePropSetting.competition), [`KGFBWorkspace`](../../rdagent/scenarios/kaggle/experiment/workspace.md#KGFBWorkspace), [`template_path`](../../rdagent/app/kaggle/conf.md#KaggleBasePropSetting.template_path)

