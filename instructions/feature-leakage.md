---
id: feature-leakage
title: Feature Leakage
summary: Check wether there is evidence of feature leakage in the study design or reporting.
defaultSelected: true
---

# Feature Leakage

## What to check

- Whether test set information was used during feature selection.
- Whether future information was used to select features.
- Whether feature was actually highly confounded with endpoint, and not a true predictor.

## Red flags

- Differential abundance analysis was performed on the full dataset to select features, then evaluated machine models on subset of full dataset.
- Select features based samples' future status but still put these samples in test set and report performance.
- Endpoint is something like "diagnosis" but the top features are things like "CSF Aβ42" that are known to be highly confounded with diagnosis and not true predictors.
