# Group 4D — Predicting Invoice Payment Risk

**Dataset:** `invoice_payment_risk.csv`

**Context:** Assessing how likely a B2B client is to pay an invoice late

**Target variable:** `payment_risk_category` — 3 classes: **On-Time / Late / Severely Late**


## Overview

This repository contains Group 4D's classification analysis notebook, applying the
full modeling pipeline covered in class — from dependency installation through
model persistence — to our assigned invoice payment risk dataset.

All decisions (missingness handling, feature selection, resampling, encoding,
diagnostics) are made specifically for this dataset's actual properties, not
copied from the in-class demonstration notebook. In particular, `payment_risk_category`
is imbalanced (Severely Late is the minority class), which shapes our approach to
stratified splitting, cross-validation, and resampling throughout.

## Team

| Name | Section(s) | GitHub Handle |
|------|-----------|----------------|
| TBD  | TBD       | TBD            |
| TBD  | TBD       | TBD            |
| TBD  | TBD       | TBD            |
| TBD  | TBD       | TBD            |
| TBD  | TBD       | TBD            |

*(Table to be filled in once section assignments are finalized via team poll.)*


## Notebook Sections

1. Setup & Dependencies
2. Data Loading & Exploratory Data Analysis
3. Train/Test Split (stratified on `payment_risk_category`)
4. Feature Selection
5. Preprocessing Pipeline (incl. imbalance-safe resampling, scoped to training fold only)
6. Modeling & Cross-Validation (stratified k-fold)
7. Diagnostics (confusion matrix, ROC, precision-recall curve — minority class discussed explicitly)
8. Evaluation of Candidate Models (macro/weighted metrics on held-out test set)
9. Hyperparameter Tuning
10. Explainability
11. Model Persistence (full pipeline; explicit note that the resampler does not act at inference time)
12. Conclusion & Limitations

## Branching Workflow

- `main` — stable, reviewed content only
- `feature/<section>-<name>` — one branch per person per section
- Open a pull request into `main` when your section is complete
