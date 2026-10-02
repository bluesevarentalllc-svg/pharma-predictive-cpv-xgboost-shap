# Release Notes — V1.0.0

**Release date:** October 1, 2026

## Predictive CPV Analytics for Tablet Compression

V1.0.0 freezes the first public-ready version of the XGBoost + SHAP predictive CPV proof-of-concept.

### Included in this release

- 720-batch synthetic tablet-compression dataset across 18 API lots.
- Lot-aware model-development split:
  - 400 training batches / 10 lots
  - 120 validation batches / 3 unseen lots
  - 120 independent test batches / 3 unseen lots
  - 80 deliberately out-of-domain stress batches / 2 lots
- Linear Regression and Random Forest baselines.
- Tuned XGBoost regression with API-lot-aware grouped cross-validation.
- Independent unseen-lot test evaluation.
- SHAP global feature importance.
- SHAP batch-level explanation example.
- Bootstrap assessment of SHAP importance stability.
- Standardized nearest-neighbor applicability-domain control.
- Deliberate OOD stress testing.
- Project report and public-release metadata.

### Key V1.0 synthetic results

Independent unseen-lot test set, N = 120:

- Tuned XGBoost MAE: **0.602**
- Tuned XGBoost RMSE: **0.740**
- Tuned XGBoost R²: **0.646**

Applicability-domain behavior:

- Normal unseen-lot test: **13/120 flagged OOD (10.8%)**
- Deliberate stress set: **80/80 flagged OOD (100%)**
- Tuned XGBoost stress-set RMSE: **3.700**
- Tuned XGBoost stress-set R²: **-2.467**

### Scope and limitations

This is a **synthetic proof of concept**. It is not a validated GMP model and should not be used for batch release, batch disposition, autonomous process adjustment, or replacement of laboratory testing. SHAP values explain model behavior; they do not prove mechanistic causality.

### Citation

A version-specific DOI should be added after the V1.0 GitHub release is archived by Zenodo.
