---
title: 'Module: rdagent/log/storage.py'
type: catalog
provenance: extracted
module: rdagent/log/storage.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.storage`/
symbols:
  FileStorage.iter_msg: FileStorage#iter_msg().
  FileStorage: FileStorage#
  FileStorage.path: FileStorage#path.
  FileStorage.log: FileStorage#log().
  FileStorage.truncate: FileStorage#truncate().
  _remove_empty_dir: _remove_empty_dir().
  FileStorage.__str__: FileStorage#__str__().
  LOG_LEVEL: LOG_LEVEL.
  FileStorage.__init__: FileStorage#__init__().
  FileStorage.log_pattern: FileStorage#log_pattern.
---
# Module: [`rdagent/log/storage.py`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py)

## Classes
### `FileStorage`  ·  implements/extends Storage
- def: [`rdagent/log/storage.py:28`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L28) — documented in [rdagent-app-CI-run](../../../concepts/rdagent-app-CI-run.md)
- doc: The info are logginged to the file systems
- signature: `class FileStorage(Storage):`
- members:
  - `iter_msg(self, tag: str | None = None, pattern: str | None = None)` — [`L79`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L79) — documented in [rdagent-log-base](../../../concepts/rdagent-log-base.md)
  - `log(self, obj: object, tag: str = "", timestamp: datetime | None = None, save_type: Literal["json", "text", "pkl"] = "pkl", **kwargs: Any)` — [`L38`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L38)
  - `truncate(self, time: datetime)` — [`L107`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L107)
  - `log_pattern` — [`L73`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L73)
  - `path` — [`L36`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L36)
- protocol/private: `__init__`[`L35`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L35), `__str__`[`L115`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L115)
- uses (calls/refs, reference-scoped): [`content`](base.md#Message.content), [`tag`](base.md#Message.tag), [`Message`](base.md#Message), [`Storage`](base.md#Storage), [`timestamp`](base.md#Message.timestamp), [`level`](base.md#Message.level), [`caller`](base.md#Message.caller), [`pid_trace`](base.md#Message.pid_trace), [`_remove_empty_dir`](storage.md#_remove_empty_dir), [`gen_datetime`](utils/__init__.md#gen_datetime)
- used by: [`load_ft_session`](../app/finetune/llm/ui/data_loader.md#load_ft_session), [`summarize_folder`](mle_summary.md#summarize_folder), [`get_sota_exp_stat`](ui/utils.md#get_sota_exp_stat), [`summarize_win`](ui/ds_trace.md#summarize_win), [`save_grade_info`](mle_summary.md#save_grade_info), [`read_trace`](server/app.md#read_trace), [`refresh`](ui/app.md#refresh), [`read_trace`](server/debug_app.md#upload_file.read_trace), [`load_data`](ui/ds_trace.md#load_data), [`load_times_info`](ui/utils.md#load_times_info), [`select_on_existing_trace`](../scenarios/data_science/proposal/exp_gen/select/submit.md#select_on_existing_trace), [`get_score_stat`](ui/utils.md#get_score_stat), [`Storage`](base.md#Storage), [`get_best_report`](ui/utils.md#get_best_report), [`set_storages_path`](logger.md#RDAgentLog.set_storages_path), [`storage`](logger.md#RDAgentLog.storage), [`iter_msg`](base.md#Storage.iter_msg), [`log`](base.md#Storage.log), [`truncate`](base.md#Storage.truncate)

## Functions
- `_remove_empty_dir(path: Path)` — [`L14`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L14) — Recursively remove empty directories.

## Module values
- `LOG_LEVEL` — [`L11`](../../../../../../raw/code/rd-agent/rdagent/log/storage.py#L11)

