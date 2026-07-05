---
title: 'Module: rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py'
type: catalog
provenance: extracted
module: rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py
status: fresh
symbol_base: scip-python python rd-agent 0.0.0 `rdagent.scenarios.kaggle.experiment.templates.feedback-prize-english-language-learning.feature.feature`/
symbols:
  IdentityFeature.vectorizer: IdentityFeature#vectorizer.
  IdentityFeature.transform: IdentityFeature#transform().
  feature_engineering_cls: feature_engineering_cls.
  IdentityFeature: IdentityFeature#
  IdentityFeature.fit: IdentityFeature#fit().
---
# Module: [`rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py)

## Classes
### `IdentityFeature`
- def: [`rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py:10`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py#L10)
- signature: `class IdentityFeature:`
- members:
  - `fit(self, train_df: pd.DataFrame)` — [`L11`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py#L11) — Fit the feature engineering model to the training data.
  - `transform(self, X: pd.DataFrame)` — [`L18`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py#L18) — Transform the input data.
  - `vectorizer` — [`L15`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py#L15)
- used by: [`feature_engineering_cls`](feature.md#feature_engineering_cls)

## Module values
- `feature_engineering_cls` — [`L27`](../../../../../../../../../../../raw/code/rd-agent/rdagent/scenarios/kaggle/experiment/templates/feedback-prize-english-language-learning/feature/feature.py#L27)

