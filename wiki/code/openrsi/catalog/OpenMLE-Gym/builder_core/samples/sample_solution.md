---
title: 'Module: OpenMLE-Gym/builder_core/samples/sample_solution.py'
type: catalog
provenance: extracted
module: OpenMLE-Gym/builder_core/samples/sample_solution.py
status: fresh
symbol_base: scip-python python openrsi 0.0.0 `OpenMLE-Gym.builder_core.samples.sample_solution`/
symbols:
  main: main().
  engineer_features: engineer_features().
  impute_missing_values: impute_missing_values().
  impute_missing_values.fill_age: impute_missing_values().fill_age().
  select_features: select_features().
  load_data: load_data().
  extract_title: extract_title().
  extract_cabin_deck: extract_cabin_deck().
  extract_ticket_prefix: extract_ticket_prefix().
  impute_missing_values.fill_fare: impute_missing_values().fill_fare().
  encode_features: encode_features().
  train_model: train_model().
---
# Module: [`OpenMLE-Gym/builder_core/samples/sample_solution.py`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py)

## Functions
- `encode_features(train, test)` — [`L128`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L128) — Encode categorical features.
- `engineer_features(df)` — [`L55`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L55) — Create new features from existing data.
- `extract_cabin_deck(cabin)` — [`L37`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L37) — Extract deck letter from cabin.
- `extract_ticket_prefix(ticket)` — [`L46`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L46) — Extract ticket prefix.
- `extract_title(name)` — [`L22`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L22) — Extract title from passenger name.
- `fill_age(row)` — [`L97`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L97)
- `fill_fare(row, df, is_train=True)` — [`L111`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L111)
- `impute_missing_values(train, test)` — [`L89`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L89) — Impute missing values in both datasets.
- `load_data(base_path)` — [`L15`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L15) — Load training and test datasets.
- `main()` — [`L203`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L203)
- `select_features(df)` — [`L148`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L148) — Select features for model training.
- `train_model(X_train, y_train)` — [`L160`](../../../../../../../raw/code/openrsi/OpenMLE-Gym/builder_core/samples/sample_solution.py#L160) — Train ensemble model with cross-validation.

