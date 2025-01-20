# House pricing predictive model, as a first estimator.

Team members: Nikolaos Marakis, Maria Kopsacheili, Apostolis Karapatis

# Introduction
## Subtitle: Empowering a real estate company to make better, faster pricing decisions.

The real estate market is competitive  and accurate pricing is crucial for success. Brokers need a reliable starting point to estimate house prices quickly and effectively. A  machine learning model would be a solution that saves a lot of time, since it can predict a first estimation of each house’s price.

# Objectives

- Data Cleaning: nulls, duplicates, feature engineering for the data to be suitable for the machine learning process.
- Exploratory Data Analysis (EDA): Perform EDA to understand the relationships between our dataset's features and the house price.
- Model Training: Choose and train our model to predict house prices, while trying different techniques in order to find the best parameters and features for our model.
- Model Evaluation: Evaluate the performance of the model using appropriate metrics.

# Technologies used

- Pandas: For data preprocessing and analysis.
- Matplotlib, Seaborn: For data visualizations.
- Scikit-Learn: Develop the machine learning model.

# Steps

## Data

Our dataset was a csv file obtained from Kaggle

## Data Cleaning

Drop out duplicates and nulls, replace categorical features with numerical values (replace, get_dummies)

## EDA

Check relationships between our features and the house price by creating graphs(box plots, scatter plots), correlation matrix, descriptive statistics

## Modeling

- model choise: Random Forest
- scalers: tried different scalers to improve model's performance
- feature selection: feature importances, shap
- drop outliers
- performance: 
Model's R2 score: 0.66, RMSE score: 1035585.94, Mean Absolute Error score: 739382.54, Mean Absolute Error (%): 0.18

** model performance was not close to our goal but this was due to our small dataset (550 row and 13 columns). To make the model even better, we need more detailed data.

Additional data could improve model's performance:
- Neighborhood trends, such as upcoming developments
- Market conditions, like seasonality or demand shifts
- Crime rate
- Kitchen, garden, pool, fireplace, etc.
- Year built
