---
title: 'Module: rdagent/log/base.py'
type: catalog
provenance: extracted
module: rdagent/log/base.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.log.base`/
symbols:
  Message.content: Message#content.
  Message.tag: Message#tag.
  Message: Message#
  Storage: Storage#
  Message.timestamp: Message#timestamp.
  Storage.iter_msg: Storage#iter_msg().
  Message.level: Message#level.
  Storage.log: Storage#log().
  Storage.truncate: Storage#truncate().
  Message.caller: Message#caller.
  Message.pid_trace: Message#pid_trace.
  View.display: View#display().
  View: View#
  Storage.__str__: Storage#__str__().
---
# Module: [`rdagent/log/base.py`](../../../../../../raw/code/rd-agent/rdagent/log/base.py)

## Classes
### `Message`
- def: [`rdagent/log/base.py:12`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L12) — documented in [rdagent-log-base](../../../concepts/rdagent-log-base.md)
- doc: The info unit of the storage
- signature: `class Message:`
- members:
  - `caller` — [`L18`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L18)
  - `content` — [`L22`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L22) — documented in [rdagent-log-base](../../../concepts/rdagent-log-base.md)
  - `level` — [`L16`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L16)
  - `pid_trace` — [`L21`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L21)
  - `tag` — [`L15`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L15) — documented in [rdagent-log-base](../../../concepts/rdagent-log-base.md)
  - `timestamp` — [`L17`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L17)
- used by: [`consume_msg`](ui/web.md#SimpleTraceWindow.consume_msg), [`consume_msg`](ui/web.md#StWindow.consume_msg), [`load_ft_session`](../app/finetune/llm/ui/data_loader.md#load_ft_session), [`summarize_folder`](mle_summary.md#summarize_folder), [`iter_msg`](storage.md#FileStorage.iter_msg), [`get_sota_exp_stat`](ui/utils.md#get_sota_exp_stat), [`consume_msg`](ui/web.md#ObjectsTabsWindow.consume_msg), [`consume_msg`](ui/web.md#TraceObjWindow.consume_msg), [`summarize_win`](ui/ds_trace.md#summarize_win), [`consume_msg`](ui/web.md#EvolvingWindow.consume_msg), [`consume_msg`](ui/web.md#TraceWindow.consume_msg), [`consume_msg`](ui/web.md#FeedbackWindow.consume_msg), [`consume_msg`](ui/web.md#ResearchWindow.consume_msg), [`consume_msg`](ui/web.md#WorkspaceWindow.consume_msg), [`consume_msg`](ui/web.md#QlibFactorExpWindow.consume_msg), [`consume_msg`](ui/web.md#QlibModelExpWindow.consume_msg), [`get_msgs_until`](ui/app.md#get_msgs_until), [`save_grade_info`](mle_summary.md#save_grade_info), [`consume_msg`](ui/web.md#ModelFeedbackWindow.consume_msg), [`consume_msg`](ui/web.md#HypothesisFeedbackWindow.consume_msg), [`consume_msg`](ui/web.md#FactorTaskWindow.consume_msg), [`consume_msg`](ui/web.md#ModelTaskWindow.consume_msg), [`read_trace`](server/app.md#read_trace), [`refresh`](ui/app.md#refresh), [`consume_msg`](ui/web.md#FactorFeedbackWindow.consume_msg), [`mock_msg`](ui/web.md#mock_msg), [`read_trace`](server/debug_app.md#upload_file.read_trace), [`load_data`](ui/ds_trace.md#load_data), [`consume_msg`](ui/web.md#SingleRDLoopWindow.consume_msg), [`consume_msg`](ui/web.md#RoundTabsWindow.consume_msg), [`consume_msg`](ui/web.md#ProgressTabsWindow.consume_msg), [`load_times_info`](ui/utils.md#load_times_info), [`consume_msg`](ui/web.md#HypothesisWindow.consume_msg), [`c2`](ui/app.md#c2), [`select_on_existing_trace`](../scenarios/data_science/proposal/exp_gen/select/submit.md#select_on_existing_trace), [`get_score_stat`](ui/utils.md#get_score_stat), [`iter_msg`](ui/storage.md#WebStorage.iter_msg), [`get_best_report`](ui/utils.md#get_best_report), [`consume_msg`](ui/web.md#DevelopmentWindow.consume_msg), [`RDL_win`](ui/web.md#TraceWindow.RDL_win)  (+7 more)

### `Storage`
- def: [`rdagent/log/base.py:25`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L25) — documented in [rdagent-log-base](../../../concepts/rdagent-log-base.md)
- doc: Basic storage to support saving objects;
- signature: `class Storage:`
- members:
  - `iter_msg(self)` — [`L67`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L67) — Iterate the message in the storage. — documented in [rdagent-log-base](../../../concepts/rdagent-log-base.md)
  - `log(self, obj: object, tag: str = "", timestamp: datetime | None = None)` — [`L43`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L43) — Parameters
  - `truncate(self, time: datetime)` — [`L74`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L74) — Remove all log entries after the specified time.
- protocol/private: `__str__`[`L80`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L80)
- uses (calls/refs, reference-scoped): [`Message`](base.md#Message), [`iter_msg`](storage.md#FileStorage.iter_msg), [`FileStorage`](storage.md#FileStorage), [`log`](ui/storage.md#WebStorage.log), [`iter_msg`](ui/storage.md#WebStorage.iter_msg), [`WebStorage`](ui/storage.md#WebStorage), [`log`](storage.md#FileStorage.log), [`truncate`](storage.md#FileStorage.truncate), [`truncate`](ui/storage.md#WebStorage.truncate)
- used by: [`log_object`](logger.md#RDAgentLog.log_object), [`FileStorage`](storage.md#FileStorage), [`display`](ui/web.md#WebView.display), [`other_storages`](logger.md#RDAgentLog.other_storages), [`truncate_storages`](logger.md#RDAgentLog.truncate_storages), [`WebStorage`](ui/storage.md#WebStorage), [`display`](base.md#View.display)

### `View`
- def: [`rdagent/log/base.py:84`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L84)
- doc: Motivation:
- signature: `class View:`
- members:
  - `display(self, s: Storage, watch: bool = False)` — [`L93`](../../../../../../raw/code/rd-agent/rdagent/log/base.py#L93) — Parameters — documented in [rdagent-log-base](../../../concepts/rdagent-log-base.md)
- uses (calls/refs, reference-scoped): [`Storage`](base.md#Storage), [`display`](ui/web.md#WebView.display), [`WebView`](ui/web.md#WebView)
- used by: [`WebView`](ui/web.md#WebView)

