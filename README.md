# NBA MVP Prediction: Data Analysis & Model

This project combines my passion for basketball with data science techniques to predict NBA Most Valuable Player (MVP) voting. Using player season statistics from 1982 onward, we explore which factors correlate with MVP success and train models to forecast award shares.

## Project Highlights

- **Exploratory Data Analysis** – cleans the dataset, engineers an `mvp` label for each season's winner, and visualizes relationships between advanced stats and award shares.
- **Machine Learning Models** – trains Ridge Regression and Random Forest regressors to estimate MVP voting results.
- **Model Evaluation** – measures performance using mean squared error and backtests predictions across seasons.

## Dataset

The notebook expects the [NBA Player Season Statistics With MVP Win Share](https://www.kaggle.com/datasets/robertsunderhaft/nba-player-season-statistics-with-mvp-win-share) dataset from Kaggle. After downloading, place `NBA_Dataset.csv` in a convenient location and update the file path in the notebook if needed.

## Requirements

- Python 3
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`
- `jupyter`

Install the dependencies with:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Running the Notebook

1. Launch Jupyter:
   ```bash
   jupyter notebook "MVP PREDICTOR .ipynb"
   ```
2. Execute each cell in the notebook to reproduce the analysis, train the models, and see the 2022 prediction results.

## Results

- **Ridge Regression** – Mean Squared Error around `0.00495`.
- **Random Forest** – Mean Squared Error around `0.00156`.

Lower scores indicate better predictions. The Random Forest model performed best in testing.

## Acknowledgements

- Kaggle contributor **RobertsUnderhaft** for compiling the dataset.
- Inspiration from David Yoo's article: [Predicting the Next NBA MVP using Machine Learning](https://towardsdatascience.com/predicting-the-next-nba-mvp-using-machine-learning-62615bfcff75).

---
This repository demonstrates data cleaning, visualization, and machine learning skills in the context of NBA analytics. Feel free to clone the project and extend the models or visualizations.
