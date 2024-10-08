#Poverty Rates Across United States

Overview:
This project focuses on predicting poverty levels across counties using a combination of multiple linear regression and logistic regression models. The analysis is based on publicly available poverty data and socioeconomic factors such as education level, household income, unemployment rate, and metro status. The goal is to identify significant predictors of poverty and create models that can reliably predict poverty levels using these variables.

Key Features:
Tech Stack: The project is implemented using R.
Data Sources: UN and US Census data are used for poverty rates, income levels, and other socioeconomic indicators.
Machine Learning Models:
1. Multiple Linear Regression: Five models with increasing complexity were built to predict the poverty rate using variables such as:
Median education level
Median household income
Unemployment rate
Metro area status
Per capita income
2. Logistic Regression: Predicts poverty or wealth classification based on a threshold derived from poverty rates. The model output is categorical, distinguishing between high and low poverty rates.

Techniques Used:
Multiple Linear Regression with Interaction Terms: We started with a simple baseline model and progressively added more variables to improve performance.
Model Performance Metrics: Adjusted R-squared values and Mean Squared Error (MSE) were used to evaluate model performance.
Final Model: The final model accounts for about 72.89% of the variance in poverty levels, with an adjusted R-squared of 0.7281 and an MSE of 0.047.
Logistic Regression for Classification:
Confusion Matrix: Used to evaluate classification performance. The model achieved an accuracy of 82.42%.
Threshold Analysis: Various probability thresholds were tested to optimize classification accuracy, with a threshold of 0.6 yielding the best results.

Model Performance:
1. Multiple Linear Regression:
    Best Model (Model 5):
    Adjusted R-squared: 0.7281
    MSE: 0.047
    Significant Predictors:
    Median education (below high school, high school diploma, some college)
    Median household income
    Unemployment rate
    Metro area status
    Per capita income
2. Logistic Regression:
    Accuracy: 82.42%
    Confusion Matrix:
    True Negatives (TN): 229
    True Positives (TP): 193
    False Negatives (FN): 59
    False Positives (FP): 31
   
The multiple linear regression models progressively improved in explanatory power with the addition of socioeconomic factors.
The logistic regression model demonstrated strong classification capabilities, with an optimal threshold of 0.6 for the best accuracy.

Visualizations: 
Residuals vs Fitted Plot: Showed no clear pattern, indicating the assumptions of linearity were met.
QQ Plot: Confirmed that the residuals followed a normal distribution.
Accuracy vs Probability Threshold Graph: Showed that higher probability thresholds led to more conservative, but accurate, predictions.
