# 🎧 Podcast Listening Time Prediction

An XGBoost regression model designed to predict podcast listening time (in minutes) based on episode metadata. This repository contains my late submission for the [Kaggle Playground Series - Season 5, Episode 4](https://www.kaggle.com/competitions/playground-series-s5e4).

## 📌 Project Overview

The goal of this project is to accurately estimate how long users will listen to a podcast given various features such as the episode's genre, host popularity, number of ads, and publication time. The core of this solution relies on an optimized **XGBoost** model trained using robust cross-validation techniques to prevent overfitting and ensure generalizability.

## 📂 Repository Contents

* `submission.ipynb`: The main Jupyter Notebook containing the entire pipeline, from Exploratory Data Analysis (EDA) and data preprocessing to model training, evaluation, and generating the final submission file.

## ⚙️ Methodology

1.  **Data Preprocessing:**
    * Handling missing values in features like `Episode_Length_minutes` and `Guest_Popularity_percentage`.
    * Encoding categorical variables (e.g., `Genre`, `Publication_Day`, `Episode_Sentiment`).
2.  **Model Architecture:**
    * **Algorithm:** Gradient Boosted Trees via `XGBoost`.
    * **Validation Strategy:** K-Fold Cross-Validation to validate performance against the target variable (`Listening_Time_minutes`).
3.  **Evaluation Metric:**
    * The model is evaluated based on **Root Mean Squared Error (RMSE)**, which is the standard evaluation metric for this specific Kaggle competition.
