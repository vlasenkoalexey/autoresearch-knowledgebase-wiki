---
title: 'Module: rdagent/utils/__init__.py'
type: catalog
provenance: extracted
module: rdagent/utils/__init__.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.utils`/
symbols:
  filter_redundant_text: filter_redundant_text().
  md5_hash: md5_hash().
  try_regex_sub: try_regex_sub().
  convert2bool: convert2bool().
  filter_redundant_text._shrink_stdout_once: filter_redundant_text()._shrink_stdout_once().
  filter_with_time_limit: filter_with_time_limit().
  REGEX_TIMEOUT: REGEX_TIMEOUT.
  get_module_by_module_path: get_module_by_module_path().
  remove_path_info_from_str: remove_path_info_from_str().
---
# Module: [`rdagent/utils/__init__.py`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py)

## Functions
- `_shrink_stdout_once(stdout: str)` — [`L133`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L133)
- `convert2bool(value: Union[str, bool])` — [`L57`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L57) — Motivation: the return value of LLM is not stable. Try to convert the value into bool
- `filter_redundant_text(stdout: str)` — [`L100`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L100) — Filter out progress bars and other redundant patterns from stdout using regex-based trimming. — documented in [rdagent-utils-env](../../../concepts/rdagent-utils-env.md)
- `filter_with_time_limit(regex_patterns: Union[str, list[str]], text: str)` — [`L88`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L88) — Apply one or more regex patterns to filter `text`, using a timeout for each substitution.
- `get_module_by_module_path(module_path: Union[str, ModuleType])` — [`L28`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L28) — Load module from path like a/b/c/d.py or a.b.c.d
- `md5_hash(input_string: str)` — [`L202`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L202) — documented in [rdagent-utils-env](../../../concepts/rdagent-utils-env.md)
- `remove_path_info_from_str(base_path: Path, target_string: str)` — [`L193`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L193) — Remove the absolute path from the target string
- `try_regex_sub(pattern: str, text: str, replace_with: str = "", flags: int = 0)` — [`L75`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L75) — Try to sub a regex pattern against a text string.

## Module values
- `REGEX_TIMEOUT` — [`L25`](../../../../../../raw/code/rd-agent/rdagent/utils/__init__.py#L25)

