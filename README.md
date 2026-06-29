# NBA Player Longevity Prediction - Feature Engineering

## Project Overview
This project demonstrates **feature engineering** for predicting NBA rookie career longevity (whether a player lasts **5+ years** in the league using `target_5yrs`).

We transformed raw rookie-season statistics into a clean, high-quality dataset suitable for machine learning.

## Key Steps Completed
- Loaded and explored the dataset (`nba-players.csv`)
- Defined `target_5yrs` as the binary target variable
- Removed non-predictive columns (`name`, `Unnamed: 0`) to avoid data leakage
- Performed correlation analysis to detect and reduce multicollinearity
- Engineered new composite features:
  - `ppm` → Points Per Minute
  - `efficiency` → Simple player efficiency rating
  - `ast_tov_ratio` → Assist-to-Turnover ratio
- Handled missing values explicitly
- Visualized target distribution
- Applied feature scaling with `StandardScaler`
- Produced clean final datasets

## Dataset
- **Original**: 1,340 rookies, 22 columns
- **Final**: 1,340 rows, 15 columns (after engineering)

## Files
- `nba_feature_engineering.ipynb` — Complete Jupyter Notebook with all code, visualizations, and explanations
- `README.md` — This file

## Technologies
- Python, Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn

## How to Use
1. Open `nba_feature_engineering.ipynb` in Jupyter / VS Code
2. Run all cells
3. Use `nba_players_engineered.csv` or `nba_players_scaled.csv` for modeling

## Future Improvements
- Build classification models (Logistic Regression, Random Forest, XGBoost)
- Handle mild class imbalance
- Advanced feature selection / dimensionality reduction

---

**Status**: Complete & Ready for Modeling  
**Author**: Osemwengie Osasere
