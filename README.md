# Retail Demand Forecasting

## Project Overview

This project explores retail demand patterns and uses machine learning to forecast daily 
demand. The analysis focuses on historical demand trends, weekly and monthly patterns, and 
the use of past demand to predict future values.

## Objectives

* Explore historical retail demand data.
* Analyze demand patterns over time.
* Create forecasting features using lag values, rolling averages, and calendar information.
* Train and evaluate a Random Forest regression model.
* Compare the model's performance with a simple baseline forecast.

## Dataset

Dataset
This project uses an open-source retail demand dataset containing 76,000 records 
and 16 columns, covering January 2022 to January 2024. It includes demand, inventory, 
pricing, promotions, weather, store, and product information.

## Tools and Technologies

* Python
* Pandas and NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Methodology

1. Load and inspect the dataset.
2. Check data quality and explore demand distributions.
3. Analyze daily, weekly, and monthly demand patterns.
4. Create lag features, rolling averages, and calendar features.
5. Split the data chronologically into training and testing sets.
6. Train a Random Forest model and compare its predictions against a baseline.
7. Evaluate the results using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

## Results

| Model         |    MAE |    RMSE |
| ------------- | -----: | ------: |
| Baseline      | 886.93 | 1240.88 |
| Random Forest | 725.62 | 1044.96 |

The Random Forest model achieved lower prediction errors than the baseline. The previous 
day's demand was the most influential feature, accounting for approximately 81.5% 
of the model's feature importance.

## Project Files

* `demand_forecasting.ipynb` — Complete analysis, visualizations, model training, and evaluation.
* `demand_forecasting.csv` — Dataset used for the analysis.
* `README.md` — Project documentation.

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open `demand_forecasting.ipynb` in Jupyter Notebook or VS Code.
4. Run the notebook cells from top to bottom.

## Future Improvements

* Test additional forecasting models.
* Tune model hyperparameters.
* Explore additional features that may improve prediction accuracy.
* Evaluate performance across different forecasting periods.
