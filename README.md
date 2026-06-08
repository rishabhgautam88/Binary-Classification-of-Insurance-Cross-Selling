# Binary Classification of Insurance Cross-Selling

## Project Overview
This project focuses on building a binary classification model to predict whether a customer who already has Health Insurance will be interested in purchasing Vehicle Insurance (Cross-Selling).

## Requirements and Dependencies
The code is written in Python within a Jupyter Notebook environment. Ensure you have the following libraries installed:
- `numpy`
- `pandas`
- `seaborn`
- `matplotlib`
- `scikit-learn`
- `ydata-profiling`
- `mlxtend`
- `scipy`

## Data
- **Input:** The model expects a training dataset named `train.csv`. The `id` column is dropped during preprocessing.
- **Output:** The final predictions and probabilities are saved to `df_vertical.csv`.

## Methodology
1. **Exploratory Data Analysis (EDA):** Uses tools like `ydata_profiling` for comprehensive data profiling.
2. **Data Preprocessing:** - Ordinal encoding for `Vehicle_Age` (`< 1 Year`: 0, `1-2 Year`: 1, `> 2 Years`: 2).
   - One-Hot Encoding for categorical features (`Gender`, `Vehicle_Damage`) using `ColumnTransformer`.
3. **Modeling:** Employs an ensemble learning technique, specifically a `BaggingClassifier` (likely with `DecisionTreeClassifier` as the base estimator), to improve classification accuracy and robustness.
4. **Evaluation:** Model performance is assessed using various metrics including accuracy, precision, recall, F1-score, and ROC-AUC.

## Usage
1. Ensure `train.csv` is located in the same directory as the notebook.
2. Run the Jupyter Notebook `Binary-Classification-of-Insurance-Cross-Selling.ipynb` cell by cell.
3. The final output file `df_vertical.csv` will be generated in the root directory.Added project
