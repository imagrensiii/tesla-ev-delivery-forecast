# Tesla EV Delivery Forecasting - Data Mining Project

## Project Overview
This project was developed for my MSc Data Mining module. It involves building a machine learning model to predict Tesla's global quarterly vehicle deliveries by region and model. The goal was to transform raw delivery data into actionable business insights for production planning and regional strategy.

## Business Problem
Accurate delivery forecasting is critical for Tesla's supply chain and production efficiency. Traditional methods struggle with complex seasonal patterns and regional variations. This model provides data-driven forecasts to reduce operational uncertainty.

## Dataset
*   **Source:** Compiled Tesla delivery data (2015-2025).
*   **Size:** ~2,500 observations.
*   **Key Features:** Region, Model, Quarter, Price, Range, Charging Infrastructure Index, Historical Deliveries.
*   **Target Variable:** Quarterly Deliveries.

## Methodology & Tech Stack
1.  **Data Preprocessing:** Handled missing values, performed feature engineering (e.g., price-per-km ratio).
2.  **Modeling:** Compared Linear Regression, Random Forest, and **XGBoost** using a time-series split (train: 2015-2023, test: 2024-2025).
3.  **Evaluation:** Selected XGBoost based on **R² score of 0.89** on the test set.
4.  **Tools:** Python, Pandas, Scikit-learn, XGBoost, Matplotlib/Seaborn.

## Key Results & Insights
*   **Model Performance:** XGBoost achieved an **R² of 0.89**, accurately capturing delivery trends.
*   **Business Insight:** Identified a consistent **25-30% quarterly delivery surge in Q4**, crucial for capacity planning.
*   **Regional Strategy:** Analysis suggested:
    *   **North America/EU:** Focus on technology and range.
    *   **Asia:** Emphasize affordable pricing and charging infrastructure.
    *   **Middle East:** Target luxury segment and fast-charging network development.

## How to Run the Code
1.  Clone this repository.
2.  Install required packages: `pip install pandas numpy scikit-learn xgboost matplotlib seaborn`
3.  Run the main analysis script: `python tesla_analysis.py`

## Project Structure
```
tesla-ev-delivery-forecast/
│   README.md
│   tesla_analysis.py   # Main Python script
│   tesla_deliveries.csv # Dataset
│   BM.pptx             # Presentation slides
```

## Author
**Grensi Patoliya** | MSc Big Data Management @ Griffith College Dublin
*   [LinkedIn](https://www.linkedin.com/in/grensi-patoliya)
