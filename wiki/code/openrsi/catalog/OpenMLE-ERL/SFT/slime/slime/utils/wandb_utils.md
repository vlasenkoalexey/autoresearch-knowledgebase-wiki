---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.wandb_utils`/
symbols:
  init_wandb_primary: init_wandb_primary().
  init_wandb_secondary: init_wandb_secondary().
  logger: logger.
  _coerce_summary_scalar: _coerce_summary_scalar().
  log_metrics: log_metrics().
  extract_summary_metrics: extract_summary_metrics().
  _is_offline_mode: _is_offline_mode().
  _init_wandb_common: _init_wandb_common().
  _compute_config_for_logging: _compute_config_for_logging().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py)

## Functions
- `_coerce_summary_scalar(value)` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L12) — Convert logged values into summary-safe scalars when possible.
- `_compute_config_for_logging(args)` — [`L132`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L132)
- `_init_wandb_common()` — [`L200`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L200)
- `_is_offline_mode(args)` — [`L60`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L60) — Detect whether W&B should run in offline mode.
- `extract_summary_metrics(metrics: Mapping[str, object])` — [`L36`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L36) — Mirror scalar metrics into summary so W&B can discover them reliably.
- `init_wandb_primary(args)` — [`L72`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L72)
- `init_wandb_secondary(args, router_addr=None)` — [`L145`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L145)
- `log_metrics(metrics: Mapping[str, object], *, update_summary: bool = True)` — [`L49`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L49) — Log metrics to W&B and optionally mirror scalar values into summary.

## Module values
- `logger` — [`L9`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/wandb_utils.py#L9)

