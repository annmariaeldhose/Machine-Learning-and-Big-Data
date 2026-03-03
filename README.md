SUSY Big Data Machine Learning Pipeline


Overview

This project implements a large-scale machine learning pipeline on the SUSY dataset from the UCI Machine Learning Repository. The objective is to classify supersymmetric signal events using distributed PySpark MLlib and compare results with a single-node scikit-learn baseline.

The workflow includes data ingestion, preprocessing, model training, cross-validation, scalability analysis, and Tableau visualization.

Dataset

5,000,000 rows

19 columns (18 features + 1 binary label)

~2.4GB uncompressed

Binary classification problem

Technologies

Python

PySpark (Spark MLlib)

scikit-learn

NumPy

Tableau Public

Models Implemented

PySpark MLlib:
Logistic Regression, Decision Tree, Random Forest, GBT

Scikit-learn:
Logistic Regression, Decision Tree, Random Forest, KNN


Outputs

Model evaluation metrics

Feature importance comparison

Strong & weak scaling analysis

4 interactive Tableau dashboards


Repository Structure
project/
├── notebooks/
│   ├── 1_data_ingestion.ipynb
│   ├── 2_feature_engineering.ipynb
│   ├── 3_model_training.ipynb
│   └── 4_evaluation.ipynb
├── scripts/
│   ├── run_pipeline.py
│   └── performance_profiler.py
├── config/
│   └── spark_config.yaml
├── tableau/
│   └── tableau_all_dashboards.xlsx
├── data/
│   ├── schemas/
│   └── samples/
├── environment.yml
├── Dockerfile
└── README.md
