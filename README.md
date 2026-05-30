# Cinema Audience Forecasting

An end-to-end Machine Learning project developed for the **Machine Learning Practice (MLP)** course of the **IIT Madras BS Degree in Data Science and Applications**.

This project was built for an academic Kaggle competition. Since the competition has been made private by the course authorities, this repository serves as an archive of the complete solution and workflow.

## 📌 Overview

The goal of this project is to predict daily cinema audience counts (`audience_count`) using data from online ticket booking platforms and offline POS systems.

## 📂 Data Sources

* BookNow booking records
* CinePOS booking records
* Theater mapping data
* Calendar and date information

## 🛠️ Pipeline

* Data cleaning and imputation
* Outlier handling
* Feature engineering
* One-hot encoding
* Feature selection (`SelectKBest`)
* Dimensionality reduction (`TruncatedSVD`)
* Model training and evaluation

## 🤖 Models Evaluated

* LinearSVR
* Decision Tree Regressor
* Gradient Boosting Regressor
* LightGBM
* ARIMA

## 📊 Evaluation Metrics

* R² Score
* MAE
* RMSE

## ⚠️ Notebook Access

The notebook preview is currently not opening on GitHub due to persistent `nbformat/nbconvert` rendering issues.

[Google Colab Notebook](https://colab.research.google.com/drive/1voPeXKY1Bs20k0JyaCmXpDcXhNqfUTYO?usp=sharing)

The Colab notebook contains the complete implementation and experiments.

## 🎓 Academic Note

This repository was created as part of the **Machine Learning Practice (MLP)** course under the **IIT Madras BS Degree in Data Science and Applications** program.

