# Zenodo Metadata — V1.0

## Recommended record type
**Software**

## Title
**Predictive CPV Analytics for Tablet Compression: XGBoost Prediction, SHAP Explainability, and Applicability-Domain Control**

## Creator
**Chakrapani, Sri Harsha**

Add your ORCID before publication if you want the Zenodo record linked to your researcher identity.

## Version
**1.0.0**

## Publication date
**2026-10-01**

## Description

This software package presents a synthetic proof-of-concept for predictive continued process verification (CPV) analytics in tablet compression. The workflow extends retrospective process monitoring into explainable predictive decision support by combining lot-aware model development, baseline comparison, tuned XGBoost regression, SHAP explainability, and an applicability-domain control.

A synthetic dataset of 720 tablet-compression batches across 18 API lots is divided by lot into 400 training batches, 120 validation batches from unseen lots, 120 independent test batches from unseen lots, and 80 deliberately out-of-domain stress batches. API lot identity is used for grouping rather than as a model predictor.

On the independent unseen-lot synthetic test set, the tuned XGBoost model achieved MAE 0.602 percentage points, RMSE 0.740 percentage points, and R² 0.646. SHAP is used to explain global and batch-level model behavior without treating feature importance as proof of causality. A standardized nearest-neighbor applicability-domain check flagged 13 of 120 observations in the normal unseen-lot test set and all 80 deliberately out-of-domain stress observations.

The package is designed to demonstrate a controlled manufacturing-analytics workflow: optimize for unseen groups, explain predictions, identify conditions where predictions should not be trusted, and preserve human engineering judgment.

**Important limitation:** all data are synthetic. No proprietary manufacturing data are included. The model is not validated for GMP release, batch disposition, autonomous process control, replacement of dissolution testing, or other regulated operational use.

## Keywords
- Continued Process Verification
- CPV
- Pharmaceutical Manufacturing
- Tablet Compression
- Predictive Analytics
- XGBoost
- SHAP
- Explainable AI
- Machine Learning
- Process Validation
- Applicability Domain
- Model Governance
- OSD Manufacturing

## Language
English

## Access
Recommended: **Open access**, if you are comfortable making the complete synthetic package public.

## License
**Select before publication.** This release kit intentionally does not make the legal choice for you. See `LICENSE_SELECTION.md`.

## Related identifiers
After the GitHub repository is public, add the GitHub repository URL as the related software/source-code identifier if Zenodo does not populate it automatically.

## Notes for the Zenodo release
- Upload/archive the exact GitHub V1.0 release.
- Verify author spelling before publishing.
- Add ORCID if desired.
- Confirm the final license.
- After publication, copy the version DOI into the README and `CITATION.cff`.
