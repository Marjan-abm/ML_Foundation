Seattle Housing Data Analysis (ML Foundations)

This project explores King County (Seattle area) housing data using foundational machine learning techniques. It covers everything from EDA and feature engineering to model training and evaluation. It's built as part of a deeper dive into machine learning fundamentals, model deployment, and reproducibility.

Project Structure:
ml-foundations.ipynb: Main notebook with all analysis and model comparisons

dataset.arff: Raw dataset from OpenML (ARFF format)

requirements.txt: Python dependencies

.vscode/, venv/: Development environment files (excluded from GitHub)


Key Features:
Loaded .arff dataset into a Polars DataFrame

Cleaned, filtered, and engineered data (e.g., date conversions, categorical handling)

Visualized feature distributions and price correlations using Altair and Matplotlib

Grouped and compared data by zip code and time (e.g., monthly trends)

Evaluated multiple models to find the best performer

Models Trained & Compared:
Linear Regression (baseline)

Decision Tree Regressor

Random Forest Regressor (final choice)

CatBoost Regressor (tried due to handling of categoricals)

Model Evaluation
We evaluated models using:

R² Score – measures explained variance

MAE / RMSE – shows prediction error range

Residual Plots – visual check for bias and trends

Final model:
Random Forest (max_depth=9)
Delivered strong generalization performance without overfitting

MLflow Tracking:
We used MLflow to:

Log models and parameters

Save pipelines as artifacts

Reload models for prediction

Track experiment results

Model was deployed locally using mlflow.pyfunc for endpoint testing.



How to Run:

1.Clone this repo:
   git clone https://github.com/marjan-abm/ML_Foundation.git
   cd ML_Foundation

2. Create and Activate virtual code
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

3. Install Requirements
pip install -r requirements.txt

4. Run the notebook
jupyter notebook

Dataset source : https://www.openml.org/data/download/22044765/dataset

Author : Mary Abd (Full-Stack Engineer with a focus on applied ML & deployment)
