---
title: 'Module: rdagent/components/coder/factor_coder/eva_utils.py'
type: catalog
provenance: extracted
module: rdagent/components/coder/factor_coder/eva_utils.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.components.coder.factor_coder.eva_utils`/Factor
symbols:
  FactorValueEvaluator.evaluate: ValueEvaluator#evaluate().
  FactorEvaluator: Evaluator#
  FactorEvaluator.evaluate: Evaluator#evaluate().
  FactorCodeEvaluator.evaluate: CodeEvaluator#evaluate().
  FactorFinalDecisionEvaluator.evaluate: FinalDecisionEvaluator#evaluate().
  FactorOutputFormatEvaluator.evaluate: OutputFormatEvaluator#evaluate().
  FactorEvaluator.scen: Evaluator#scen.
  FactorEvaluator._get_df: Evaluator#_get_df().
  FactorCorrelationEvaluator.evaluate: CorrelationEvaluator#evaluate().
  FactorInfEvaluator.evaluate: InfEvaluator#evaluate().
  FactorSingleColumnEvaluator.evaluate: SingleColumnEvaluator#evaluate().
  FactorDatetimeDailyEvaluator.evaluate: DatetimeDailyEvaluator#evaluate().
  FactorRowCountEvaluator.evaluate: RowCountEvaluator#evaluate().
  FactorIndexEvaluator.evaluate: IndexEvaluator#evaluate().
  FactorMissingValuesEvaluator.evaluate: MissingValuesEvaluator#evaluate().
  FactorEqualValueRatioEvaluator.evaluate: EqualValueRatioEvaluator#evaluate().
  FactorSingleColumnEvaluator: SingleColumnEvaluator#
  FactorRowCountEvaluator: RowCountEvaluator#
  FactorIndexEvaluator: IndexEvaluator#
  FactorEqualValueRatioEvaluator: EqualValueRatioEvaluator#
  FactorCorrelationEvaluator: CorrelationEvaluator#
  FactorCodeEvaluator: CodeEvaluator#
  FactorValueEvaluator: ValueEvaluator#
  FactorFinalDecisionEvaluator: FinalDecisionEvaluator#
  FactorInfEvaluator: InfEvaluator#
  FactorOutputFormatEvaluator: OutputFormatEvaluator#
  FactorDatetimeDailyEvaluator: DatetimeDailyEvaluator#
  FactorMissingValuesEvaluator: MissingValuesEvaluator#
  FactorCorrelationEvaluator.__init__: CorrelationEvaluator#__init__().
  FactorEvaluator.__init__: Evaluator#__init__().
  FactorCorrelationEvaluator.hard_check: CorrelationEvaluator#hard_check.
  FactorEvaluator.__str__: Evaluator#__str__().
---
# Module: [`rdagent/components/coder/factor_coder/eva_utils.py`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py)

## Classes
### `FactorCodeEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:67`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L67)
- signature: `class FactorCodeEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, target_task: FactorTask, implementation: Workspace, execution_feedback: str, value_feedback: str = "", gt_implementation: Workspace = None, **kwargs)` — [`L68`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L68)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`FactorTask`](factor.md#FactorTask), [`FACTOR_COSTEER_SETTINGS`](config.md#FACTOR_COSTEER_SETTINGS), [`chat_token_limit`](../../../oai/backend/base.md#APIBackend.chat_token_limit), [`build_messages_and_calculate_token`](../../../oai/backend/base.md#APIBackend.build_messages_and_calculate_token), [`get_task_information`](factor.md#FactorTask.get_task_information), [`scen`](eva_utils.md#FactorEvaluator.scen), [`all_codes`](../../../core/experiment.md#Workspace.all_codes), [`simple_background`](config.md#FactorCoSTEERSettings.simple_background)
- used by: [`evaluate`](evaluators.md#FactorEvaluatorForCoder.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate), [`code_evaluator`](evaluators.md#FactorEvaluatorForCoder.code_evaluator)

### `FactorCorrelationEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:348`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L348)
- signature: `class FactorCorrelationEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L353`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L353)
  - `hard_check` — [`L351`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L351)
- protocol/private: `__init__`[`L349`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L349)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`_get_df`](eva_utils.md#FactorEvaluator._get_df), [`__init__`](eva_utils.md#FactorEvaluator.__init__)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)  (1 test-only)

### `FactorDatetimeDailyEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:217`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L217)
- signature: `class FactorDatetimeDailyEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L218`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L218)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`_get_df`](eva_utils.md#FactorEvaluator._get_df)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)

### `FactorEqualValueRatioEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:317`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L317)
- signature: `class FactorEqualValueRatioEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L318`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L318)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`_get_df`](eva_utils.md#FactorEvaluator._get_df)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)  (1 test-only)

### `FactorEvaluator`
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:16`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L16)
- doc: Although the init method is same to Evaluator, but we want to emphasize they are different
- signature: `class FactorEvaluator:`
- members:
  - `evaluate(self, target_task: Task, implementation: Workspace, gt_implementation: Workspace, **kwargs)` — [`L23`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L23) — You can get the dataframe by
  - `scen` — [`L20`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L20)
