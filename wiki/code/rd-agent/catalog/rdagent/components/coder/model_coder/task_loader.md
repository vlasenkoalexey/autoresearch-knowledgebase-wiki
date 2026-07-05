---
title: 'Module: rdagent/components/coder/model_coder/task_loader.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/task_loader.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.task_loader`/
symbols:
  extract_model_from_doc: extract_model_from_doc().
  ModelExperimentLoaderFromPDFfiles.load: ModelExperimentLoaderFromPDFfiles#load().
  ModelExperimentLoaderFromDict.load: ModelExperimentLoaderFromDict#load().
  ModelExperimentLoaderFromPDFfiles: ModelExperimentLoaderFromPDFfiles#
  extract_model_from_docs: extract_model_from_docs().
  ModelExperimentLoaderFromDict: ModelExperimentLoaderFromDict#
  merge_file_to_model_dict_to_model_dict: merge_file_to_model_dict_to_model_dict().
---
# Module: [`rdagent/components/coder/model_coder/task_loader.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/task_loader.py)

## Classes
### `ModelExperimentLoaderFromDict`  ·  implements/extends ModelTaskLoader
- def: [`rdagent/components/coder/model_coder/task_loader.py:99`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/task_loader.py#L99)
- signature: `class ModelExperimentLoaderFromDict(ModelTaskLoader):`
- members:
  - `load(self, model_dict: dict)` — [`L100`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/task_loader.py#L100) — Load data from a dict.
- uses (calls/refs, reference-scoped): [`ModelTask`](model.md#ModelTask), [`QlibModelExperiment`](../../../scenarios/qlib/experiment/model_experiment.md#QlibModelExperiment), [`ModelTaskLoader`](../../loader/task_loader.md#ModelTaskLoader)
- used by: [`load`](../../../core/experiment.md#Loader.load), [`load`](task_loader.md#ModelExperimentLoaderFromPDFfiles.load), [`ModelTaskLoader`](../../loader/task_loader.md#ModelTaskLoader)

### `ModelExperimentLoaderFromPDFfiles`  ·  implements/extends ModelTaskLoader
- def: [`rdagent/components/coder/model_coder/task_loader.py:118`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/task_loader.py#L118)
- signature: `class ModelExperimentLoaderFromPDFfiles(ModelTaskLoader):`
- members:
  - `load(self, file_or_folder_path: str)` — [`L120`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/task_loader.py#L120)
- uses (calls/refs, reference-scoped): [`QlibModelExperiment`](../../../scenarios/qlib/experiment/model_experiment.md#QlibModelExperiment), [`wait_retry`](../../../utils/workflow/misc.md#wait_retry), [`ModelTaskLoader`](../../loader/task_loader.md#ModelTaskLoader), [`load_and_process_pdfs_by_langchain`](../../document_reader/document_reader.md#load_and_process_pdfs_by_langchain), [`load`](task_loader.md#ModelExperimentLoaderFromDict.load), [`ModelExperimentLoaderFromDict`](task_loader.md#ModelExperimentLoaderFromDict), [`extract_model_from_docs`](task_loader.md#extract_model_from_docs), [`merge_file_to_model_dict_to_model_dict`](task_loader.md#merge_file_to_model_dict_to_model_dict)
- used by: [`extract_models_and_implement`](../../../app/general_model/general_model.md#extract_models_and_implement), [`load`](../../../core/experiment.md#Loader.load), [`ModelTaskLoader`](../../loader/task_loader.md#ModelTaskLoader)

## Functions
- `extract_model_from_doc(doc_content: str)` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/task_loader.py#L20) — Extract model information from document content.
- `extract_model_from_docs(docs_dict)` — [`L92`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/task_loader.py#L92)
- `merge_file_to_model_dict_to_model_dict(file_to_model_dict: dict[str, dict])` — [`L71`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/task_loader.py#L71)

