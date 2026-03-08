# Developer Job Satisfaction Analysis — StackOverflow 2025 Survey

![Python](https://img.shields.io/badge/Python-3.10-blue) ![Scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange) ![License](https://img.shields.io/badge/license-MIT-green)

## Motivation

With AI rapidly reshaping the software industry, understanding what drives developer job satisfaction has never been more relevant. This project analyzes the 2025 StackOverflow Developer Survey to explore whether AI attitudes, usage habits, and traditional career factors like salary and experience can predict how satisfied a developer feels at work.

## Questions of Interest

1. Do developers who actively use AI tools report higher job satisfaction?
2. Which AI-related behaviors and attitudes are the strongest predictors of job satisfaction?
3. Can we build a classification model to reliably predict whether a developer has low, medium, or high job satisfaction?

## Repository Contents

| File | Description |
|------|-------------|
| `SurveyAnalysis.ipynb` | Main Jupyter notebook containing all analysis, visualizations, and modeling |
| `survey_results_public.csv` | Raw survey data from StackOverflow 2025|
| `survey_results_schema.csv` | Column descriptions for the survey dataset |
| `README.md` | Project overview and documentation |

## Libraries Used

- `pandas` — data loading, cleaning, and manipulation
- `numpy` — numerical operations
- `matplotlib` & `seaborn` — data visualization
- `scikit-learn` — machine learning (Random Forest, train/test split, evaluation metrics)

## Summary of Results

- **Salary, years of experience, and developer type** are the strongest predictors of job satisfaction — far outweighing AI-related factors
- **Daily AI users report slightly higher satisfaction** (%52.2 High) compared to non-users (%50.7 High), but the difference is modest
- **AIThreat is the most relevant AI feature** (correlation: -0.073), suggesting that fear of AI has a slightly negative association with job satisfaction — though the effect is still weak
- **The classification model achieved 52% accuracy** (vs. 33% random baseline) in predicting Low / Medium / High satisfaction, performing best on High satisfaction cases (F1: 0.61)
- The overall finding: **job satisfaction is complex and personal** — demographics and compensation explain more than AI attitudes do

## Data Source
https://survey.stackoverflow.co/
Download 2025 versions to run the code, no file name is changed. Can't upload csv to Github because of size.

## Acknowledgments: 
StackOverflow for making the survey data publicly available. Udacity Data Science Nanodegree for project guidance.
