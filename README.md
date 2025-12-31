# Titanic Survival Prediction

**Description**
End-to-end ML pipeline to predict passenger survival using scikit-learn. Preprocessing is done with ColumnTransformer and Pipeline; model used: RandomForestClassifier.

**Project structure**
- `notebook.ipynb` : cleaned notebook with all steps
- `titanic_pipeline.pkl` : trained model (joblib)
- `requirements.txt` : python packages

**How to run**
1. Clone the repo
2. Create virtual env: `python -m venv venv` and activate it
3. Install deps: `pip install -r requirements.txt`
4. Run notebook or load model:
   ```python
   import joblib
   model = joblib.load('titanic_pipeline.pkl')
   preds = model.predict(X_new)
