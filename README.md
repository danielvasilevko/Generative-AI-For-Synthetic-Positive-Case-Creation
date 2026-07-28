# Generative-AI-For-Synthetic-Positive-Case-Creation
This repository contains the final paper and R Markdown file used to analyze advertisement click-through prediction on a severely imbalanced Kaggle dataset (1.5% positive rate), along with an evaluation of synthetic data generation methods (CTGAN, DataSynthesizer, LLM-based generation) as a strategy to address the class imbalance.

# Repository Structure

* Generative-AI.Rmd - R Markdown featuring the modeling and synthetic data generation analysis behind this project.
* Generative-AI_Paper.pdf - A PDF containing the final paper summarizing the methodology, results, and conclusions of the analysis.

# What Analysis.Rmd Does

* Cleans and merges news-feed and advertisement behavior datasets on a shared user ID.
* Trains baseline click-through prediction models (logistic regression, lasso regularization, neural network, LightGBM) and evaluates them using F1 score.
* Generates synthetic minority-class (positive) observations using CTGAN and DataSynthesizer.
* Compares model performance when synthetic data is added at varying ratios, including original-ratio augmentation, positive-only augmentation, and fully synthetic training sets.
* Visualizes F1 and AUC-ROC scores across synthetic data conditions to assess whether augmentation improves predictive performance.

