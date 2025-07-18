# Employee Salary Prediction

This repository contains a machine learning pipeline to predict employee salaries based on features like experience, education, and job role.

## ✅ Files

- `data/sample_data.csv`: sample dataset with features & salary.
- `notebooks/salary_prediction.ipynb`: step-by-step analysis from preprocessing to model evaluation.
- `src/`:
  - `data_preprocessing.py`: cleaning & feature encoding.
  - `train_model.py`: trains and saves model.
  - `predict.py`: loads saved model to predict for new input.
- `requirements.txt`: list of dependencies.

## 📊 How it works

1. Clean and encode the data.
2. Train multiple models (Linear Regression, Decision Tree, Random Forest).
3. Evaluate using R² and RMSE.
4. Save the best model (`model.joblib`).
5. Provide sample prediction from the CLI using `predict.py`.

## 🔧 Run it locally

```bash
pip install -r requirements.txt
python src/train_model.py
python src/predict.py --experience 5 --education "Masters" --role "Data Scientist"
```
