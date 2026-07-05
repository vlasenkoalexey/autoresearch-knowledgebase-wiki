---
title: 'Module: rdagent/components/coder/model_coder/one_shot/__init__.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/model_coder/one_shot/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.model_coder.one_shot`/
symbols:
  ModelCodeWriter.develop: ModelCodeWriter#develop().
  ModelCodeWriter: ModelCodeWriter#
  DIRNAME: DIRNAME.
---
# Module: [`rdagent/components/coder/model_coder/one_shot/__init__.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/one_shot/__init__.py)

## Classes
### `ModelCodeWriter`  ·  implements/extends Developer
- def: [`rdagent/components/coder/model_coder/one_shot/__init__.py:12`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/one_shot/__init__.py#L12)
- signature: `class ModelCodeWriter(Developer[ModelExperiment]):`
- members:
  - `develop(self, exp: ModelExperiment)` — [`L13`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/one_shot/__init__.py#L13)
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`inject_files`](../../../../core/experiment.md#FBWorkspace.inject_files), [`sub_tasks`](../../../../core/experiment.md#Experiment.sub_tasks), [`Developer`](../../../../core/developer.md#Developer), [`ModelFBWorkspace`](../model.md#ModelFBWorkspace), [`sub_workspace_list`](../../../../core/experiment.md#Experiment.sub_workspace_list), [`ModelExperiment`](../model.md#ModelExperiment), [`prepare`](../../../../core/experiment.md#FBWorkspace.prepare)
- used by: [`Developer`](../../../../core/developer.md#Developer), [`develop`](../../../../core/developer.md#Developer.develop)  (1 test-only)

## Module values
- `DIRNAME` — [`L9`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/model_coder/one_shot/__init__.py#L9)

