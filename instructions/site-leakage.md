---
id: site-leakage
title: Site Leakage
summary: Check whether there is evidence of site leakage in the study design or reporting.
defaultSelected: true
---

# Site Leakage

## What to check

- Whether test site have been already used for model selection or hyperparameter tuning.
- Whether harmonization is performed across sites, and if so, whether it is performed separately for training and test sets.

## Red flags

- Statistical harmonization (e.g., ComBat) is performed across all sites without separating training and test sets.
- No mention of whether test sites were used for model selection or hyperparameter tuning.
