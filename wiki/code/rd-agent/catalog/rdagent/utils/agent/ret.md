---
title: 'Module: rdagent/utils/agent/ret.py'
type: catalog
provenance: extracted
module: rdagent/utils/agent/ret.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.utils.agent.ret`/
symbols:
  PythonAgentOut: PythonAgentOut#
  AgentOut: AgentOut#
  AgentOut.get_spec: AgentOut#get_spec().
  AgentOut.extract_output: AgentOut#extract_output().
  PythonAgentOut.get_spec: PythonAgentOut#get_spec().
  PythonBatchEditOut: PythonBatchEditOut#
  PythonAgentOut.extract_output: PythonAgentOut#extract_output().
  PythonBatchEditOut.get_spec: PythonBatchEditOut#get_spec().
  MarkdownAgentOut: MarkdownAgentOut#
  PythonBatchPatchOut.get_spec: PythonBatchPatchOut#get_spec().
  PythonBatchPatchOut: PythonBatchPatchOut#
  MarkdownAgentOut.get_spec: MarkdownAgentOut#get_spec().
  BatchEditOut.get_spec: BatchEditOut#get_spec().
  PythonBatchPatchOut.extract_output: PythonBatchPatchOut#extract_output().
  BatchEditOut: BatchEditOut#
  MarkdownAgentOut.extract_output: MarkdownAgentOut#extract_output().
  PythonBatchEditOut.extract_output: PythonBatchEditOut#extract_output().
  AgentOut.json_mode: AgentOut#json_mode.
  BatchEditOut.json_mode: BatchEditOut#json_mode.
  BatchEditOut.extract_output: BatchEditOut#extract_output().
---
# Module: [`rdagent/utils/agent/ret.py`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py)

## Classes
### `AgentOut`
- def: [`rdagent/utils/agent/ret.py:17`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L17)
- signature: `class AgentOut:`
- members:
  - `extract_output(cls, resp: str)` — [`L25`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L25)
  - `get_spec(cls, **context: Any)` — [`L21`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L21)
  - `json_mode` — [`L18`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L18)
- uses (calls/refs, reference-scoped): [`PythonAgentOut`](ret.md#PythonAgentOut), [`get_spec`](ret.md#PythonAgentOut.get_spec), [`PythonBatchEditOut`](ret.md#PythonBatchEditOut), [`extract_output`](ret.md#PythonAgentOut.extract_output), [`get_spec`](ret.md#PythonBatchEditOut.get_spec), [`MarkdownAgentOut`](ret.md#MarkdownAgentOut), [`get_spec`](ret.md#PythonBatchPatchOut.get_spec), [`PythonBatchPatchOut`](ret.md#PythonBatchPatchOut), [`get_spec`](ret.md#BatchEditOut.get_spec), [`get_spec`](ret.md#MarkdownAgentOut.get_spec), [`extract_output`](ret.md#PythonBatchPatchOut.extract_output), [`BatchEditOut`](ret.md#BatchEditOut), [`extract_output`](ret.md#MarkdownAgentOut.extract_output), [`extract_output`](ret.md#PythonBatchEditOut.extract_output), [`extract_output`](ret.md#BatchEditOut.extract_output)
- used by: [`PythonAgentOut`](ret.md#PythonAgentOut), [`PythonBatchEditOut`](ret.md#PythonBatchEditOut), [`MarkdownAgentOut`](ret.md#MarkdownAgentOut), [`PythonBatchPatchOut`](ret.md#PythonBatchPatchOut), [`BatchEditOut`](ret.md#BatchEditOut)

### `BatchEditOut`  ·  implements/extends AgentOut
- def: [`rdagent/utils/agent/ret.py:59`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L59)
- signature: `class BatchEditOut(AgentOut):`
- members:
  - `extract_output(cls, resp: str)` — [`L67`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L67)
  - `get_spec(cls, with_del=True)` — [`L63`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L63)
  - `json_mode` — [`L60`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L60)
- uses (calls/refs, reference-scoped): [`T`](tpl.md#T), [`r`](tpl.md#RDAT.r), [`AgentOut`](ret.md#AgentOut)
- used by: [`AgentOut`](ret.md#AgentOut), [`extract_output`](ret.md#AgentOut.extract_output), [`get_spec`](ret.md#AgentOut.get_spec)

### `MarkdownAgentOut`  ·  implements/extends AgentOut
- def: [`rdagent/utils/agent/ret.py:45`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L45)
- signature: `class MarkdownAgentOut(AgentOut):`
- members:
  - `extract_output(cls, resp: str)` — [`L51`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L51)
  - `get_spec(cls)` — [`L47`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L47)
- uses (calls/refs, reference-scoped): [`T`](tpl.md#T), [`r`](tpl.md#RDAT.r), [`AgentOut`](ret.md#AgentOut)
- used by: [`convert`](../../components/coder/data_science/share/notebook.md#NotebookConverter.convert), [`develop`](../../components/coder/data_science/share/doc.md#DocDev.develop), [`AgentOut`](ret.md#AgentOut), [`extract_output`](ret.md#AgentOut.extract_output), [`get_spec`](ret.md#AgentOut.get_spec)

### `PythonAgentOut`  ·  implements/extends AgentOut
- def: [`rdagent/utils/agent/ret.py:29`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L29)
- signature: `class PythonAgentOut(AgentOut):`
- members:
  - `extract_output(cls, resp: str)` — [`L35`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L35)
  - `get_spec(cls)` — [`L31`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L31)
- uses (calls/refs, reference-scoped): [`T`](tpl.md#T), [`r`](tpl.md#RDAT.r), [`AgentOut`](ret.md#AgentOut)
- used by: [`_generate_and_run_script`](../../scenarios/data_science/proposal/exp_gen/select/submit.md#ValidationSelector._generate_and_run_script), [`implement_one_task`](../../components/coder/data_science/pipeline/__init__.md#PipelineMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/raw_data_loader/__init__.md#DataLoaderMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/ensemble/__init__.md#EnsembleMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/feature/__init__.md#FeatureMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/workflow/__init__.md#WorkflowMultiProcessEvolvingStrategy.implement_one_task), [`AgentOut`](ret.md#AgentOut), [`extract_output`](ret.md#AgentOut.extract_output), [`get_spec`](ret.md#AgentOut.get_spec)  (1 test-only)

### `PythonBatchEditOut`  ·  implements/extends AgentOut
- def: [`rdagent/utils/agent/ret.py:71`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L71)
- signature: `class PythonBatchEditOut(AgentOut):`
- members:
  - `extract_output(cls, resp: str)` — [`L77`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L77)
  - `get_spec(cls, with_del=True)` — [`L73`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L73)
- uses (calls/refs, reference-scoped): [`T`](tpl.md#T), [`r`](tpl.md#RDAT.r), [`AgentOut`](ret.md#AgentOut)
- used by: [`implement_one_task`](../../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`implement_one_task`](../../components/coder/data_science/model/__init__.md#ModelMultiProcessEvolvingStrategy.implement_one_task), [`AgentOut`](ret.md#AgentOut), [`extract_output`](ret.md#AgentOut.extract_output), [`get_spec`](ret.md#AgentOut.get_spec)

### `PythonBatchPatchOut`  ·  implements/extends AgentOut
- def: [`rdagent/utils/agent/ret.py:89`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L89)
- signature: `class PythonBatchPatchOut(AgentOut):`
- members:
  - `extract_output(cls, resp: str, prefix: Path | None = None)` — [`L95`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L95)
  - `get_spec(cls)` — [`L91`](../../../../../../../raw/code/rd-agent/rdagent/utils/agent/ret.py#L91)
- uses (calls/refs, reference-scoped): [`T`](tpl.md#T), [`r`](tpl.md#RDAT.r), [`AgentOut`](ret.md#AgentOut), [`apply_patch_from_text`](apply_patch.md#apply_patch_from_text)
- used by: [`implement_one_task`](../../scenarios/data_science/dev/runner/__init__.md#DSRunnerMultiProcessEvolvingStrategy.implement_one_task), [`AgentOut`](ret.md#AgentOut), [`extract_output`](ret.md#AgentOut.extract_output), [`get_spec`](ret.md#AgentOut.get_spec)

