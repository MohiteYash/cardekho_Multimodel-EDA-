# Car Price Prediction -

This project aims to predict the selling price of cars using various machine learning models. The workflow includes data preprocessing, feature engineering, visualization, model training, and evaluation. The dataset is sourced from CarDekho (via Kaggle) and contains detailed information about used cars.

---

## Dataset Information

- Dataset Name: Car details v3.csv
- Source: CarDekho (Kaggle)
- Target Variable: `selling_price`
- Key Features:
  - `name` (car brand and model)
  - `year`, `km_driven`, `fuel`, `seller_type`, `transmission`, `owner`
  - `mileage`, `engine`, `max_power`, `seats`

---

## Exploratory Data Analysis

- Extracted and visualized top 20 car brands using bar plots.
- Checked for missing values and handled them accordingly.
- Used pairplots and heatmaps to analyze correlations.
- Explored distribution of categorical and numerical features.

---

## Data Preprocessing

- Extracted brand names from the `name` column.
- Filled missing values in features like `mileage`, `engine`, `max_power`, and `seats`.
- Converted categorical columns using `LabelEncoder` and `OrdinalEncoder`.
- Removed irrelevant columns.
- Ensured all features were numerical before modeling.

---

## Models Implemented

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor

Each model was evaluated using:
- R² Score
- Mean Squared Error (MSE)
- Cross-validation score

---

## Model Evaluation Results

| Model            | Cross-Validation Score | Training Accuracy (%) | Testing Accuracy (%) | R² Score (%) |
|------------------|------------------------|------------------------|----------------------|--------------|
| Linear Regression | 66.14                  | 67.73                  | 69.02                | 69.02        |
| Random Forest     | -                      | 98.85                  | 96.91                | 96.91        |
| XGBoost           | -                      | 96.97                  | 95.85                | 95.85        |

- Best Performing Model: Random Forest Regressor
- Achieved 96.91% accuracy on the test set with minimal overfitting.

---

## Results and Visualizations

- Top car brands were visualized using a bar chart based on frequency.
- Testing accuracy of all models was compared using a multi-colored bar chart.
- Accuracy values were displayed inside the bars for better readability.

---

## Libraries Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost

---

## How to Run

1. Open the `cardekho_FA_2.ipynb` notebook.
2. Ensure the dataset `Car details v3.csv` is available in your working directory.
3. Run the notebook cell by cell to see preprocessing, visualization, modeling, and evaluation.

---

## Contact

For queries or suggestions, feel free to reach out.
