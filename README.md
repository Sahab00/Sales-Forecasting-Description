# Sales-Forecasting-Description

# Project Description 
"This project aims to build a machine learning model that forecasts weekly sales for retail stores. It was developed as part of my internship at Elevvo."

# Sales-Forecasting-Description/
│── code_model.ipynb # Main Jupyter Notebook
│── train.csv        # Training data
│── test.csv         # Test data
│── features.csv     # Additional features (holidays, CPI, fuel price, etc.)
│── stores.csv       # Store details (Type, Size)
│── submission.csv   # Final predictions
│── README.md        # Project documentation

# Workflow

# Data Loading
Train, Test, Features, and Store datasets are loaded.
All datasets are merged into one consolidated dataframe.

# Data Preprocessing
Missing values handled with forward-fill.
Date column converted to datetime.
New time-based features: Year, Month, Week.
Categorical encoding:
IsHoliday → integer (0/1)
Type (A/B/C) → numeric (1/2/3)

# Modeling

Model: XGBRegressor

# Evaluation Metrics
RMSE (Root Mean Squared Error)
MAE (Mean Absolute Error)
R² (Coefficient of Determination)

# Visualization
Scatter plot: Actual vs Predicted sales.
Metric performance visualization (bar chart).
# Final Predictions
Model applied on test.csv.
Output saved as submission.csv

# Model Performance
On validation set:
RMSE: 4139.40
MAE: 2235.01
R²: 0.9671 ✅

# How to Run
git clone https://github.com/Sahab00/Sales-Forecasting-Description.git
cd Sales-Forecasting-Description

# Install dependencies:
pip install -r requirements.txt

# Run the notebook:
jupyter notebook code_model.ipynb

# Predictions will be saved in:
submission.csv

