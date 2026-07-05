---
title: 'Module: ai_scientist/treesearch/log_summarization.py'
type: catalog
provenance: extracted
module: ai_scientist/treesearch/log_summarization.py
status: fresh
symbol_base: scip-python python ai-scientist-v2 0.0.0 `ai_scientist.treesearch.log_summarization`/
symbols:
  ablation_file: ablation_file.
  update_summary: update_summary().
  annotate_history: annotate_history().
  reconstruct_journal: reconstruct_journal().
  journal: journal.
  parent_dir: parent_dir.
  overall_summarize.process_stage: overall_summarize().process_stage().
  folder: folder.
  get_summarizer_prompt: get_summarizer_prompt().
  get_stage_summary: get_stage_summary().
  draft_file: draft_file.
  baseline_file: baseline_file.
  research_file: research_file.
  journal_path: journal_path.
  ablation_summary_path: ablation_summary_path.
  get_node_log: get_node_log().
  stage_folders: stage_folders.
  journal_data: journal_data.
  ablation_summary: ablation_summary.
  overall_summarize: overall_summarize().
  draft_summary_path: draft_summary_path.
  baseline_summary_path: baseline_summary_path.
  research_summary_path: research_summary_path.
  log_dir: log_dir.
  report_summarizer_prompt: report_summarizer_prompt.
  stage_name: stage_name.
  index: index.
  report_summarizer_sys_msg: report_summarizer_sys_msg.
  get_nodes_infos: get_nodes_infos().
  journals: journals.
  output_format_control: output_format_control.
  stage_aggregate_prompt: stage_aggregate_prompt.
  overall_plan_summarizer_prompt: overall_plan_summarizer_prompt.
  example_path: example_path.
  load_stage_folders: load_stage_folders().
  file: file.
  draft_summary: draft_summary.
  baseline_summary: baseline_summary.
  research_summary: research_summary.
---
# Module: [`ai_scientist/treesearch/log_summarization.py`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py)

## Functions
- `annotate_history(journal, cfg=None)` — [`L262`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L262) — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)
- `get_node_log(node)` — [`L156`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L156) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `get_nodes_infos(nodes)` — [`L109`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L109) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `get_stage_summary(journal, stage_name, model, client)` — [`L149`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L149) — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)
- `get_summarizer_prompt(journal, stage_name)` — [`L138`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L138)
- `load_stage_folders(base_path)` — [`L368`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L368) — Load the folders that start with 'stage_' followed by a number. — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `overall_summarize(journals, cfg=None)` — [`L299`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L299) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `process_stage(idx, stage_tuple)` — [`L302`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L302) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `reconstruct_journal(journal_data)` — [`L384`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L384) — documented in [ai_scientist-treesearch-journal](../../../concepts/ai_scientist-treesearch-journal.md)
- `update_summary(prev_summary, cur_stage_name, cur_journal, cur_summary, model, client, max_retry=5)` — [`L198`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L198) — documented in [ai_scientist-llm](../../../concepts/ai_scientist-llm.md)

## Module values
- `ablation_file` — [`L445`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L445) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `ablation_summary` — [`L428`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L428) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `ablation_summary_path` — [`L434`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L434) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `baseline_file` — [`L439`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L439)
- `baseline_summary` — [`L426`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L426)
- `baseline_summary_path` — [`L432`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L432) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `draft_file` — [`L436`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L436)
- `draft_summary` — [`L425`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L425)
- `draft_summary_path` — [`L431`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L431) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `example_path` — [`L366`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L366) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `file` — [`L415`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L415) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `folder` — [`L410`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L410) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `index` — [`L410`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L410) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `journal` — [`L420`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L420)
- `journal_data` — [`L416`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L416) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `journal_path` — [`L413`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L413)
- `journals` — [`L409`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L409) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `log_dir` — [`L430`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L430) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `output_format_control` — [`L23`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L23)
- `overall_plan_summarizer_prompt` — [`L232`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L232)
- `parent_dir` — [`L7`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L7)
- `report_summarizer_prompt` — [`L50`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L50)
- `report_summarizer_sys_msg` — [`L13`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L13)
- `research_file` — [`L442`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L442)
- `research_summary` — [`L427`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L427)
- `research_summary_path` — [`L433`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L433) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `stage_aggregate_prompt` — [`L66`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L66) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `stage_folders` — [`L408`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L408) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)
- `stage_name` — [`L412`](../../../../../../raw/code/ai-scientist-v2/ai_scientist/treesearch/log_summarization.py#L412) — documented in [ai_scientist-treesearch-log_summarization](../../../concepts/ai_scientist-treesearch-log_summarization.md)

