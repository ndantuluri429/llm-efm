# llm-efm

This repository contains the anonymized code and materials associated with our TS4H Workshop (NeurIPS 2025) submission:
“Establishing Large Language Model Baselines for Physiological Time Series: Insights from Intrapartum Electronic Fetal Monitoring.”

## Repository Structure:
### /prompts
Prompt templates used for zero-shot large language model (LLM) analysis of electronic fetal monitoring (EFM) time series.

### /analysis
Scripts and notebooks for:
Manual calculation of EFM time-series metrics (baseline FHR, variability, accelerations, decelerations, UC frequency).
Comparative evaluation of model, expert, and ground-truth performance.

### /evaluation
Code for computing regression and classification metrics, including RMSE, MAE, bias, balanced accuracy, F1, and $R^2$.

### /interpretation_only
Implementation of the “interpretation-only” configuration.
In this setting, LLMs are provided precomputed, structured summaries of CTG metrics instead of raw signals.
Models apply FIGO guideline criteria to these summaries to generate floating-point pH estimates.
Performance is quantified against ground truth using RMSE, MAE, bias, and $R^2$.

## Data
- Data is drawn from the CTU-UHB intrapartum cardiotocography database (PhysioNet).
- All identifiers have been removed to maintain anonymity.
- Replication requires access to the dataset under its original license.

## Notes
- This repository is anonymized for peer review.
- All reported results match those described in the submitted manuscript.
