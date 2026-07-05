---
title: 'Module: rdagent/core/developer.py'
type: catalog
provenance: extracted
module: rdagent/core/developer.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.core.developer`/Developer#
symbols:
  Developer: ''
  Developer.develop: develop().
  Developer.scen: scen.
  Developer.__init__: __init__().
---
# Module: [`rdagent/core/developer.py`](../../../../../../raw/code/rd-agent/rdagent/core/developer.py)

## Classes
### `Developer`  ·  implements/extends ABC, Generic
- def: [`rdagent/core/developer.py:12`](../../../../../../raw/code/rd-agent/rdagent/core/developer.py#L12)
- signature: `class Developer(ABC, Generic[ASpecificExp]):`
- members:
  - `develop(self, exp: ASpecificExp)` — [`L17`](../../../../../../raw/code/rd-agent/rdagent/core/developer.py#L17) — Task Generator should take in an experiment.
  - `scen` — [`L14`](../../../../../../raw/code/rd-agent/rdagent/core/developer.py#L14)
- protocol/private: `__init__`[`L13`](../../../../../../raw/code/rd-agent/rdagent/core/developer.py#L13)
- uses (calls/refs, reference-scoped): [`Scenario`](scenario.md#Scenario), [`develop`](../scenarios/qlib/developer/factor_runner.md#QlibFactorRunner.develop), [`develop`](../scenarios/qlib/developer/model_runner.md#QlibModelRunner.develop), [`develop`](../scenarios/kaggle/developer/runner.md#KGFactorRunner.develop), [`develop`](../scenarios/kaggle/developer/runner.md#KGModelRunner.develop), [`CoSTEER`](../components/coder/CoSTEER/__init__.md#CoSTEER), [`develop`](../components/coder/CoSTEER/__init__.md#CoSTEER.develop), [`develop`](../scenarios/kaggle/developer/coder.md#KGModelFeatureSelectionCoder.develop), [`develop`](../components/coder/data_science/share/doc.md#DocDev.develop), [`CachedRunner`](../components/runner/__init__.md#CachedRunner), [`develop`](../components/coder/model_coder/one_shot/__init__.md#ModelCodeWriter.develop), [`ASpecificExp`](experiment.md#ASpecificExp), [`develop`](../scenarios/rl/train/runner.md#RLPostTrainingRunner.develop), [`DocDev`](../components/coder/data_science/share/doc.md#DocDev), [`ModelCodeWriter`](../components/coder/model_coder/one_shot/__init__.md#ModelCodeWriter), [`KGModelFeatureSelectionCoder`](../scenarios/kaggle/developer/coder.md#KGModelFeatureSelectionCoder), [`RLPostTrainingRunner`](../scenarios/rl/train/runner.md#RLPostTrainingRunner)
- used by: [`CoSTEER`](../components/coder/CoSTEER/__init__.md#CoSTEER), [`running`](../app/kaggle/loop.md#KaggleRDLoop.running), [`CachedRunner`](../components/runner/__init__.md#CachedRunner), [`coding`](../components/workflow/rd_loop.md#RDLoop.coding), [`running`](../scenarios/data_science/loop.md#DataScienceRDLoop.running), [`coding`](../app/kaggle/loop.md#KaggleRDLoop.coding), [`__init__`](../components/coder/CoSTEER/__init__.md#CoSTEER.__init__), [`develop`](../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderCoSTEER.develop), [`running`](../components/workflow/rd_loop.md#RDLoop.running), [`running`](../app/qlib_rd_loop/quant.md#QuantRDLoop.running), [`running`](../app/qlib_rd_loop/factor.md#FactorRDLoop.running), [`factor_coder`](../app/qlib_rd_loop/quant.md#QuantRDLoop.factor_coder), [`factor_runner`](../app/qlib_rd_loop/quant.md#QuantRDLoop.factor_runner), [`feature_coder`](../app/kaggle/loop.md#KaggleRDLoop.feature_coder), [`feature_runner`](../app/kaggle/loop.md#KaggleRDLoop.feature_runner), [`model_coder`](../app/kaggle/loop.md#KaggleRDLoop.model_coder), [`model_coder`](../app/qlib_rd_loop/quant.md#QuantRDLoop.model_coder), [`model_feature_selection_coder`](../app/kaggle/loop.md#KaggleRDLoop.model_feature_selection_coder), [`model_runner`](../app/kaggle/loop.md#KaggleRDLoop.model_runner), [`model_runner`](../app/qlib_rd_loop/quant.md#QuantRDLoop.model_runner), [`coding`](../app/qlib_rd_loop/quant.md#QuantRDLoop.coding), [`coder`](../components/workflow/rd_loop.md#RDLoop.coder), [`runner`](../components/workflow/rd_loop.md#RDLoop.runner), [`coding`](../app/qlib_rd_loop/factor_from_report.md#FactorReportLoop.coding), [`coding`](../scenarios/finetune/loop.md#LLMFinetuneRDLoop.coding), [`coding`](../scenarios/rl/loop.md#RLPostTrainingRDLoop.coding), [`get_develop_max_seconds`](../components/coder/data_science/share/ds_costeer.md#DSCoSTEER.get_develop_max_seconds), [`get_develop_max_seconds`](../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.get_develop_max_seconds), [`get_develop_max_seconds`](../scenarios/finetune/train/runner.md#LLMFinetuneRunner.get_develop_max_seconds), [`DocDev`](../components/coder/data_science/share/doc.md#DocDev), [`ModelCodeWriter`](../components/coder/model_coder/one_shot/__init__.md#ModelCodeWriter), [`KGModelFeatureSelectionCoder`](../scenarios/kaggle/developer/coder.md#KGModelFeatureSelectionCoder), [`__init__`](../scenarios/rl/train/runner.md#RLPostTrainingRunner.__init__), [`compare_scores`](../scenarios/data_science/dev/runner/__init__.md#DSCoSTEERRunner.compare_scores), [`compare_scores`](../scenarios/finetune/train/runner.md#LLMFinetuneRunner.compare_scores), [`RLPostTrainingRunner`](../scenarios/rl/train/runner.md#RLPostTrainingRunner)  (3 test-only)

