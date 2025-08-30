# Sales-Forecasting-Description

# Project Description 
"This project aims to build a machine learning model that forecasts weekly sales for retail stores. It was developed as part of my internship at Elevvo."

# Sales-Forecasting-Description/
1) code_model.ipynb # Main Jupyter Notebook
2)  train.csv        # Training data
3)   test.csv         # Test data
4)     atures.csv     # Additional features (holidays, CPI, fuel price, etc.)
5) stores.csv       # Store details (Type, Size)
6)  submission.csv   # Final predictions
7)   README.md        # Project documentation

# Workflow

# Data Loading
Train, Test, Features, and Store datasets are loaded.
All datasets are merged into one consolidated dataframe.

# Data Preprocessing
1) Missing values handled with forward-fill.
2) Date column converted to datetime.
3) New time-based features: Year, Month, Week.
4) Categorical encoding:

# Modeling

Model: XGBRegressor

# Evaluation Metrics
RMSE (Root Mean Squared Error)
MAE (Mean Absolute Error)
R² (Coefficient of Determination)

# Visualization
Scatter plot: Actual vs Predicted sales.
Metric performance visualization (bar chart).

<img width="1017" height="644" alt="Screenshot 2025-08-30 151355" src="https://github.com/user-attachments/assets/8ee02a9a-de6b-4692-b3f5-a84beb51af68" />


# Final Predictions
Model applied on test.csv.
Output saved as submission.csv

<img width="1179" height="632" alt="Screenshot 2025-08-30 151418" src="https://github.com/user-attachments/assets/dde4842a-1345-47c2-943a-449417cc8d6b" />

<img width="1228" height="545" alt="Screenshot 2025-08-30 151428" src="https://github.com/user-attachments/assets/8a67082b-c3ee-434a-9bf3-6b3fd66053d3" />



# Model Performance
On validation set:
RMSE: 4139.40
MAE: 2235.01
R²: 0.9671 


# How to Run
git clone https://github.com/Sahab00/Sales-Forecasting-Description.git
cd Sales-Forecasting-Description

# Install dependencies:
pip install -r requirements.txt

# Run the notebook:
jupyter notebook code_model.ipynb

# Predictions will be saved in:
submission.csv

