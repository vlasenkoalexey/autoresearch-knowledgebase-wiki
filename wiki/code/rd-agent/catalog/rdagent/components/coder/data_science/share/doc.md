---
title: 'Module: rdagent/components/coder/data_science/share/doc.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/share/doc.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.share.doc`/DocDev#
symbols:
  DocDev.develop: develop().
  DocDev: ''
---
# Module: [`rdagent/components/coder/data_science/share/doc.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/doc.py)

## Classes
### `DocDev`  ·  implements/extends Developer
- def: [`rdagent/components/coder/data_science/share/doc.py:12`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/doc.py#L12)
- doc: The developer is responsible for writing documents for a workspace.
- signature: `class DocDev(Developer[Experiment]):`
- members:
  - `develop(self, exp: Experiment)` — [`L17`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/doc.py#L17) — Write documents for the workspace.
- uses (calls/refs, reference-scoped): [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`FBWorkspace`](../../../../core/experiment.md#FBWorkspace), [`experiment_workspace`](../../../../core/experiment.md#Experiment.experiment_workspace), [`Experiment`](../../../../core/experiment.md#Experiment), [`workspace_path`](../../../../core/experiment.md#FBWorkspace.workspace_path), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`inject_files`](../../../../core/experiment.md#FBWorkspace.inject_files), [`Developer`](../../../../core/developer.md#Developer), [`MarkdownAgentOut`](../../../../utils/agent/ret.md#MarkdownAgentOut), [`extract_output`](../../../../utils/agent/ret.md#MarkdownAgentOut.extract_output)
- used by: [`Developer`](../../../../core/developer.md#Developer), [`develop`](../../../../core/developer.md#Developer.develop), [`running`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.running), [`docdev`](../../../../scenarios/data_science/loop.md#DataScienceRDLoop.docdev)

