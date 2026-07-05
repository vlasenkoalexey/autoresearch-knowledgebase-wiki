---
title: 'Module: domains/train_opt/outer.py'
type: catalog
provenance: extracted
module: domains/train_opt/outer.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.outer`/
symbols:
  TrainOuterLoop.run: TrainOuterLoop#run().
  TrainOuterLoop._analyze: TrainOuterLoop#_analyze().
  TrainOuterLoop._build_report: TrainOuterLoop#_build_report().
  TrainOuterLoop._apply_analysis: TrainOuterLoop#_apply_analysis().
  logger: logger.
  TrainOuterLoop.runner: TrainOuterLoop#runner.
  TrainOuterLoop.artifacts_dir: TrainOuterLoop#artifacts_dir.
  TrainOuterLoop: TrainOuterLoop#
  TrainOuterLoop.__init__: TrainOuterLoop#__init__().
  TrainOuterLoop.outer_trace: TrainOuterLoop#outer_trace.
  TrainOuterLoop.max_outer_cycles: TrainOuterLoop#max_outer_cycles.
  OUTER_SYSTEM: OUTER_SYSTEM.
  OUTER_PROMPT: OUTER_PROMPT.
  TrainOuterLoop.client: TrainOuterLoop#client.
---
# Module: [`domains/train_opt/outer.py`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py)

## Classes
### `TrainOuterLoop`
- def: [`domains/train_opt/outer.py:71`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L71)
- doc: Outer loop that modifies the inner loop's search configuration.
- signature: `class TrainOuterLoop:`
- members:
  - `_analyze(self, cycle: int)` — [`L142`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L142) — Ask outer LLM to analyze inner trace and propose search config changes. — documented in [core-llm_client](../../../concepts/core-llm_client.md)
  - `_apply_analysis(self, analysis: dict, cycle: int)` — [`L188`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L188) — Apply outer loop analysis to inner loop's search config. — documented in [domains-train_opt-config](../../../concepts/domains-train_opt-config.md)
  - `_build_report(self)` — [`L231`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L231) — Build final experiment report. — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `run(self)` — [`L88`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L88) — Run the full bilevel experiment. — documented in [domains-train_opt-config](../../../concepts/domains-train_opt-config.md)
  - `artifacts_dir` — [`L84`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L84) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
  - `client` — [`L82`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L82)
  - `max_outer_cycles` — [`L83`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L83)
  - `outer_trace` — [`L86`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L86)
  - `runner` — [`L81`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L81) — documented in [domains-train_opt-outer](../../../concepts/domains-train_opt-outer.md)
- protocol/private: `__init__`[`L74`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L74)
- uses (calls/refs, reference-scoped): [`active_params`](config.md#SearchConfig.active_params), [`parse_json_response`](../../core/llm_client.md#parse_json_response), [`run_iteration`](runner.md#TrainRunner.run_iteration), [`call`](../../core/llm_client.md#LLMClient.call), [`frozen_params`](config.md#SearchConfig.frozen_params), [`strategy`](config.md#SearchConfig.strategy), [`LLMClient`](../../core/llm_client.md#LLMClient), [`run_baseline`](runner.md#TrainRunner.run_baseline), [`guidance`](config.md#SearchConfig.guidance), [`search_config`](runner.md#TrainRunner.search_config), [`val_bpb`](runner.md#TrainResult.val_bpb), [`trace`](runner.md#TrainRunner.trace), [`status`](runner.md#TrainResult.status), [`best_bpb`](runner.md#TrainTrace.best_bpb), [`results`](runner.md#TrainTrace.results), [`summary`](runner.md#TrainTrace.summary), [`description`](runner.md#TrainResult.description), [`logger`](outer.md#logger), [`iteration`](runner.md#TrainResult.iteration), [`best_iteration`](runner.md#TrainTrace.best_iteration), [`changes`](runner.md#TrainResult.changes), [`TrainRunner`](runner.md#TrainRunner), [`editable_params`](config.md#SearchConfig.editable_params), [`artifacts_dir`](runner.md#TrainRunner.artifacts_dir), [`inner_budget`](config.md#SearchConfig.inner_budget), [`OUTER_PROMPT`](outer.md#OUTER_PROMPT), [`OUTER_SYSTEM`](outer.md#OUTER_SYSTEM)
- used by: [`run_group_c`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_c), [`run_group_b`](../../experiments/ablations/paper_ablation/run_ablation.md#run_group_b), [`cmd_bilevel`](cli.md#cmd_bilevel), [`_v`](../../experiments/ablations/paper_ablation/run_ablation.md#_v), [`_v`](cli.md#_v)

## Module values
- `OUTER_PROMPT` — [`L24`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L24)
- `OUTER_SYSTEM` — [`L18`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L18)
- `logger` — [`L16`](../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/outer.py#L16)

