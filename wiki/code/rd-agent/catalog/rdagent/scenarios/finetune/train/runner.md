---
title: 'Module: rdagent/scenarios/finetune/train/runner.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/finetune/train/runner.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.finetune.train.runner`/
symbols:
  FTRunnerEvolvingStrategy.implement_one_task: FTRunnerEvolvingStrategy#implement_one_task().
  LLMFinetuneRunner.__init__: LLMFinetuneRunner#__init__().
  LLMFinetuneRunner.develop: LLMFinetuneRunner#develop().
  LLMFinetuneRunner.get_develop_max_seconds: LLMFinetuneRunner#get_develop_max_seconds().
  FTRunnerSettings: FTRunnerSettings#
  FTRunnerEvolvingStrategy: FTRunnerEvolvingStrategy#
  LLMFinetuneRunner.compare_scores: LLMFinetuneRunner#compare_scores().
  LLMFinetuneRunner: LLMFinetuneRunner#
  LLMFinetuneRunner.compare_and_pick_fb: LLMFinetuneRunner#compare_and_pick_fb().
  FTRunnerSettings.Config: FTRunnerSettings#Config#
  FTRunnerSettings.Config.env_prefix: FTRunnerSettings#Config#env_prefix.
---
# Module: [`rdagent/scenarios/finetune/train/runner.py`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py)

## Classes
### `Config`
- def: [`rdagent/scenarios/finetune/train/runner.py:34`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L34)
- signature: `class Config:`
- members:
  - `env_prefix` — [`L35`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L35)

### `FTRunnerEvolvingStrategy`  ·  implements/extends MultiProcessEvolvingStrategy
- def: [`rdagent/scenarios/finetune/train/runner.py:38`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L38)
- doc: Evolving strategy for LLM fine-tuning runner.
- signature: `class FTRunnerEvolvingStrategy(MultiProcessEvolvingStrategy):`
- members:
  - `implement_one_task(self, target_task: Task, queried_knowledge: CoSTEERQueriedKnowledge | None = None, workspace: FBWorkspace | None = None, prev_task_feedback: CoSTEERSingleFeedback | None = None)` — [`L45`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L45) — No modification needed - directly use coder's full training config.
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`FBWorkspace`](../../../core/experiment.md#FBWorkspace), [`file_dict`](../../../core/experiment.md#FBWorkspace.file_dict), [`CoSTEERSingleFeedback`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERSingleFeedback), [`Task`](../../../core/experiment.md#Task), [`MultiProcessEvolvingStrategy`](../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`error`](../../../log/logger.md#RDAgentLog.error), [`CoSTEERQueriedKnowledge`](../../../components/coder/CoSTEER/knowledge_management.md#CoSTEERQueriedKnowledge), [`FT_YAML_FILE_NAME`](../../../components/coder/finetune/conf.md#FT_YAML_FILE_NAME)
- used by: [`MultiProcessEvolvingStrategy`](../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy), [`implement_one_task`](../../../components/coder/CoSTEER/evolving_strategy.md#MultiProcessEvolvingStrategy.implement_one_task), [`__init__`](runner.md#LLMFinetuneRunner.__init__)

### `FTRunnerSettings`  ·  implements/extends FTCoderCoSTEERSettings
- def: [`rdagent/scenarios/finetune/train/runner.py:31`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L31)
- doc: LLM Fine-tuning specific runner settings.
- signature: `class FTRunnerSettings(FTCoderCoSTEERSettings):`
- uses (calls/refs, reference-scoped): [`FTCoderCoSTEERSettings`](../../../components/coder/finetune/conf.md#FTCoderCoSTEERSettings)
- used by: [`__init__`](runner.md#LLMFinetuneRunner.__init__), [`FTCoderCoSTEERSettings`](../../../components/coder/finetune/conf.md#FTCoderCoSTEERSettings)

### `LLMFinetuneRunner`  ·  implements/extends CoSTEER
- def: [`rdagent/scenarios/finetune/train/runner.py:63`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L63)
- doc: LLM Fine-tuning specific runner that executes LLaMA-Factory configurations.
- signature: `class LLMFinetuneRunner(CoSTEER):`
- members:
  - `compare_and_pick_fb(self, base_fb, new_fb)` — [`L114`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L114) — Compare feedback for LLM fine-tuning results.
  - `compare_scores(s1, s2)` — [`L122`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L122)
  - `develop(self, exp)` — [`L95`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L95) — Execute LLaMA-Factory fine-tuning on full dataset.
  - `get_develop_max_seconds(self)` — [`L110`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L110) — Get maximum seconds for development using FT settings.
- protocol/private: `__init__`[`L66`](../../../../../../../../raw/code/rd-agent/rdagent/scenarios/finetune/train/runner.py#L66)
- uses (calls/refs, reference-scoped): [`rdagent_logger`](../../../log/__init__.md#rdagent_logger.rdagent_logger), [`info`](../../../log/logger.md#RDAgentLog.info), [`Scenario`](../../../core/scenario.md#Scenario), [`FT_RD_SETTING`](../../../app/finetune/llm/conf.md#FT_RD_SETTING), [`CoSTEER`](../../../components/coder/CoSTEER/__init__.md#CoSTEER), [`develop`](../../../components/coder/CoSTEER/__init__.md#CoSTEER.develop), [`CoSTEERMultiEvaluator`](../../../components/coder/CoSTEER/evaluators.md#CoSTEERMultiEvaluator), [`__init__`](../../../components/coder/CoSTEER/__init__.md#CoSTEER.__init__), [`scen`](../../../core/developer.md#Developer.scen), [`settings`](../../../components/coder/CoSTEER/__init__.md#CoSTEER.settings), [`FTRunnerEvaluator`](eval.md#FTRunnerEvaluator), [`FTRunnerEvolvingStrategy`](runner.md#FTRunnerEvolvingStrategy), [`FTRunnerSettings`](runner.md#FTRunnerSettings), [`max_seconds_multiplier`](../../../components/coder/CoSTEER/config.md#CoSTEERSettings.max_seconds_multiplier)
- used by: [`CoSTEER`](../../../components/coder/CoSTEER/__init__.md#CoSTEER), [`develop`](../../../components/coder/CoSTEER/__init__.md#CoSTEER.develop), [`get_develop_max_seconds`](../../../components/coder/CoSTEER/__init__.md#CoSTEER.get_develop_max_seconds)

