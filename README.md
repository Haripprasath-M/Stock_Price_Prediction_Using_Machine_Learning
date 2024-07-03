# Stock_Price_Prediction_Using_Machine_Learning
### Introduction
This project focuses on predicting stock prices for Infosys using various machine learning techniques. The goal is to develop accurate models that can forecast future stock prices based on historical data. This analysis involves data preprocessing, exploratory data analysis, model building, and hyperparameter tuning.

### Steps Taken
1. Importing Libraries and Data
  - Libraries: Necessary Python libraries such as NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, and more were imported.
  - Data: Loaded historical stock price data for Infosys using Pandas and displayed the first few rows to understand its structure.
2. Data Preprocessing
  - Column Standardization: Converted all column names to lowercase to maintain consistency.
  - Handling Missing Values: Checked for and handled missing values in the dataset to ensure clean data for analysis.
3. Feature Engineering
  - Technical Indicators: Added technical indicators such as Moving Averages, Bollinger Bands, RSI, and MACD to enrich the dataset.
  - Lagged Features: Created lagged features to incorporate historical price information into the model.
4. Model Building and Evaluation
  - Baseline Models: Implemented baseline models including Linear Regression, Random Forest Regressor, Gradient Boosting Regressor, and Support Vector Regression (SVR).
  - Linear Regression Baseline Results:
    - Mean Squared Error: 713.937
    - R-squared Score: 0.8988
    - Mean Absolute Error: 18.7406
  - Random Forest Regressor Baseline Results:
    - Mean Squared Error: 894.477
    - R-squared Score: 0.8733
    - Mean Absolute Error: 21.3959
  - Gradient Boosting Regressor Baseline Results:
    - Mean Squared Error: 857.082
    - R-squared Score: 0.8786
    - Mean Absolute Error: 20.7869
  - SVR Baseline Results:
    - Mean Squared Error: 22656.637
    - R-squared Score: -2.2103
    - Mean Absolute Error: 135.3713
5. Hyperparameter Tuning
- Random Forest Regressor:
Best Parameters: {'max_depth': 13, 'min_samples_leaf': 1, 'min_samples_split': 15, 'n_estimators': 100}
Results:
  - Mean Squared Error: 870.467
  - R-squared Score: 0.8767
  - Mean Absolute Error: 21.1902
- Gradient Boosting Regressor:
Best Parameters: {'learning_rate': 0.05, 'max_depth': 3, 'n_estimators': 100}
Results:
  - Mean Squared Error: 838.256
  - R-squared Score: 0.8812
  - Mean Absolute Error: 20.5256
- Support Vector Regression (SVR):
Best Parameters: {'C': 1, 'gamma': 'scale', 'kernel': 'linear'}
Results:
  - Mean Squared Error: 702.344
  - R-squared Score: 0.9005
  - Mean Absolute Error: 18.4470
6. Prediction and Final Evaluation
  - Final Model: The Support Vector Regression model with hyperparameter tuning provided the best performance.
  - Performance Metrics: Evaluated predictions using Mean Squared Error, R-squared Score, and Mean Absolute Error.
### Conclusion
This project illustrates a comprehensive approach to stock price prediction using machine learning techniques. Through data preprocessing, exploratory analysis, feature engineering, model building, and hyperparameter tuning, the Support Vector Regression model emerged as the best-performing model. The insights gained and methodologies applied are essential for making informed decisions in stock price prediction.
