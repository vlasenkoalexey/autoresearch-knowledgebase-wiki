---
title: 'Module: rdagent/utils/repo/repo_utils.py'
type: catalog
provenance: extracted
module: rdagent/utils/repo/repo_utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.utils.repo.repo_utils`/
symbols:
  RepoAnalyzer.repo_path: RepoAnalyzer#repo_path.
  RepoAnalyzer.summarize_repo: RepoAnalyzer#summarize_repo().
  RepoAnalyzer._summarize_file: RepoAnalyzer#_summarize_file().
  summary: summary.
  content: content.
  highlighted_files: highlighted_files.
  analyzer: analyzer.
  RepoAnalyzer._generate_tree_structure: RepoAnalyzer#_generate_tree_structure().
  RepoAnalyzer._summarize_class: RepoAnalyzer#_summarize_class().
  RepoAnalyzer.highlight: RepoAnalyzer#highlight().
  RepoAnalyzer._summarize_function: RepoAnalyzer#_summarize_function().
  file_name: file_name.
  RepoAnalyzer: RepoAnalyzer#
  RepoAnalyzer.__init__: RepoAnalyzer#__init__().
  RepoAnalyzer.summaries: RepoAnalyzer#summaries.
---
# Module: [`rdagent/utils/repo/repo_utils.py`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py)

## Classes
### `RepoAnalyzer`
- def: [`rdagent/utils/repo/repo_utils.py:8`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L8)
- signature: `class RepoAnalyzer:`
- members:
  - `_generate_tree_structure(self)` — [`L47`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L47) — Generate a tree-like structure of the repository.
  - `highlight(self, file_names: Union[str, List[str]])` — [`L130`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L130) — Extract content from specified file(s) within the repo.
  - `summarize_repo(self, verbose_level: int = 1, doc_str_level: int = 1, sign_level: int = 1)` — [`L13`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L13) — Generate a natural language summary of the entire repository workspace.
  - `repo_path` — [`L10`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L10)
  - `summaries` — [`L11`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L11)
- protocol/private: `__init__`[`L9`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L9), `_summarize_class`[`L89`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L89), `_summarize_file`[`L65`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L65), `_summarize_function`[`L103`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L103)
- used by: [`summary`](repo_utils.md#summary), [`highlighted_files`](repo_utils.md#highlighted_files), [`analyzer`](repo_utils.md#analyzer)

## Module values
- `analyzer` — [`L153`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L153)
- `content` — [`L160`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L160)
- `file_name` — [`L160`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L160)
- `highlighted_files` — [`L156`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L156)
- `summary` — [`L154`](../../../../../../../raw/code/rd-agent/rdagent/utils/repo/repo_utils.py#L154)

