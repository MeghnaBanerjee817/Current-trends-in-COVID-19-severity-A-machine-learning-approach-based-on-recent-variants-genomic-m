## Overview

This repository contains machine learning and genomic analysis workflows for predicting COVID-19 severity using recently circulating SARS-CoV-2 variants, nucleotide-level mutations, and patient metadata derived from GISAID.

The study integrates demographic variables, viral genomic mutations, lineage/clade information, and geographic metadata to construct interpretable severity prediction models using multiple machine learning algorithms, including Logistic Regession with Elastic Net, Random Forest, LightGBM, XGBoost, and GPBoost mixed-effects models.

The models were evaluated using statistical robustness analysis, temporal validation, leave-one-country-out cross-validation (LOOCV), and decision curve analysis to assess predictive performance and clinical utility of the best performing models.

SHAP (SHapley Additive exPlanations) was applied to identify important genomic and demographic predictors associated with severe COVID-19 outcomes. 

The repository also includes an extendable Python-based prototype pipeline capable of incorporating updated datasets and future clinical covariates for dynamic model updating and severity prediction.

## Machine Learning Models used

The following models were evaluated:

- Logistic Regression with Elastic Net Regularization 
- Random Forest
- XGBoost
- LightGBM
- GPBoost
- GPBoost (Mixed-effects)
Each if the models were tested under two scenarios i.e with and without country and region metadata except for GPBoost (Mixed effects) model where country and region have been included as random effect variables.


## Dataset

The study uses SARS-CoV-2 metadata and genomic sequences obtained from GISAID.

Due to GISAID data-sharing policies, raw sequence data are not redistributed in this repository.

## Author

Meghna Banerjee
