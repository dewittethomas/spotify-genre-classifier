# Spotify Genre Classifier

## Overview

This project explores a dataset containing over 2 million Spotify tracks, with features such as danceability, energy, acousticness, loudness, and tempo. The goal is to investigate the dataset and develop machine learning models that predict a track's genre from its features.

The project is part of a machine learning assignment and emphasizes sound data analysis, model validation, and critical evaluation of results.

## Dataset
The dataset contains over 2 million records, each containing information about a single
song. For each song, we have attributes such as the title, artist, release date, a genre
label and several audio features such as “danceability” and “tempo”.

You can download the data [here](https://cloud.ilabt.imec.be/index.php/s/Lmp6WZJtpjXiqMY).

External data is not used, in accordance with the assignment requirements.

## Objectives

- Perform exploratory data analysis to understand the dataset and identify potential issues.

- Clean and preprocess the data where necessary.

- Split the data into training, validation, and test sets, and apply cross-validation.

- Train at least three classifiers from different model families.

- Perform hyperparameter tuning to search for suitable model configurations.

- Compare model performance using appropriate evaluation metrics.

- Generate and discuss visualizations, including confusion matrices.

- Identify the most useful features and retrain the best-performing model using only those features.

- Analyze the results both quantitatively and qualitatively.

## Results

The optimized CatBoost model achieved the best overall performance among the evaluated classifiers.

| Model | Accuracy | Macro-F1 |
|---|---:|---:|
| Logistic Regression | 0.50 | 0.5345 |
| Decision Tree | 0.46 | 0.4683 |
| **CatBoost** | **0.58** | **0.6200** |

Accuracy measures the overall proportion of correct predictions, while macro-F1 gives equal weight to each class, making it particularly useful for evaluating performance on an imbalanced dataset.

Hyperparameter optimization yielded modest improvements for CatBoost and the Decision Tree, while Logistic Regression showed virtually no improvement over its baseline.

## Status

**Completed.**