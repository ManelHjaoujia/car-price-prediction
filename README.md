# Car Price Prediction using Machine Learning

## Project Overview
This project focuses on predicting the **selling price of used cars** based on their features such as model, year, fuel type, transmission, and seller type.  
The objective is to build and compare different machine learning regression models to find the best-performing algorithm for price prediction.

## Dataset
The dataset used is **CarDekho Dataset**.  
It contains car details such as model, year, mileage, fuel type, transmission type, and seller information.  
Target variable: **Selling Price**.

## Project Workflow
1. **Data Cleaning**
   - Removed unnecessary columns (`car_name`, `brand`, `Unnamed: 0`).  
   - Checked and handled missing values.

2. **Feature Engineering & Preprocessing**
   - Encoded categorical features (`fuel_type`, `seller_type`, `transmission_type`, `model`).  
   - Scaled numerical features using `StandardScaler`.  
   - Applied One-Hot Encoding for categorical features.  

3. **Model Training**
   - Compared multiple regression models:  
     - Linear Regression  
     - Lasso Regression  
     - Ridge Regression  
     - K-Nearest Neighbors (KNN)  
     - Decision Tree Regressor  
     - Random Forest Regressor
     - AdaBoost Regressor

4. **Model Evaluation**
   - Metrics used: **MAE, MSE, RMSE, R² Score**.  
   - Evaluated models on both training and test sets.  

5. **Hyperparameter Tuning**
   - Applied `RandomizedSearchCV` for:  
     - K-Nearest Neighbors (KNN)  
     - Random Forest Regressor  

6. **Model Selection**
   - Selected the best-performing models after tuning.

## Results
- **Random Forest Regressor** (after tuning):  
  - Test RMSE: ~1.20  
  - Test MAE: ~0.85  
  - R² Score: ~0.92  

- **K-Nearest Neighbors (KNN)** (after tuning):  
  - Test RMSE: ~1.40  
  - Test MAE: ~1.05  
  - R² Score: ~0.89  

📌 Random Forest performed best overall in predicting car prices.  

## Installation & Usage
```bash
git clone https://github.com/ManelHjaoujia/car-price-prediction.git
cd car-price-prediction
pip install -r requirements.txt
```
## Dependencies
- Python 3.8+
- pandas  
- numpy  
- matplotlib  
- seaborn  
- plotly  
- scikit-learn  

## Key Learnings
- Data preprocessing techniques: encoding, scaling, handling categorical and numerical features.  
- Comparison of regression models and their trade-offs.  
- Importance of evaluation metrics (RMSE, MAE, R²) for regression problems.  
- Hyperparameter tuning with `RandomizedSearchCV` to optimize model performance.  
- Practical application of ensemble methods like Random Forest.  

## Author
**Manel Hjaoujia**  
Junior Data Scientist 
Passionate about Data Science & Machine Learning  
