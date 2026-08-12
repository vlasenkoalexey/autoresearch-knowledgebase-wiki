---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/timer.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/timer.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.timer`/
symbols:
  timer: timer().
  Timer: Timer#
  inverse_timer: inverse_timer().
  Timer.end: Timer#end().
  Timer.start: Timer#start().
  Timer.context: Timer#context().
  with_defer: with_defer().
  Timer.timers: Timer#timers.
  timer.wrapper: timer().wrapper().
  Timer.start_time: Timer#start_time.
  Timer.reset: Timer#reset().
  Timer.add: Timer#add().
  Timer.log_dict: Timer#log_dict().
  with_defer.decorator: with_defer().decorator().
  logger: logger.
  with_defer.decorator.wrapper: with_defer().decorator().wrapper().
  __all__: __all__.
  Timer.__init__: Timer#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/timer.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py)

## Classes
### `Timer`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/timer.py:15`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L15)
- signature: `class Timer(metaclass=SingletonMeta):`
- members:
  - `add(self, name, elapsed_time)` — [`L40`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L40)
  - `context(self, name)` — [`L47`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L47)
  - `end(self, name)` — [`L26`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L26)
  - `log_dict(self)` — [`L43`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L43)
  - `reset(self, name=None)` — [`L34`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L34)
  - `start(self, name)` — [`L20`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L20)
  - `start_time` — [`L18`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L18)
  - `timers` — [`L17`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L17)
- protocol/private: `__init__`[`L16`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L16)
- uses (calls/refs, reference-scoped): [`SingletonMeta`](misc.md#SingletonMeta), [`logger`](timer.md#logger)
- used by: [`timer`](timer.md#timer), [`init`](../backends/megatron_utils/actor.md#MegatronTrainRayActor.init), [`log_perf_data_raw`](train_metric_utils.md#log_perf_data_raw), [`init`](../backends/fsdp_utils/actor.md#FSDPTrainRayActor.init), [`inverse_timer`](timer.md#inverse_timer), [`process_rollout_data`](data.md#process_rollout_data), [`wrapper`](timer.md#timer.wrapper)

## Functions
- `decorator(fn)` — [`L93`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L93)
- `inverse_timer(name)` — [`L84`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L84)
- `timer(name_or_func)` — [`L55`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L55) — Can be used either as a decorator or a context manager:
- `with_defer(deferred_func)` — [`L92`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L92)
- `wrapper(*args, **kwargs)` — [`L76`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L76)
- `wrapper(*args, **kwargs)` — [`L95`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L95)

## Module values
- `__all__` — [`L10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L10)
- `logger` — [`L12`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/timer.py#L12)

