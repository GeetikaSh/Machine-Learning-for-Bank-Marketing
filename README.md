# Machine Learning for Bank Marketing

A concise, reproducible comparative analysis of machine learning models applied to a bank telemarketing dataset. The goal is to identify which models and preprocessing approaches produce the best predictive performance for campaign success and to provide clear guidance for practitioners in financial marketing.

## Objectives
- Load and clean the bank marketing dataset.
- Evaluate multiple models (baseline and more advanced) across consistent metrics.
- Present model selection guidance and reproducible notebooks/scripts to accelerate similar projects.

## Dataset
Source: Kaggle — "Bank Marketing Dataset" (Moro et al., 2014)  
Link: https://www.kaggle.com/datasets/janiobachmann/bank-marketing-dataset

Citation: S. Moro, P. Cortez and P. Rita. "A Data-Driven Approach to Predict the Success of Bank Telemarketing." Decision Support Systems, 62:22–31, 2014.

## Reproducibility
- All preprocessing and model training steps are implemented in notebooks and scripts with fixed random seeds where applicable.
- Configurable parameters are kept near the top of notebooks/scripts so experiments can be reproduced or extended.

## Findings (summary)
This repository implements several models (e.g., tree-based ensembles, gradient boosting) and compares them using standard classification metrics (accuracy, precision, recall, F1, ROC-AUC). See reports/ and notebooks/ for detailed results and visualizations.
- Decision Tree: Accuracy->68%

## Code Structure
```cpp
banking-marketing-model/
│
├── data/
│   └── (optional sample CSV)
│
├── notebooks/
│   └── model_training.ipynb
│
├── src/
│   ├── data_preprocessing.py
│   ├── model_train.py
│   ├── inference.py
│   └── utils.py
│
├── models/
│   └── decision_tree_pruned.pkl
│
├── api/
│   └── app.py  (FastAPI)
│
├── tests/
│   └── test_api.py
│
├── requirements.txt
├── README.md
└── .github/
    └── workflows/
        └── ci-cd.yml
```
