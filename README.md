# model_xgboost

There are two important folders under the main branch, model_data and model_xgb:

1. The model_data file is the data set participating in the model training set. The last column is the dependent variable, and all are independent variables except the last column, which is the format of the data set participating in model verification.

independent variables: Age(years), SBP(mmHg), Fasting glucose(mmol/L), Insulin therapy, MCHC(g/L), PDW(fL), UA(umol/L), SCR(umol/L), FIB(g/L), INR, LDL-C(mmol/L).
dependent variable: Group

2.model_xgb file is a packaged model file that can be directly run when imported into python without retraining the model.

Import a pkl file: 

		#joblib.load(open("model_xgb.pkl", 'rb'))
  
  		#classifier.predict_proba(X.iloc[3:10, :])[:,1]
