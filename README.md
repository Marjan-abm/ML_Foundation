# 🏠 Seattle Housing Data Analysis (ML Foundations)

This project explores housing data from King County, WA (including Seattle) using machine learning foundations. The dataset contains details about house sales and is used to demonstrate exploratory data analysis and basic modeling workflows.

## 📁 Project Structure

- `ml-foundations.ipynb`: Jupyter notebook with all code and analysis.
- `dataset.arff`: Raw dataset in ARFF format.
- `requirements.txt`: Python dependencies.
- `.vscode/`, `venv/`: Development environment (excluded from GitHub).

## 🔍 Key Features

- Data loaded from ARFF format into Polars DataFrame
- Cleaned and engineered features (e.g. converting dates, categoricals)
- Visualized relationships between features using Altair and Matplotlib
- Filtered and grouped data by zip codes and months
- Explored correlations and pricing trends

## 🚀 How to Run

1.Clone this repo:
   ```bash
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

Author : Mary Abd
