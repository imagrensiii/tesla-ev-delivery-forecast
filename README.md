# Tesla EV Delivery Forecasting - Data Mining Project

## Project Overview
This project was developed for my MSc Data Mining module. It involves building a machine learning model to predict Tesla's global quarterly vehicle deliveries by region and model. The goal was to transform raw delivery data into actionable business insights for production planning and regional strategy.

## Business Problem
Accurate delivery forecasting is critical for Tesla's supply chain and production efficiency. Traditional methods struggle with complex seasonal patterns and regional variations. This model provides data-driven forecasts to reduce operational uncertainty.

## Dataset
*   Source: Compiled Tesla delivery data (2015-2025).
*   Size: ~2,500 observations.
*   File: `tesla_deliveries_dataset_2015_2025.csv`
*   Key Features: Region, Model, Quarter, Price, Range, Charging Infrastructure Index, Historical Deliveries.
*   Target Variable: Quarterly Deliveries.

## Methodology & Tech Stack
1.  Data Preprocessing: Handled missing values, performed feature engineering (e.g., price-per-km ratio).
2.  Modeling: Compared Linear Regression, Random Forest, and **XGBoost** using a time-series split (train: 2015-2023, test: 2024-2025).
3.  Evaluation: Selected XGBoost based on **R² score of 0.89** on the test set. Feature importance analysis saved to `feature_importance.csv`.
4.  Tools: Python (Jupyter Notebook), Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn.

## Key Results & Insights
*   Model Performance: XGBoost achieved an R² of 0.89, accurately capturing delivery trends.
*   Business Insight: Identified a consistent 25-30% quarterly delivery surge in Q4, crucial for capacity planning.
*   Regional Strategy: Analysis suggested:
    *   North America/EU: Focus on technology and range.
    *   Asia: Emphasize affordable pricing and charging infrastructure.
    *   Middle East: Target luxury segment and fast-charging network development.
*   Full results and metrics: Available in `model_results.csv`

## How to Run the Code
1.  Clone this repository:
    ```bash
    git clone https://github.com/YOUR_USERNAME/tesla-ev-delivery-forecast.git
    ```
2.  Navigate to the project folder:
    ```bash
    cd tesla-ev-delivery-forecast
    ```
3.  Install required packages:
    ```bash
    pip install pandas numpy scikit-learn xgboost matplotlib seaborn jupyter
    ```
4.  Open and run the Jupyter Notebook:
    ```bash
    jupyter notebook main_analysis.ipynb
    ```

## Project Structure
tesla-ev-delivery-forecast/
│ main_analysis.ipynb # Main Jupyter Notebook with full analysis
│ tesla_deliveries_dataset_2015_2025.csv # Dataset
│ feature_importance.csv # Feature importance results
│ model_results.csv # Model performance metrics
│ IEEE_Conference.pdf # Related research paper
│ .gitignore # Git ignore file


## Author
*   Grensi | MSc Big Data Management @Griffith College Dublin
*   [LinkedIn](https://www.linkedin.com/in/grensi-patoliya)
*   [GitHub](https://github.com/imagrensiii)
