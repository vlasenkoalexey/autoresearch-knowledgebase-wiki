---
title: 'Module: domains/train_opt/mechanisms/crash_memory.py'
type: catalog
provenance: extracted
module: domains/train_opt/mechanisms/crash_memory.py
status: fresh
symbol_base: scip-python python bilevel-autoresearch 0.0.0 `domains.train_opt.mechanisms.crash_memory`/
symbols:
  CrashMemory.record: CrashMemory#record().
  CrashMemory.get_warning_text: CrashMemory#get_warning_text().
  CrashMemory._crashes: CrashMemory#_crashes.
  CrashRecord: CrashRecord#
  CrashMemory: CrashMemory#
  CrashMemory.crash_count: CrashMemory#crash_count().
  CrashRecord.param: CrashRecord#param.
  CrashRecord.value: CrashRecord#value.
  CrashRecord.error_hint: CrashRecord#error_hint.
  CrashMemory._param_crash_counts: CrashMemory#_param_crash_counts.
  logger: logger.
  CrashRecord.iteration: CrashRecord#iteration.
  CrashMemory.__init__: CrashMemory#__init__().
---
# Module: [`domains/train_opt/mechanisms/crash_memory.py`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py)

## Classes
### `CrashMemory`
- def: [`domains/train_opt/mechanisms/crash_memory.py:20`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L20)
- doc: Tracks which parameter changes caused crashes so the LLM can avoid them.
- signature: `class CrashMemory:`
- members:
  - `crash_count(self)` — [`L47`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L47)
  - `get_warning_text(self)` — [`L50`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L50) — Generate a warning block to inject into the proposal prompt. — documented in [domains-train_opt-runner](../../../../concepts/domains-train_opt-runner.md)
  - `record(self, changes: dict, iteration: int, error_hint: str = "timeout/OOM")` — [`L33`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L33) — Record a crash caused by the given parameter changes. — documented in [domains-train_opt-runner](../../../../concepts/domains-train_opt-runner.md)
- protocol/private: `__init__`[`L28`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L28), `_crashes`[`L29`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L29), `_param_crash_counts`[`L31`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L31)
- uses (calls/refs, reference-scoped): [`CrashRecord`](crash_memory.md#CrashRecord), [`error_hint`](crash_memory.md#CrashRecord.error_hint), [`param`](crash_memory.md#CrashRecord.param), [`value`](crash_memory.md#CrashRecord.value), [`iteration`](crash_memory.md#CrashRecord.iteration), [`logger`](crash_memory.md#logger)
- used by: [`run_iteration`](../runner.md#TrainRunner.run_iteration), [`_propose`](../runner.md#TrainRunner._propose), [`crash_memory`](../runner.md#TrainRunner.crash_memory)

### `CrashRecord`
- def: [`domains/train_opt/mechanisms/crash_memory.py:12`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L12)
- doc: Records a single crash event for crash memory.
- signature: `class CrashRecord:`
- members:
  - `error_hint` — [`L17`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L17)
  - `iteration` — [`L16`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L16)
  - `param` — [`L14`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L14)
  - `value` — [`L15`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L15)
- used by: [`record`](crash_memory.md#CrashMemory.record), [`get_warning_text`](crash_memory.md#CrashMemory.get_warning_text), [`_crashes`](crash_memory.md#CrashMemory._crashes)

## Module values
- `logger` — [`L8`](../../../../../../../raw/code/bilevel-autoresearch/domains/train_opt/mechanisms/crash_memory.py#L8)

