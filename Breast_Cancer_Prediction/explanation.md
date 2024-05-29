**Stock Market Prediction with LightGBM**

This repository contains code for a Light Gradient Boosting Machine (LGBM) model that predicts stock market performance using historical data. The code performs the following steps:

* **Data Loading:** Loads historical stock data from CSV files.
* **Preprocessing:**
    * Removes rows with missing values in the target variable ("TARGET").
    * Calculates new features like 20-day price change and Relative Strength Index (RSI).
    * Splits the training data into training and validation sets.
* **Model Training:**
    * Trains an LGBM model to predict stock price movement (up or down) based on various features.
    * Analyzes feature importance to identify the most influential factors for prediction.
* **Evaluation:**
    * Evaluates the model's performance on the validation set using mean absolute error.
    * Calculates precision, a metric for measuring the proportion of correctly predicted positive outcomes.
    * Considers the class imbalance in the data (more non-movements than movements) and analyzes the improvement in precision compared to a random guess.
    * Generates a classification report to get a more detailed view of the model's performance.
* **Profitability Analysis:**
    * Calculates the average return on investment (ROI) for the entire test set (unfiltered).
    * Calculates the average ROI based on the model's predictions (considering only stocks predicted to go up).
    * Analyzes the average ROI for stocks that actually went up in the training data (represents the solution set).

**Note:**

* This code is specifically designed for the provided stock market prediction dataset.
* The model uses LightGBM, a machine learning algorithm known for its efficiency and accuracy in various tasks.

**Getting Started:**

1. Ensure you have Python and the required libraries (pandas, matplotlib, lightgbm, etc.) installed.
2. Download the stock market dataset and place it in the same directory as this code.
3. Run the Jupyter Notebook file to execute the code.

This code provides a basic framework for stock market prediction using LGBM. You can experiment with different features, hyperparameter tuning, and model selection techniques to potentially improve the model's performance.
