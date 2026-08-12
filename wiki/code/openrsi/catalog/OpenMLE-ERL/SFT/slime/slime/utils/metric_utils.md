---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.metric_utils`/
symbols:
  dict_add_prefix: dict_add_prefix().
  compute_rollout_step: compute_rollout_step().
  compute_pass_rate: compute_pass_rate().
  has_repetition: has_repetition().
  _estimate_pass_at_k: _estimate_pass_at_k().
  compute_statistics: compute_statistics().
  _estimate_pass_at_k.estimator: _estimate_pass_at_k().estimator().
  compression_ratio: compression_ratio().
  logger: logger.
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py)

## Functions
- `_estimate_pass_at_k(num_samples, num_correct, k)` — [`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L43) — Estimates pass@k of each problem and returns them in an array.
- `compression_ratio(data: str | bytes, *, encoding: str = "utf-8", algorithm: Literal["zlib", "gzip", "bz2", "lzma"] = "zlib", level: int = 9)` — [`L69`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L69)
- `compute_pass_rate(flat_rewards: list[float], group_size: int, num_groups: int | None = None)` — [`L14`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L14)
- `compute_rollout_step(args, rollout_id)` — [`L120`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L120)
- `compute_statistics(values: list[float])` — [`L59`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L59)
- `dict_add_prefix(d: dict[str, Any], prefix: str)` — [`L10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L10)
- `estimator(n, c, k)` — [`L48`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L48) — Calculates 1 - comb(n - c, k) / comb(n, k).
- `has_repetition(text: str)` — [`L113`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L113)

## Module values
- `logger` — [`L7`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/metric_utils.py#L7)

