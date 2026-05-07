---
id: split-leakage
title: Split Leakage
summary: Check whether there is evidence of split leakage in the study design or reporting.
defaultSelected: true
---

## What to check

- Whether no proper train/validation/test split was performed.
- whether no proper nested cross-validation was performed.
- Whether no controls for split for longitudinal data were performed (e.g. all samples from a given subject are in the same split).

## Red flags

- No mention of train/validation/test split or cross-validation in the methods.
- Test set samples were used for model selection or hyperparameter tuning.
- For K-fold cross-validation, no mention of nested cross-validation for model selection or hyperparameter tuning.
- No mention of controlling for longitudinal data leakage risks in the methods.
