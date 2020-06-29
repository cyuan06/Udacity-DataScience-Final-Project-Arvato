# Capstone Project:
Create a Customer Segmentation Report for Arvato Financial Services

Udacity Data Scientist Nanodegree capstone project to create Customer Segmentation for Arvato Financial Services

## Table of Contents

- [Project Overview](#projectoverview)
- [Technical Overview](#technicaloverview)



------

<a id='projectoverview'></a>

## 1. Project Overview

In this project, we are provided with demographic data of customers of a mail-order company in Germany and demographic data of general population of Germany. Using this data, we are required to identify new customers for the company.

We approach this project in 2 phases:

- Use Unsupervised Learning to perform customer segmentation and identify clusters/segments from general population who best match mail-order company's customer base.
- Use Supervised Learning to identify targets for marketing campaign of the mail-order company who could possibly become their customers.

Goal of this project is to predict individuals who are most likely to become customers for a mail-order sales company in Germany.

Model:
1. For unsupervised learning, I use PCA and Kmeans.
2. For supervised learning, I use Xgboost and RandomForest as a votingregressor.

Metrics:
1. Use calinski_harabz score, inertia score and davies_bouldin score to evaluate and assess the best cluster number of Kmeans.
2. Use ROC-AUC score to evaluate the VotingRegressor Model for the reason that the data is quite imbalanced.

<a id='technicaloverview'></a>

## 2. Technical overview:

Step by step workflow from data exploration, processing to inference is approached in a structured fashion. Because of the large volume of source data, we build preprocessing pipeline  to get rid of unnecessary and outlier data and implement Dimensionality Reduction and Clustering to identify segments. Due to the nature of the data (details in notebook), AUC/ROC is used as the evaluation metric for this project. Prediction for test set is to be submitted to Kaggle competition for evaluation.

Following concepts implemented and covered in detail in the notebook: 

- Data Exploration & Cleansing
- Dimensionality Reduction
- Clustering
- Supervised Learning
- Final Model Evaluation
- Feature Importance
- Analysis of Model and Algorithmn
- Scoring and submisstion to Kaggle



