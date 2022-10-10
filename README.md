# Classification-Predictor
Trained a Random Forest algorythm to predict when the outcome of an event will be 1 or 0 based on given features.

The data is pulled using a bigquery client and transformed (removing NAs from dependent variables and substituting NAs from independent variables with mean/mode).

After selecting features with heighest AUC scores a Random Forest and Logistic Regression models are trained with different hyperparameters using GridSearchCV to find the better performing model.

The better performing model with the best combination of hyperparameters is then trained and its performance is tested. Additionally the features importance using permutation importance is also evaluated before saving the model to a pickle file, later to be fed real time data to make predictions.


