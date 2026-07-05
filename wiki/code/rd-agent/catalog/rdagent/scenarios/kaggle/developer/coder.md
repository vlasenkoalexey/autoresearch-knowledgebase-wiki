---
title: 'Module: rdagent/scenarios/kaggle/developer/coder.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/developer/coder.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.developer.coder`/
symbols:
  KGModelFeatureSelectionCoder.develop: KGModelFeatureSelectionCoder#develop().
  KGFactorCoSTEER: KGFactorCoSTEER.
  KGModelFeatureSelectionCoder: KGModelFeatureSelectionCoder#
  KGModelCoSTEER: KGModelCoSTEER.
  DEFAULT_SELECTION_CODE: DEFAULT_SELECTION_CODE.
---
# Module: [`rdagent/scenarios/kaggle/developer/coder.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/coder.py)

## Classes
### `KGModelFeatureSelectionCoder`  ·  implements/extends Developer
- def: [`rdagent/scenarios/kaggle/developer/coder.py:35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/coder.py#L35)
- signature: `class KGModelFeatureSelectionCoder(Developer[KGModelExperiment]):`
- members:
  - `develop(self, exp: KGModelExperiment)` — [`L36`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/coder.py#L36)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`experiment_workspace`](../../../core/experiment.md#Experiment.experiment_workspace), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`inject_files`](../../../core/experiment.md#FBWorkspace.inject_files), [`sub_tasks`](../../../core/experiment.md#Experiment.sub_tasks), [`Developer`](../../../core/developer.md#Developer), [`KGModelExperiment`](../experiment/kaggle_experiment.md#KGModelExperiment), [`KG_SELECT_MAPPING`](../experiment/kaggle_experiment.md#KG_SELECT_MAPPING), [`model_type`](../../../components/coder/model_coder/model.md#ModelTask.model_type), [`data_description`](../experiment/workspace.md#KGFBWorkspace.data_description), [`DEFAULT_SELECTION_CODE`](coder.md#DEFAULT_SELECTION_CODE)
- used by: [`Developer`](../../../core/developer.md#Developer), [`develop`](../../../core/developer.md#Developer.develop)

## Module values
- `DEFAULT_SELECTION_CODE` — [`L19`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/coder.py#L19)
- `KGFactorCoSTEER` — [`L16`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/coder.py#L16)
- `KGModelCoSTEER` — [`L15`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/developer/coder.py#L15)

