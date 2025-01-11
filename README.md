# Life-Expectancy-Prediction-2000-to-2015-
Data Intensive Computing Project ( cleaning, Preprocessing, Modeling)


## Life Expectancy Analysis and Prediction (2000–2015)

## Overview
This project analyzes global life expectancy trends from 2000 to 2015, using health, demographic, and economic data from a Kaggle dataset. The primary goal is to identify key factors influencing life expectancy and build predictive models to estimate it. By highlighting disparities between developed and developing countries, this project provides insights into improving global health outcomes.

## Dataset
The dataset contains 2,938 records across 22 attributes, with variables such as:
Life Expectancy: Target variable indicating the average lifespan.
Adult Mortality: Number of adult deaths per 1,000 people, inversely related to life expectancy.
Schooling: Average years of education per individual, positively correlated with life expectancy.
HIV/AIDS: Disease-related deaths, negatively impacting life expectancy.
Income Composition of Resources: Reflecting economic development.
BMI: Average Body Mass Index as an indicator of nutritional health.
The dataset underwent significant preprocessing to handle missing values, remove duplicates, and standardize columns.

## Methodology

### Data Preprocessing:

Removed columns with >30% missing values (e.g., Hepatitis B, GDP, Population).
Imputed missing data using median values.
Standardized column names and converted categorical variables into numerical values.
Addressed inconsistencies in data (e.g., country names) using regular expressions.
Exploratory Data Analysis (EDA):

Analyzed correlations between variables and life expectancy.
Visualized patterns using histograms, scatter plots, box plots, and violin plots.
Highlighted disparities between developed and developing countries in healthcare access, education, and mortality rates.

### Key findings included:
A strong negative correlation between adult mortality and life expectancy.
Positive correlations with schooling, income composition, and immunization rates.
Limited impact of alcohol consumption on life expectancy globally.
### Predictive Modeling:
Target Variable: Life Expectancy.
Models used:
Linear Regression: R² = 0.88, MSE = 9.99.
Random Forest: R² = 0.97, MSE = 2.22 (Best performance).
Gradient Boosting: R² = 0.96, MSE = 3.49.
Lasso Regression: Effective for feature selection but less predictive.
K-Nearest Neighbors (KNN): Moderate accuracy with R² = 0.89.
Decision Tree: Good interpretability but prone to overfitting.
Performance Metrics: R², Mean Squared Error (MSE), and Mean Absolute Error (MAE).

## Key Insights:

Ensemble models (Random Forest and Gradient Boosting) consistently outperformed linear and simpler models.
Education, healthcare, and income composition significantly influence life expectancy.
Immunization campaigns (e.g., polio vaccination) have a measurable positive impact.
## Results
The Random Forest model provided the best results with an R² of 0.97, demonstrating its ability to capture both linear and non-linear relationships.
The analysis emphasized the importance of addressing disparities in healthcare access, education, and economic resources to improve life expectancy, particularly in developing countries.
## Visualizations
### Key visualizations include:

Correlation heatmaps.
Distribution of life expectancy across countries.
Comparison of mortality rates between developed and developing nations.
Feature importance plots from ensemble models.
Future Work
Incorporate additional datasets (e.g., recent healthcare advancements or economic indicators).
Explore deep learning models to capture more complex patterns.
Regional analysis to account for geographical variations in life expectancy.
Tools & Technologies
Programming Languages: Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn).
Libraries: Scikit-learn for modeling, Seaborn for advanced visualization.
Data Source: Life Expectancy Data on Kaggle
