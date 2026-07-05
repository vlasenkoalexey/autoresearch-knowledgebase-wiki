---
title: 'Module: rdagent/app/cli.py'
type: catalog
provenance: extracted
module: rdagent/app/cli.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.app.cli`/
symbols:
  app: app.
  health_check_cli: health_check_cli().
  fin_factor_cli: fin_factor_cli().
  fin_model_cli: fin_model_cli().
  fin_quant_cli: fin_quant_cli().
  fin_factor_report_cli: fin_factor_report_cli().
  data_science_cli: data_science_cli().
  llm_finetune_cli: llm_finetune_cli().
  CheckoutOption: CheckoutOption.
  general_model_cli: general_model_cli().
  grade_summary_cli: grade_summary_cli().
  collect_info_cli: collect_info_cli().
  server_ui: server_ui().
  CheckEnvOption: CheckEnvOption.
  CheckDockerOption: CheckDockerOption.
  CheckPortsOption: CheckPortsOption.
  ui: ui().
  ds_user_interact: ds_user_interact().
---
# Module: [`rdagent/app/cli.py`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py)

## Functions
- `collect_info_cli()` — [`L195`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L195)
- `data_science_cli(path: Optional[str] = None, checkout: CheckoutOption = True, step_n: Optional[int] = None, loop_n: Optional[int] = None, timeout: Optional[str] = None, competition: Optional[str] = None)` — [`L131`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L131)
- `ds_user_interact(port=19900)` — [`L74`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L74) — start web app to show the log traces in real time
- `fin_factor_cli(path: Optional[str] = None, step_n: Optional[int] = None, loop_n: Optional[int] = None, all_duration: Optional[str] = None, checkout: CheckoutOption = True)` — [`L83`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L83)
- `fin_factor_report_cli(report_folder: Optional[str] = None, path: Optional[str] = None, all_duration: Optional[str] = None, checkout: CheckoutOption = True)` — [`L116`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L116)
- `fin_model_cli(path: Optional[str] = None, step_n: Optional[int] = None, loop_n: Optional[int] = None, all_duration: Optional[str] = None, checkout: CheckoutOption = True)` — [`L94`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L94)
- `fin_quant_cli(path: Optional[str] = None, step_n: Optional[int] = None, loop_n: Optional[int] = None, all_duration: Optional[str] = None, checkout: CheckoutOption = True)` — [`L105`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L105)
- `general_model_cli(report_file_path: str)` — [`L126`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L126)
- `grade_summary_cli(log_folder: str)` — [`L177`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L177)
- `health_check_cli(check_env: CheckEnvOption = True, check_docker: CheckDockerOption = True, check_ports: CheckPortsOption = True)` — [`L186`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L186)
- `llm_finetune_cli(path: Optional[str] = None, checkout: CheckoutOption = True, benchmark: Optional[str] = None, benchmark_description: Optional[str] = None, dataset: Optional[str] = None, base_model: Optional[str] = None, upper_data_size_limit: Optional[int] = None, step_n: Optional[int] = None, loop_n: Optional[int] = None, timeout: Optional[str] = None)` — [`L150`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L150)
- `server_ui(port=19899)` — [`L65`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L65) — start the Flask log server in real time
- `ui(port=19899, log_dir="", debug: bool = False, data_science: bool = False)` — [`L45`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L45) — start web app to show the log traces.

## Module values
- `CheckDockerOption` — [`L41`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L41)
- `CheckEnvOption` — [`L40`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L40)
- `CheckPortsOption` — [`L42`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L42)
- `CheckoutOption` — [`L39`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L39)
- `app` — [`L37`](../../../../../../raw/code/rd-agent/rdagent/app/cli.py#L37)

