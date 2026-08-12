---
title: 'Module: OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py'
type: catalog
provenance: extracted
module: OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-ERL.SFT.slime.slime.utils.health_monitor`/
symbols:
  RolloutHealthMonitor._health_monitor_loop: RolloutHealthMonitor#_health_monitor_loop().
  logger: logger.
  RolloutHealthMonitor.stop: RolloutHealthMonitor#stop().
  RolloutHealthMonitor.start: RolloutHealthMonitor#start().
  RolloutHealthMonitor._pause_event: RolloutHealthMonitor#_pause_event.
  RolloutHealthMonitor._stop_event: RolloutHealthMonitor#_stop_event.
  RolloutHealthMonitor._run_health_checks: RolloutHealthMonitor#_run_health_checks().
  RolloutHealthMonitor.resume: RolloutHealthMonitor#resume().
  RolloutHealthMonitor._check_engine_health: RolloutHealthMonitor#_check_engine_health().
  RolloutHealthMonitor.pause: RolloutHealthMonitor#pause().
  RolloutHealthMonitor._thread: RolloutHealthMonitor#_thread.
  RolloutHealthMonitor._engine_group: RolloutHealthMonitor#_engine_group.
  RolloutHealthMonitor._kill_engine: RolloutHealthMonitor#_kill_engine().
  RolloutHealthMonitor._is_checking_enabled: RolloutHealthMonitor#_is_checking_enabled.
  RolloutHealthMonitor._need_first_wait: RolloutHealthMonitor#_need_first_wait.
  RolloutHealthMonitor.is_checking_enabled: RolloutHealthMonitor#is_checking_enabled().
  RolloutHealthMonitor: RolloutHealthMonitor#
  RolloutHealthMonitor._check_interval: RolloutHealthMonitor#_check_interval.
  RolloutHealthMonitor._check_timeout: RolloutHealthMonitor#_check_timeout.
  RolloutHealthMonitor._check_first_wait: RolloutHealthMonitor#_check_first_wait.
  RolloutHealthMonitor.__init__: RolloutHealthMonitor#__init__().
---
# Module: [`OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py)

## Classes
### `RolloutHealthMonitor`
- def: [`OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py:10`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L10)
- doc: Health monitor for rollout engines.
- signature: `class RolloutHealthMonitor:`
- members:
  - `is_checking_enabled(self)` — [`L101`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L101) — Return whether health checking is currently enabled (not paused).
  - `pause(self)` — [`L84`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L84) — Pause health checking. Called when engines are offloaded.
  - `resume(self)` — [`L92`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L92) — Resume health checking. Called when engines are onloaded.
  - `start(self)` — [`L35`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L35) — Start the health monitor thread. Called once during initialization.
  - `stop(self)` — [`L61`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L61) — Stop the health monitor thread completely. Called during dispose.
- protocol/private: `__init__`[`L23`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L23), `_check_engine_health`[`L145`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L145), `_check_first_wait`[`L31`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L31), `_check_interval`[`L29`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L29), `_check_timeout`[`L30`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L30), `_engine_group`[`L24`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L24), `_health_monitor_loop`[`L105`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L105), `_is_checking_enabled`[`L33`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L33), `_kill_engine`[`L160`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L160), `_need_first_wait`[`L32`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L32), `_pause_event`[`L28`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L28), `_run_health_checks`[`L137`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L137), `_stop_event`[`L27`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L27), `_thread`[`L26`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L26)
- uses (calls/refs, reference-scoped): [`logger`](health_monitor.md#logger)
- used by: [`_health_monitors`](../ray/rollout.md#RolloutManager._health_monitors)

## Module values
- `logger` — [`L7`](../../../../../../../../../raw/code/openrsi/OpenMLE-ERL/SFT/slime/slime/utils/health_monitor.py#L7)

