---
id: model-leakage
title: Model Leakage
summary: Check whether there is evidence of model leakage in the study design or reporting.
defaultSelected: true
---

## What to check

- Whether model tune or preprcessing step is performed on the test set.
- Whether multiple iterations of model tune are performed on the test set (e.g. multiple rounds of hyperparameter tuning or model selection).

## Red flags

- Model tune is performed on the test set.
- Normalization or missing data imputation was done on the whole sample instead of on training samples.
- Multiple iterations of model tune are performed on the test set (e.g. multiple rounds of hyperparameter tuning or model selection).
- The test set is NOT held out until the final evaluation of the model.