- protocol/private: `__init__`[`L19`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L19), `__str__`[`L63`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L63), `_get_df`[`L46`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L46)
- uses (calls/refs, reference-scoped): [`Task`](../../../core/experiment.md#Task), [`Workspace`](../../../core/experiment.md#Workspace), [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorCodeEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorFinalDecisionEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorOutputFormatEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorCorrelationEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorDatetimeDailyEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorEqualValueRatioEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorIndexEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorInfEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorMissingValuesEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorRowCountEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorSingleColumnEvaluator.evaluate), [`FactorCorrelationEvaluator`](eva_utils.md#FactorCorrelationEvaluator), [`FactorEqualValueRatioEvaluator`](eva_utils.md#FactorEqualValueRatioEvaluator), [`FactorIndexEvaluator`](eva_utils.md#FactorIndexEvaluator), [`FactorRowCountEvaluator`](eva_utils.md#FactorRowCountEvaluator), [`FactorSingleColumnEvaluator`](eva_utils.md#FactorSingleColumnEvaluator), [`execute`](../../../core/experiment.md#Workspace.execute), [`FactorCodeEvaluator`](eva_utils.md#FactorCodeEvaluator), [`FactorFinalDecisionEvaluator`](eva_utils.md#FactorFinalDecisionEvaluator), [`FactorValueEvaluator`](eva_utils.md#FactorValueEvaluator), [`FactorDatetimeDailyEvaluator`](eva_utils.md#FactorDatetimeDailyEvaluator), [`FactorInfEvaluator`](eva_utils.md#FactorInfEvaluator), [`FactorMissingValuesEvaluator`](eva_utils.md#FactorMissingValuesEvaluator), [`FactorOutputFormatEvaluator`](eva_utils.md#FactorOutputFormatEvaluator)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorCodeEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorFinalDecisionEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorOutputFormatEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorCorrelationEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorDatetimeDailyEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorEqualValueRatioEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorIndexEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorInfEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorMissingValuesEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorRowCountEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorSingleColumnEvaluator.evaluate), [`FactorCorrelationEvaluator`](eva_utils.md#FactorCorrelationEvaluator), [`FactorEqualValueRatioEvaluator`](eva_utils.md#FactorEqualValueRatioEvaluator), [`FactorIndexEvaluator`](eva_utils.md#FactorIndexEvaluator), [`FactorRowCountEvaluator`](eva_utils.md#FactorRowCountEvaluator), [`FactorSingleColumnEvaluator`](eva_utils.md#FactorSingleColumnEvaluator), [`FactorCodeEvaluator`](eva_utils.md#FactorCodeEvaluator), [`FactorFinalDecisionEvaluator`](eva_utils.md#FactorFinalDecisionEvaluator), [`FactorValueEvaluator`](eva_utils.md#FactorValueEvaluator), [`FactorDatetimeDailyEvaluator`](eva_utils.md#FactorDatetimeDailyEvaluator), [`FactorInfEvaluator`](eva_utils.md#FactorInfEvaluator), [`FactorMissingValuesEvaluator`](eva_utils.md#FactorMissingValuesEvaluator), [`FactorOutputFormatEvaluator`](eva_utils.md#FactorOutputFormatEvaluator), [`__init__`](eva_utils.md#FactorCorrelationEvaluator.__init__)  (3 test-only)

### `FactorFinalDecisionEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:478`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L478)
- signature: `class FactorFinalDecisionEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, target_task: FactorTask, execution_feedback: str, value_feedback: str, code_feedback: str, **kwargs)` — [`L479`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L479)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`FactorTask`](factor.md#FactorTask), [`chat_token_limit`](../../../oai/backend/base.md#APIBackend.chat_token_limit), [`build_messages_and_calculate_token`](../../../oai/backend/base.md#APIBackend.build_messages_and_calculate_token), [`get_task_information`](factor.md#FactorTask.get_task_information), [`scen`](eva_utils.md#FactorEvaluator.scen)
- used by: [`evaluate`](evaluators.md#FactorEvaluatorForCoder.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate), [`final_decision_evaluator`](evaluators.md#FactorEvaluatorForCoder.final_decision_evaluator)

### `FactorIndexEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:271`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L271)
- signature: `class FactorIndexEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L272`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L272)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`_get_df`](eva_utils.md#FactorEvaluator._get_df)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)  (1 test-only)

### `FactorInfEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:120`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L120)
- signature: `class FactorInfEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L121`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L121)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`_get_df`](eva_utils.md#FactorEvaluator._get_df)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)

### `FactorMissingValuesEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:296`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L296)
- signature: `class FactorMissingValuesEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L297`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L297)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`_get_df`](eva_utils.md#FactorEvaluator._get_df)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)

### `FactorOutputFormatEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:163`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L163)
- signature: `class FactorOutputFormatEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L164`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L164)
- uses (calls/refs, reference-scoped): [`T`](../../../utils/agent/tpl.md#T), [`r`](../../../utils/agent/tpl.md#RDAT.r), [`APIBackend`](../../../oai/llm_utils.md#APIBackend), [`build_messages_and_create_chat_completion`](../../../oai/backend/base.md#APIBackend.build_messages_and_create_chat_completion), [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`target_task`](../../../core/experiment.md#Workspace.target_task), [`scen`](eva_utils.md#FactorEvaluator.scen), [`_get_df`](eva_utils.md#FactorEvaluator._get_df)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)

### `FactorRowCountEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:247`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L247)
- signature: `class FactorRowCountEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L248`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L248)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`_get_df`](eva_utils.md#FactorEvaluator._get_df)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)  (1 test-only)

### `FactorSingleColumnEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:142`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L142)
- signature: `class FactorSingleColumnEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace)` — [`L143`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L143)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`_get_df`](eva_utils.md#FactorEvaluator._get_df)
- used by: [`evaluate`](eva_utils.md#FactorValueEvaluator.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate)  (1 test-only)

### `FactorValueEvaluator`  ·  implements/extends FactorEvaluator
- def: [`rdagent/components/coder/factor_coder/eva_utils.py:389`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L389)
- signature: `class FactorValueEvaluator(FactorEvaluator):`
- members:
  - `evaluate(self, implementation: Workspace, gt_implementation: Workspace, version: int = 1, **kwargs)` — [`L390`](../../../../../../../../raw/code/rd-agent/rdagent/components/coder/factor_coder/eva_utils.py#L390)
- uses (calls/refs, reference-scoped): [`Workspace`](../../../core/experiment.md#Workspace), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorOutputFormatEvaluator.evaluate), [`scen`](eva_utils.md#FactorEvaluator.scen), [`_get_df`](eva_utils.md#FactorEvaluator._get_df), [`evaluate`](eva_utils.md#FactorCorrelationEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorDatetimeDailyEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorEqualValueRatioEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorIndexEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorInfEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorMissingValuesEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorRowCountEvaluator.evaluate), [`evaluate`](eva_utils.md#FactorSingleColumnEvaluator.evaluate), [`FactorCorrelationEvaluator`](eva_utils.md#FactorCorrelationEvaluator), [`FactorEqualValueRatioEvaluator`](eva_utils.md#FactorEqualValueRatioEvaluator), [`FactorIndexEvaluator`](eva_utils.md#FactorIndexEvaluator), [`FactorRowCountEvaluator`](eva_utils.md#FactorRowCountEvaluator), [`FactorSingleColumnEvaluator`](eva_utils.md#FactorSingleColumnEvaluator), [`FactorDatetimeDailyEvaluator`](eva_utils.md#FactorDatetimeDailyEvaluator), [`FactorInfEvaluator`](eva_utils.md#FactorInfEvaluator), [`FactorMissingValuesEvaluator`](eva_utils.md#FactorMissingValuesEvaluator), [`FactorOutputFormatEvaluator`](eva_utils.md#FactorOutputFormatEvaluator)
- used by: [`evaluate`](evaluators.md#FactorEvaluatorForCoder.evaluate), [`FactorEvaluator`](eva_utils.md#FactorEvaluator), [`evaluate`](eva_utils.md#FactorEvaluator.evaluate), [`value_evaluator`](evaluators.md#FactorEvaluatorForCoder.value_evaluator)

