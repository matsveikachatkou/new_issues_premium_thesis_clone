# New Issues Premium in the European Corporate Bond Market: From Empirical Evidence to Forecasting

Welcome to the README for the "New Issues Premium in the European Corporate Bond Market: From Empirical Evidence to Forecasting" project. This project is a part of a master's thesis focused on analyzing and forecasting the new issues premium in the European corporate bond market.

The new issues premium is a critical metric that reflects the pricing dynamics of newly issued corporate bonds compared to their secondary market counterparts. Through empirical analysis and forecasting techniques, this project aims to provide valuable insights into the behavior of the new issues premium and its potential predictability.

## Features

- In-depth empirical analysis of the European corporate bond market
- Utilization of forecasting models to predict new issues premium behavior
- Data visualization to illustrate pricing dynamics

## Project Structure

The project is organized as follows:

- `data/`: This directory contains the raw and processed data used in the analysis.
The original dataset used in this project was sourced from Bloomberg and Refinitiv terminals during my university research. 
Due to licensing and confidentiality restrictions, the data files are not included in this public repository. 
The code structure and analytical logic remain fully intact.
- `requirements.txt`: Requirments for python environment.
- `README.md`: The document you're currently reading.

## Reproduce results

To reproduce the analysis and findings of this thesis project, follow these steps:

1. Clone the repository:
   ```bash
   $ git clone https://github.com/matsveikachatkou/new_issues_premium_agi.git
   $ cd new_issues_premium_agi
   $ pip install -r requirements.txt
2. For NIP analysis, explore Jupyter notebooks in `notebooks/`.
3. For feature selection analysis, explore `feature_engineering.ipynb` in `data/preprocessed`.
4. For multicollinearity analysis, run `multicollinearity_checker.py`. Results stored in `src/results/`.
5. For regression analysis, run `linear_regression_panel_analysis.py`, `linear_regression_panel_analysis_rating.py`, `robust_linear_regression_panel_analysis.py` in `src/`. Results stored in `src/results/`. To run regression for different rating subgroup, change panel_filtered = panel[panel['rating'].between(8, 16)]. The assigned rating values can be found in `data_preprocessing.py`.
6. For ML models results, run the corresponding scripts. The metrics are printed out in the console. Results of model comparison are saved as txt files, feature importance is saved as pictures.
