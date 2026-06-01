# Semiconductor Quality Prediction - SECOM Dataset

**CV priority:** 06  
**Date:** January 2026  
**Type:** Data Analytics group project  
**Tools:** Python, pandas, NumPy, Matplotlib, scikit-learn  
**Source report:** `DA-Jan26-report-G11T9.pdf`

## Notebook

- [Google Colab notebook](https://colab.research.google.com/drive/1pdQF2ZEdHic0H2TvSEV6ZKdUKqwGmnKN?usp=sharing)

## Project Summary

This project used the SECOM semiconductor manufacturing dataset to classify wafer/process outcomes as Pass or Fail. The task is difficult because the dataset is high-dimensional, contains missing values, and is heavily imbalanced toward Pass samples.

The project compared original-feature models against PCA-reduced feature sets to test whether dimensionality reduction improves quality prediction.

## Dataset and Preprocessing

| Item | Value |
| --- | --- |
| Samples | 1,566 |
| Raw features | 590 |
| Class distribution | 1,462 Pass, 104 Fail |
| Missing values | 41,907, about 4.54% |
| Cleaned feature count | 442 after high-missing and zero-variance removal |
| Preprocessing | Mean imputation and standardization |

## Model Comparison

| Model/Feature Set | Observation |
| --- | --- |
| Logistic Regression on original features | Best F1-score at 0.192 |
| Decision Tree | Comparable F1-score at 0.183 but lower recall |
| Random Forest | Very low recall, about 0.038 |
| PCA-reduced datasets | Consistently underperformed original features |

The report concluded that PCA removed low-variance signals that were still useful for detecting rare Fail-class cases. A fixed decision threshold of 0.20 was used to improve sensitivity to minority failures.

## What I Learned

- Why class imbalance makes accuracy a misleading metric in manufacturing quality prediction.
- How PCA can reduce dimensionality while also discarding minority-class information.
- How recall, F1-score, and decision-threshold tuning matter more than raw accuracy for rare failure detection.
- How to build a reproducible preprocessing and model-comparison pipeline.

## Recruiter Notes

This project connects semiconductor manufacturing context with practical data analytics. It is especially relevant to yield analytics, process monitoring, test engineering, and manufacturing data science.

## Missing Before Publishing

- Confusion matrices and model-performance plot exports.
- Short note clarifying Adam's personal contribution in the group workflow.
