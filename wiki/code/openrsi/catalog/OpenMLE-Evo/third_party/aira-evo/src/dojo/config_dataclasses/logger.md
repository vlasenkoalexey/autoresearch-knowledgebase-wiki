---
title: 'Module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py'
type: catalog
provenance: extracted
module: OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Evo.third_party.aira-evo.src.dojo.config_dataclasses.logger`/LoggerConfig#
symbols:
  LoggerConfig: ''
  LoggerConfig.output_dir: output_dir.
  LoggerConfig.validate: validate().
  LoggerConfig.print_config: print_config.
  LoggerConfig.write_env_vars: write_env_vars.
  LoggerConfig.use_console: use_console.
  LoggerConfig.use_wandb: use_wandb.
  LoggerConfig.use_json: use_json.
  LoggerConfig.wandb_entity: wandb_entity.
  LoggerConfig.wandb_project_name: wandb_project_name.
  LoggerConfig.tags: tags.
  LoggerConfig.detailed_logging: detailed_logging.
---
# Module: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py)

## Classes
### `LoggerConfig`  ·  implements/extends BaseConfig
- def: [`OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py:17`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L17)
- signature: `class LoggerConfig(BaseConfig):`
- members:
  - `validate(self)` — [`L94`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L94)
  - `detailed_logging` — [`L71`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L71)
  - `output_dir` — [`L18`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L18)
  - `print_config` — [`L79`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L79)
  - `tags` — [`L63`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L63)
  - `use_console` — [`L27`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L27)
  - `use_json` — [`L41`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L41)
  - `use_wandb` — [`L34`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L34)
  - `wandb_entity` — [`L48`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L48)
  - `wandb_project_name` — [`L55`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L55)
  - `write_env_vars` — [`L86`](../../../../../../../../../../raw/code/openrsi/OpenMLE-Evo/third_party/aira-evo/src/dojo/config_dataclasses/logger.py#L86)
- uses (calls/refs, reference-scoped): [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`validate`](../../aira_core/config/base.md#BaseConfig.validate), [`get_log_dir`](../utils/environment.md#get_log_dir)
- used by: [`_main`](../main_run.md#_main), [`BaseConfig`](../../aira_core/config/base.md#BaseConfig), [`validate`](../../aira_core/config/base.md#BaseConfig.validate), [`logger`](run.md#RunConfig.logger), [`_make_multi_logger`](../utils/logger.md#_make_multi_logger), [`main`](../main_run.md#main), [`print_config_tree`](../utils/rich_utils.md#print_config_tree), [`save`](run.md#RunConfig.save), [`__init__`](../utils/logger.md#ConsoleLogger.__init__), [`save`](runner.md#RunnerConfig.save), [`logger`](runner.md#RunnerConfig.logger), [`__init__`](../utils/logger.md#BaseLogger.__init__), [`__init__`](../utils/logger.md#JsonLogger.__init__), [`__init__`](../utils/logger.md#WandBLogger.__init__)

