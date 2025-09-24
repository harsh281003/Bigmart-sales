# BigMart Sales Prediction 🛒📊

A machine learning project that predicts retail sales for BigMart outlets using historical product and outlet data. This project applies end-to-end data science practices to generate business insights and build a predictive model to support inventory and pricing strategies.

## 📌 Project Overview

This project leverages a regression-based machine learning model (XGBoost) to forecast sales of products across multiple BigMart outlets. By analyzing sales data from 2013, it identifies key sales drivers and enables data-driven decision-making for retail optimization.

## 🗂️ Dataset

The dataset includes 8523 records with the following key features:
- `Item_Identifier`, `Item_Weight`, `Item_Fat_Content`, `Item_Visibility`, `Item_Type`, `Item_MRP`
- `Outlet_Identifier`, `Outlet_Establishment_Year`, `Outlet_Size`, `Outlet_Location_Type`, `Outlet_Type`
- **Target**: `Item_Outlet_Sales`

## 🔍 Project Pipeline

1. **Data Collection & Exploration**
   - Loaded dataset with Pandas
   - Used `.describe()`, `.info()`, and visualizations for initial analysis

2. **Exploratory Data Analysis (EDA)**
   - Visualized feature distributions using **Matplotlib** and **Seaborn**
   - Identified key correlations and feature patterns

3. **Data Preprocessing**
   - Imputed missing values for `Item_Weight` and `Outlet_Size`
   - Standardized categorical values (e.g., 'low fat', 'LF')
   - Applied **Label Encoding** to categorical features

4. **Model Building**
   - Split data into train-test sets using `train_test_split`
   - Trained **XGBoost Regressor** on training data

5. **Model Evaluation**
   - Achieved **R² Score: 0.87 (Train)**, **0.50 (Test)**
   - Evaluated model generalization and overfitting

## 🧰 Tech Stack

- **Python 3**
- **Pandas**, **NumPy** — Data manipulation
- **Matplotlib**, **Seaborn** — Visualization
- **Scikit-learn** — Preprocessing, evaluation
- **XGBoost** — ML model
- **Jupyter Notebook** — Development environment

## 🚀 Getting Started

### Clone the Repository

```bash
git clone https://github.com/harsh281003/bigmart-sales-prediction.git
cd bigmart-sales-prediction
