# Rain-Prediction-in-Australia_Finished

This notebook focuses on building a **Supervised Machine Learning** model to predict whether it will rain tomorrow in Australia, based on historical weather data. 

### A. OBJECTIVE 
This project aims to predict whether it will rain tomorrow in various locations across Australia based on historical weather observations.

### B. DATASET
i. The dataset is publicly available from Kaggle (https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package) and contains various meteorological features such as temperature, humidity, wind, and rainfall.

ii. The raw CSV file has been stored in this repository and loaded via GitHub’s raw URL: https://raw.githubusercontent.com/yohaneskh/Rain-Prediction-in-Australia_Finished/refs/heads/main/weatherAUS.csv.

### C. Project Workflow
1. Import Libraries.
- Loaded essential packages including pandas, numpy, matplotlib, seaborn, sklearn, xgboost, and category_encoders.

2. Install category_encoders (if needed).
- !pip install category_encoders.
- Used to encode categorical variables like RainToday, WindDir9am, and WindGustDir.

3. Load & Explore Dataset.
- Displayed data shape and column types.
- Checked missing values, target class balance, and correlations.

4. Data Cleaning
- Handled missing values by doing imputation using mode and median values, or dropping those with few missing values.

5. Feature Encoding
- Used category_encoders to convert categorical features into numeric values suitable for modeling.

6. Feature Selection
- Selected relevant columns and chose RainTomorrow as the binary target.

7. Train-Test Split
- Split data into 80% training and 20% testing using train_test_split from scikit-learn.

8. Model Training
- Train using Logistic Regression method.

9. Model Evaluation
