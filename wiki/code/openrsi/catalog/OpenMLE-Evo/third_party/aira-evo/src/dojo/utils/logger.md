---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.utils.logger`/
symbols:
  LogEvent: LogEvent#
  LogEvent.SOLVER: LogEvent#SOLVER.
  CollectiveLogger.info: CollectiveLogger#info().
  EVENT_COLOURS: EVENT_COLOURS.
  BaseLogger: BaseLogger#
  _make_multi_logger: _make_multi_logger().
  BaseLogger.log_stat: BaseLogger#log_stat().
  BaseLogger.log_dict: BaseLogger#log_dict().
  CollectiveLogger.warning: CollectiveLogger#warning().
  JsonLogger.log_stat: JsonLogger#log_stat().
  get_logger: get_logger().
  CollectiveLogger.process_event_message: CollectiveLogger#process_event_message().
  LogEvent.INTERPRETER: LogEvent#INTERPRETER.
  BaseLogger.log_file: BaseLogger#log_file().
  CollectiveLogger.log: CollectiveLogger#log().
  CollectiveLogger.logger: CollectiveLogger#logger.
  ConsoleLogger.log_stat: ConsoleLogger#log_stat().
  ConsoleLogger.log_dict: ConsoleLogger#log_dict().
  CollectiveLogger.log_file: CollectiveLogger#log_file().
  BaseLogger.stop: BaseLogger#stop().
  JsonLogger.flush_logs: JsonLogger#flush_logs().
  CollectiveLogger: CollectiveLogger#
  CollectiveLogger.low_resource_use: CollectiveLogger#low_resource_use.
  CollectiveLogger.debug: CollectiveLogger#debug().
  MultiLogger.log_stat: MultiLogger#log_stat().
  MultiLogger.log_dict: MultiLogger#log_dict().
  CollectiveLogger.error: CollectiveLogger#error().
  init_logger: init_logger().
  CollectiveLogger.stop: CollectiveLogger#stop().
  CollectiveLogger.critical: CollectiveLogger#critical().
  MultiLogger.log_file: MultiLogger#log_file().
  MultiLogger.stop: MultiLogger#stop().
  ConsoleLogger.__init__: ConsoleLogger#__init__().
  ConsoleLogger.logger: ConsoleLogger#logger.
  JsonLogger.log_dict: JsonLogger#log_dict().
  CollectiveLogger.cfg: CollectiveLogger#cfg().
  JsonLogger.json_logs_path: JsonLogger#json_logs_path.
  config_logger: config_logger().
  LogEvent.MISC: LogEvent#MISC.
  CollectiveLogger._cfg: CollectiveLogger#_cfg.
  MultiLogger.loggers: MultiLogger#loggers.
  MultiLogger: MultiLogger#
  WandBLogger: WandBLogger#
  ConsoleLogger: ConsoleLogger#
  JsonLogger: JsonLogger#
  JsonLogger.buffer: JsonLogger#buffer.
  BaseLogger.__init__: BaseLogger#__init__().
  MultiLogger.__init__: MultiLogger#__init__().
  WandBLogger.__init__: WandBLogger#__init__().
  WandBLogger.log_stat: WandBLogger#log_stat().
  JsonLogger.__init__: JsonLogger#__init__().
  JsonLogger.stop: JsonLogger#stop().
  LogEvent.EVAL: LogEvent#EVAL.
  JsonLogger.last_flush_time: JsonLogger#last_flush_time.
  LOGGERS: LOGGERS.
  LogEvent.AGENT: LogEvent#AGENT.
  LogEvent.TASK: LogEvent#TASK.
  LogEvent.LLM_CLIENT: LogEvent#LLM_CLIENT.
  JsonLogger.flush_interval: JsonLogger#flush_interval.
  CollectiveLogger.__init__: CollectiveLogger#__init__().
  CollectiveLogger.config: CollectiveLogger#config().
  WandBLogger.detailed_logging: WandBLogger#detailed_logging.
  WandBLogger.unique_token: WandBLogger#unique_token.
  WandBLogger.log_file: WandBLogger#log_file().
  WandBLogger.stop: WandBLogger#stop().
  ConsoleLogger.log_file: ConsoleLogger#log_file().
  JsonLogger.log_file: JsonLogger#log_file().
  describe: describe().
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py)

## Classes
### `BaseLogger`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py:121`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L121)
- members:
  - `log_dict(self, data: Dict, event: Union[LogEvent, str], step: Optional[int] = None)` — [`L131`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L131) — Log a dictionary of metrics.
  - `log_file(self, file_path: str)` — [`L146`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L146)
  - `log_stat(self, key: str, value: float, event: LogEvent, step: Optional[int] = None)` — [`L127`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L127) — Log a single metric.
  - `stop(self)` — [`L149`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L149) — Stop the logger.
