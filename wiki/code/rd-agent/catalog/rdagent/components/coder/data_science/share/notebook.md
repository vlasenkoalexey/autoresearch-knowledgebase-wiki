---
title: 'Module: rdagent/components/coder/data_science/share/notebook.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/data_science/share/notebook.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.data_science.share.notebook`/
symbols:
  NotebookConverter.convert: NotebookConverter#convert().
  args: args.
  NotebookConverter.validate_code_format: NotebookConverter#validate_code_format().
  parser: parser.
  NotebookConverter: NotebookConverter#
  converter: converter.
---
# Module: [`rdagent/components/coder/data_science/share/notebook.py`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/notebook.py)

## Classes
### `NotebookConverter`
- def: [`rdagent/components/coder/data_science/share/notebook.py:22`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/notebook.py#L22)
- doc: Builder responsible for writing a Jupyter notebook for a workspace.
- signature: `class NotebookConverter:`
- members:
  - `convert(self, task: Optional[Task], code: str, stdout: str, outfile: Optional[str] = None, use_debug_flag: bool = False)` — [`L41`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/notebook.py#L41) — Build a notebook based on the current progression.
  - `validate_code_format(self, code: str)` — [`L27`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/notebook.py#L27) — Returns None if the code format is valid, otherwise returns an error message.
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../../log/__init__.md#rdagent_logger.rdagent_logger), [`T`](../../../../utils/agent/tpl.md#T), [`r`](../../../../utils/agent/tpl.md#RDAT.r), [`info`](../../../../log/logger.md#RDAgentLog.info), [`APIBackend`](../../../../oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Task`](../../../../core/experiment.md#Task), [`get_task_information`](../../../../core/experiment.md#Task.get_task_information), [`split_code_and_output_into_sections`](util.md#split_code_and_output_into_sections), [`extract_function_body`](util.md#extract_function_body), [`extract_first_section_name_from_code`](util.md#extract_first_section_name_from_code), [`MarkdownAgentOut`](../../../../utils/agent/ret.md#MarkdownAgentOut), [`extract_output`](../../../../utils/agent/ret.md#MarkdownAgentOut.extract_output)
- used by: [`evaluate`](../pipeline/eval.md#PipelineCoSTEEREvaluator.evaluate), [`args`](notebook.md#args), [`converter`](notebook.md#converter)  (8 test-only)

## Module values
- `args` — [`L128`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/notebook.py#L128)
- `converter` — [`L117`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/notebook.py#L117)
- `parser` — [`L118`](../../../../../../../../../raw/code/rd-agent/rdagent/components/coder/data_science/share/notebook.py#L118)

