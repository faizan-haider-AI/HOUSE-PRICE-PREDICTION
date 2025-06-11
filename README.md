🏠 House Prices - Advanced Regression Techniques
This project is a solution to the Kaggle competition "House Prices - Advanced Regression Techniques". It involves building a regression model to predict the sale prices of houses in Ames, Iowa using various numerical and categorical features.

📌 Problem Statement
Accurately predict house sale prices based on a mix of features such as area, quality, location, and amenities. The goal is to minimize the Root Mean Squared Logarithmic Error (RMSLE) on the test set.

🚀 Final Model Summary
Algorithm: XGBoost Regressor

Target Transformation: np.log1p() to normalize price distribution

Evaluation Metric: RMSLE

Train RMSLE: 0.0057

Validation RMSLE: 0.0103

Final Prediction: np.expm1() used to reverse log transform

🛠️ Key Techniques Used
✅ Data Cleaning: Handled missing values using strategies like median imputation and mode filling

🎨 Feature Engineering: Combined features, label encoding for categoricals, and added log transformations

📊 Modeling:

Used XGBRegressor with tuned hyperparameters

Early stopping on validation set to avoid overfitting

🔁 Train/Test Split: Data split into training and validation using train_test_split

📉 Evaluation: Custom function to calculate RMSLE and monitor overfitting

📁 Submission
Predictions were generated on the test dataset and saved in submission.csv following Kaggle format:
Id,SalePrice
1461,123421.02
1462,151557.67


Files Included
train.csv: Original training data

test.csv: Test data for prediction

submission.csv: Final predictions for Kaggle submission

notebook.ipynb: All steps including preprocessing, training, evaluation, and prediction

Result
This solution demonstrates a well-generalized model with minimal overfitting and high accuracy on both training and validation sets.