- protocol/private: `__init__`[`L123`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L123)
- uses (calls/refs, reference-scoped): [`LogEvent`](logger.md#LogEvent), [`LoggerConfig`](../config_dataclasses/logger.md#LoggerConfig), [`log_stat`](logger.md#JsonLogger.log_stat), [`log_dict`](logger.md#ConsoleLogger.log_dict), [`log_stat`](logger.md#ConsoleLogger.log_stat), [`log_dict`](logger.md#MultiLogger.log_dict), [`log_stat`](logger.md#MultiLogger.log_stat), [`log_dict`](logger.md#JsonLogger.log_dict), [`log_file`](logger.md#MultiLogger.log_file), [`stop`](logger.md#MultiLogger.stop), [`ConsoleLogger`](logger.md#ConsoleLogger), [`JsonLogger`](logger.md#JsonLogger), [`MultiLogger`](logger.md#MultiLogger), [`WandBLogger`](logger.md#WandBLogger), [`log_stat`](logger.md#WandBLogger.log_stat), [`stop`](logger.md#JsonLogger.stop), [`log_file`](logger.md#ConsoleLogger.log_file), [`log_file`](logger.md#JsonLogger.log_file), [`log_file`](logger.md#WandBLogger.log_file), [`stop`](logger.md#WandBLogger.stop)
- used by: [`_make_multi_logger`](logger.md#_make_multi_logger), [`log`](logger.md#CollectiveLogger.log), [`logger`](logger.md#CollectiveLogger.logger), [`log_file`](logger.md#CollectiveLogger.log_file), [`log_dict`](logger.md#MultiLogger.log_dict), [`log_stat`](logger.md#MultiLogger.log_stat), [`log_file`](logger.md#MultiLogger.log_file), [`stop`](logger.md#CollectiveLogger.stop), [`stop`](logger.md#MultiLogger.stop), [`ConsoleLogger`](logger.md#ConsoleLogger), [`JsonLogger`](logger.md#JsonLogger), [`MultiLogger`](logger.md#MultiLogger), [`WandBLogger`](logger.md#WandBLogger), [`__init__`](logger.md#MultiLogger.__init__)

### `CollectiveLogger`
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py:59`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L59)
- doc: The main logger.
- signature: `class CollectiveLogger:`
- members:
  - `cfg(self)` — [`L66`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L66)
  - `config(self, config: DictConfig)` — [`L71`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L71)
  - `critical(self, msg: object, event: Optional[LogEvent] = None)` — [`L117`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L117)
  - `debug(self, msg: object, event: Optional[LogEvent] = None)` — [`L114`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L114)
  - `error(self, msg: object, event: Optional[LogEvent] = None)` — [`L111`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L111)
  - `info(self, msg: object, event: Optional[LogEvent] = None)` — [`L105`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L105)
  - `log(self, metrics: Dict, event: Union[LogEvent, str], step: Optional[int] = None)` — [`L81`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L81) — Log a dictionary metrics at a given timestep.
  - `log_file(self, file_path: str)` — [`L92`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L92)
  - `process_event_message(self, msg: object, event: Optional[LogEvent] = None)` — [`L100`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L100)
  - `stop(self)` — [`L96`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L96) — Stop the logger.
  - `warning(self, msg: object, event: Optional[LogEvent] = None)` — [`L108`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L108)
  - `logger` — [`L73`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L73)
  - `low_resource_use` — [`L75`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L75)
- protocol/private: `__init__`[`L62`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L62), `_cfg`[`L63`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L63)
- uses (calls/refs, reference-scoped): [`LogEvent`](logger.md#LogEvent), [`EVENT_COLOURS`](logger.md#EVENT_COLOURS), [`BaseLogger`](logger.md#BaseLogger), [`_make_multi_logger`](logger.md#_make_multi_logger), [`log_dict`](logger.md#BaseLogger.log_dict), [`log_file`](logger.md#BaseLogger.log_file), [`stop`](logger.md#BaseLogger.stop), [`MISC`](logger.md#LogEvent.MISC)
- used by: [`sample_in_context`](../solvers/evo/evo.md#SolutionsDatabase.sample_in_context), [`add_nodes_to_islands`](../solvers/evo/evo.md#SolutionsDatabase.add_nodes_to_islands), [`export_search_results`](../core/solvers/utils/search_exporter.md#export_search_results), [`register_node_in_island`](../solvers/evo/evo.md#Island.register_node_in_island), [`reset_islands`](../solvers/evo/evo.md#SolutionsDatabase.reset_islands), [`only_keep_best`](../solvers/evo/evo.md#Island.only_keep_best), [`remove_lowest`](../solvers/evo/evo.md#Island.remove_lowest), [`remove_node`](../solvers/evo/evo.md#Island.remove_node), [`seed_islands_with_nodes`](../solvers/evo/evo.md#SolutionsDatabase.seed_islands_with_nodes), [`migrate_node`](../solvers/evo/evo.md#Island.migrate_node), [`main`](../core/interpreters/python.md#main), [`_update_global_fitness_range`](../solvers/evo/evo.md#SolutionsDatabase._update_global_fitness_range), [`init_logger`](logger.md#init_logger), [`__init__`](../solvers/evo/evo.md#Island.__init__), [`__init__`](../solvers/evo/evo.md#SolutionsDatabase.__init__)

### `ConsoleLogger`  ·  implements/extends BaseLogger
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py:205`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L205)
- doc: Logger for writing to stdout.
- signature: `class ConsoleLogger(BaseLogger):`
- members:
  - `log_dict(self, data: Dict, event: LogEvent, step: Optional[int] = None)` — [`L234`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L234)
  - `log_file(self, file_path: str)` — [`L264`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L264)
  - `log_stat(self, key: str, value: float, event: LogEvent, step: Optional[int] = None)` — [`L221`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L221)
  - `logger` — [`L209`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L209)
- protocol/private: `__init__`[`L208`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L208)
- uses (calls/refs, reference-scoped): [`LogEvent`](logger.md#LogEvent), [`EVENT_COLOURS`](logger.md#EVENT_COLOURS), [`BaseLogger`](logger.md#BaseLogger), [`LoggerConfig`](../config_dataclasses/logger.md#LoggerConfig), [`MISC`](logger.md#LogEvent.MISC)
- used by: [`BaseLogger`](logger.md#BaseLogger), [`_make_multi_logger`](logger.md#_make_multi_logger), [`log_dict`](logger.md#BaseLogger.log_dict), [`log_stat`](logger.md#BaseLogger.log_stat), [`log_file`](logger.md#BaseLogger.log_file)

### `JsonLogger`  ·  implements/extends BaseLogger
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py:268`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L268)
- signature: `class JsonLogger(BaseLogger):`
- members:
  - `flush_logs(self)` — [`L304`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L304) — Writes all buffered logs to disk using jsonlines.
  - `log_dict(self, data: Dict, event: Union[LogEvent, str], step: Optional[int] = None)` — [`L277`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L277) — Log a dictionary of metrics under the same step.
  - `log_file(self, file_path: str)` — [`L321`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L321)
  - `log_stat(self, data: Dict[str, float], event: Union[LogEvent, str], step: Optional[int] = None)` — [`L282`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L282) — Logs all key-value pairs under the same step in a buffer.
  - `stop(self)` — [`L324`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L324) — Ensure all logs are written before stopping.
  - `buffer` — [`L273`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L273)
  - `flush_interval` — [`L275`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L275)
  - `json_logs_path` — [`L270`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L270)
  - `last_flush_time` — [`L274`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L274)
- protocol/private: `__init__`[`L269`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L269)
- uses (calls/refs, reference-scoped): [`LogEvent`](logger.md#LogEvent), [`BaseLogger`](logger.md#BaseLogger), [`LoggerConfig`](../config_dataclasses/logger.md#LoggerConfig)
- used by: [`BaseLogger`](logger.md#BaseLogger), [`_make_multi_logger`](logger.md#_make_multi_logger), [`log_dict`](logger.md#BaseLogger.log_dict), [`log_stat`](logger.md#BaseLogger.log_stat), [`log_file`](logger.md#BaseLogger.log_file), [`stop`](logger.md#BaseLogger.stop)

### `LogEvent`  ·  implements/extends Enum
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py:38`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L38)
- signature: `class LogEvent(Enum):`
- members:
  - `AGENT` — [`L39`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L39)
  - `EVAL` — [`L44`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L44)
  - `INTERPRETER` — [`L42`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L42)
  - `LLM_CLIENT` — [`L45`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L45)
  - `MISC` — [`L43`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L43)
  - `SOLVER` — [`L40`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L40)
  - `TASK` — [`L41`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L41)
- used by: [`search`](../solvers/evo/evo.md#Evolutionary.search), [`_main`](../main_run.md#_main), [`_debug_cycle_async`](../solvers/evo/evo.md#Evolutionary._debug_cycle_async), [`sample_in_context`](../solvers/evo/evo.md#SolutionsDatabase.sample_in_context), [`_async_worker_loop`](../solvers/evo/evo.md#Evolutionary._async_worker_loop), [`root_node`](../solvers/evo/evo.md#Evolutionary.root_node), [`add_nodes_to_islands`](../solvers/evo/evo.md#SolutionsDatabase.add_nodes_to_islands), [`debug_cycle`](../solvers/evo/evo.md#Evolutionary.debug_cycle), [`run`](../core/interpreters/python.md#PythonInterpreter.run), [`export_search_results`](../core/solvers/utils/search_exporter.md#export_search_results), [`__call__`](../solvers/evo/evo.md#Evolutionary.__call__), [`register_node_in_island`](../solvers/evo/evo.md#Island.register_node_in_island), [`info`](logger.md#CollectiveLogger.info), [`reset_islands`](../solvers/evo/evo.md#SolutionsDatabase.reset_islands), [`EVENT_COLOURS`](logger.md#EVENT_COLOURS), [`only_keep_best`](../solvers/evo/evo.md#Island.only_keep_best), [`remove_lowest`](../solvers/evo/evo.md#Island.remove_lowest), [`remove_node`](../solvers/evo/evo.md#Island.remove_node), [`migrate_node`](../solvers/evo/evo.md#Island.migrate_node), [`_update_global_fitness_range`](../solvers/evo/evo.md#SolutionsDatabase._update_global_fitness_range), [`cleanup_session`](../core/interpreters/python.md#PythonInterpreter.cleanup_session), [`log_dict`](logger.md#BaseLogger.log_dict), [`log_stat`](logger.md#BaseLogger.log_stat), [`warning`](logger.md#CollectiveLogger.warning), [`log_stat`](logger.md#JsonLogger.log_stat), [`process_event_message`](logger.md#CollectiveLogger.process_event_message), [`log`](logger.md#CollectiveLogger.log), [`log_dict`](logger.md#ConsoleLogger.log_dict), [`log_stat`](logger.md#ConsoleLogger.log_stat), [`debug`](logger.md#CollectiveLogger.debug), [`log_dict`](logger.md#MultiLogger.log_dict), [`log_stat`](logger.md#MultiLogger.log_stat), [`error`](logger.md#CollectiveLogger.error), [`critical`](logger.md#CollectiveLogger.critical), [`log_dict`](logger.md#JsonLogger.log_dict), [`log_stat`](logger.md#WandBLogger.log_stat)

### `MultiLogger`  ·  implements/extends BaseLogger
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py:154`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L154)
- doc: Logger that can log to multiple loggers at oncce.
- signature: `class MultiLogger(BaseLogger):`
- members:
  - `log_dict(self, data: Dict, event: LogEvent, step: Optional[int] = None)` — [`L164`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L164)
  - `log_file(self, file_path: str)` — [`L168`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L168)
  - `log_stat(self, key: str, value: float, event: LogEvent, step: Optional[int] = None)` — [`L160`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L160)
  - `stop(self)` — [`L172`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L172)
  - `loggers` — [`L158`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L158)
- protocol/private: `__init__`[`L157`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L157)
- uses (calls/refs, reference-scoped): [`LogEvent`](logger.md#LogEvent), [`BaseLogger`](logger.md#BaseLogger), [`log_dict`](logger.md#BaseLogger.log_dict), [`log_stat`](logger.md#BaseLogger.log_stat), [`log_file`](logger.md#BaseLogger.log_file), [`stop`](logger.md#BaseLogger.stop)
- used by: [`BaseLogger`](logger.md#BaseLogger), [`_make_multi_logger`](logger.md#_make_multi_logger), [`log_dict`](logger.md#BaseLogger.log_dict), [`log_stat`](logger.md#BaseLogger.log_stat), [`log_file`](logger.md#BaseLogger.log_file), [`stop`](logger.md#BaseLogger.stop)

### `WandBLogger`  ·  implements/extends BaseLogger
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py:177`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L177)
- doc: Logger for wandb.ai.
- signature: `class WandBLogger(BaseLogger):`
- members:
  - `log_file(self, file_path: str)` — [`L198`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L198)
  - `log_stat(self, key: str, value: float, event: Union[LogEvent, str], step: Optional[int] = None)` — [`L190`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L190)
  - `stop(self)` — [`L201`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L201)
  - `detailed_logging` — [`L187`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L187)
  - `unique_token` — [`L188`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L188)
- protocol/private: `__init__`[`L180`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L180)
- uses (calls/refs, reference-scoped): [`LogEvent`](logger.md#LogEvent), [`BaseLogger`](logger.md#BaseLogger), [`LoggerConfig`](../config_dataclasses/logger.md#LoggerConfig)
- used by: [`BaseLogger`](logger.md#BaseLogger), [`_make_multi_logger`](logger.md#_make_multi_logger), [`log_stat`](logger.md#BaseLogger.log_stat), [`log_file`](logger.md#BaseLogger.log_file), [`stop`](logger.md#BaseLogger.stop)

## Functions
- `_make_multi_logger(cfg: LoggerConfig)` — [`L329`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L329) — Creates a MultiLogger given a config
- `config_logger(*args, **kwargs)` — [`L368`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L368)
- `describe(x: np.ndarray)` — [`L345`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L345) — Generate summary statistics for an array of metrics (mean, std, min, max).
- `get_logger()` — [`L364`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L364)
- `init_logger()` — [`L360`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L360)

## Module values
- `EVENT_COLOURS` — [`L48`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L48)
- `LOGGERS` — [`L357`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/utils/logger.py#L357)

