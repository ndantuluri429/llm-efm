# llm-efm

This repository contains the anonymized code and materials associated with our TS4H Workshop (NeurIPS 2025) submission:
“Establishing Large Language Model Baselines for Physiological Time Series: Insights from Intrapartum Electronic Fetal Monitoring.”

Contents
LLM Prompting Framework:
Prompt templates used for generating analyses with large language models (/prompts).

Raw Analysis & Manual Metrics:
Scripts and notebooks for manual calculation of time-series features (baseline heart rate, variability, accelerations, decelerations) and evaluation metrics (/analysis).

Performance Evaluation:
Code for computing RMSE, MAE, bias, and $R^2$ against ground-truth physiological outcomes (/evaluation).

Interpretation-Only Configuration:
In this setting, LLMs are provided with pre-computed, summarized time-series metrics rather than raw tracings. The models apply FIGO guideline criteria to structured inputs to estimate fetal pH values. Performance is again assessed via RMSE, MAE, bias, and $R^2$ (/interpretation_only).
