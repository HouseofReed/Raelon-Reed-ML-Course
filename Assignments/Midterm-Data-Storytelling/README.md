# Midterm Project – Data Storytelling

## Project Overview

The goal of this project was to complete an end-to-end machine learning investigation using the Titanic dataset. I used the machine learning workflow to explore and prepare the data, train classification models, evaluate their performance, and interpret what the results revealed about passenger survival.

## Problem

The main problem was to predict whether a passenger survived the Titanic disaster based on available passenger information.

The target variable was `Survived`, where:

- 0 represented a passenger who did not survive
- 1 represented a passenger who survived

## Exploratory Data Analysis

I used exploratory data analysis to identify patterns that could potentially help predict passenger survival.

Two of the relationships I examined were:

- Survival based on gender
- Survival based on passenger class

My analysis showed that female passengers had a much higher survival rate than male passengers. I also found that passengers traveling in first class had better survival outcomes, while third-class passengers experienced a higher number of deaths.

Based on these results, I hypothesized that gender and passenger class would be important features for predicting survival.

## Data Preparation

Before training the models, I prepared the dataset for machine learning.

Some of the preprocessing steps included:

- Identifying missing values
- Filling missing `Age` values using the median
- Encoding categorical variables
- Converting passenger information into numerical features that could be used by the models
- Splitting the dataset into training and testing sets

I used the median for missing age values because it is less affected by extreme values than the mean and allowed me to keep passenger records that would otherwise have been removed.

## Models

I trained and compared two classification models:

1. Logistic Regression
2. Decision Tree Classifier

Logistic Regression was used as the baseline model, and the Decision Tree was trained as the second model for comparison.

## Results

The models produced the following test accuracy:

- **Logistic Regression: 81.01%**
- **Decision Tree: 74.86%**

The Logistic Regression model performed approximately 6% better than the Decision Tree and demonstrated better generalization to the test data.

For the Decision Tree's positive survival class:

- **Precision: 0.69**
- **Recall: 0.70**

A precision of 0.69 means that when the Decision Tree predicted that a passenger survived, approximately 69% of those predictions were correct. A recall of 0.70 means that the model correctly identified approximately 70% of the passengers who actually survived.

## Key Findings

One of the most important findings from this project was the strong relationship between survival, gender, and passenger class. Female passengers and passengers traveling in first class appeared to have significantly higher survival rates.

The project also demonstrated that a more complex model does not automatically produce better results. In this case, Logistic Regression performed better than the Decision Tree on unseen test data.

## What I Learned

This project helped me understand how the different stages of machine learning connect together. Instead of focusing only on training a model, I worked through the complete process of exploring data, preparing features, training models, evaluating results, and interpreting model performance.

I also learned why accuracy alone does not tell the complete story of a model's performance. Metrics such as precision, recall, classification reports, and confusion matrices provide additional information about the types of predictions and errors a model makes.

## Future Improvements

If I continued this project, I would test additional machine learning algorithms such as Random Forest or Gradient Boosting. I would also explore additional feature engineering, including variables such as family size, to determine whether they could improve predictive performance.

## Files

- `MT_RaelonReed_ITAI1371.ipynb` – Completed Jupyter Notebook containing the analysis, visualizations, preprocessing, models, evaluation, and conclusions.
