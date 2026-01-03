# Diabetes Progression Prediction & Model Interpretation

Αυτό το project αναλύει το σύνολο δεδομένων "Diabetes" χρησιμοποιώντας διάφορους αλγόριθμους παλινδρόμησης και ερμηνεύει τα αποτελέσματα με την ανάλυση SHAP.

## Μοντέλα που χρησιμοποιήθηκαν:
- **Gaussian Process Regressor (GPR)**
- **Random Forest (RF)**
- **Support Vector Regressor (SVR)**
- **Gradient Boosting Regressor (GBR)**

## Διαδικασία:
1. **Data Preprocessing:** Min-Max Scaling και έλεγχος για NaN τιμές.
2. **Cross-Validation:** Χρήση 6-Fold Cross Validation για αξιοπιστία.
3. **Hyperparameter Tuning:** Χρήση `RandomizedSearchCV` για βελτιστοποίηση των μοντέλων.
4. **Evaluation:** Υπολογισμός RMSE, MAE, MAPE και Max Error.
5. **Explainability:** Ανάλυση SHAP (Summary & Waterfall plots) για την κατανόηση της επίδρασης κάθε χαρακτηριστικού (feature importance).

## Πώς να το τρέξετε:
Εγκαταστήστε τις βιβλιοθήκες:
`pip install -r requirements.txt`