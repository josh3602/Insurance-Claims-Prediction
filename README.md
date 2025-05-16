# COMP 3608 Final Project – Insurance Claim Prediction

### Team Members:
- Sanjay Bispath

### Project Overview
This project explores the use of machine learning to predict health insurance claim charges using demographic and departmental features (age, gender, smoker status, profession, etc.). The primary goal is to assess premium fairness and help insurers align premiums with true underlying risk.

### Models Implemented
1. **Hosein’s Distance-Based Model**
   - Personalized claim rate prediction using a distance-weighted average in claim-rate space.
   - Tuned using k-fold cross-validation for optimal bias-variance trade-off.
   - Highly interpretable.

2. **Random Forest Regressor**
   - Ensemble tree-based model.
   - Strong performance and feature importance insights.

3. **XGBoost Regressor**
   - Gradient-boosted trees with regularization.
   - Best overall performance in accuracy.

### Evaluation Metrics
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **Normalized MAE** (relative to global mean baseline)

### Key Results
| Model                    | MAE      | RMSE     | Normalized MAE |
|--------------------------|----------|----------|----------------|
| Hosein Distance-Based    | ----     | ----     | 0.2611         |
| Random Forest Regressor  | 454.26   | 1342.71  | 0.0486         |
| XGBoost Regressor        | 449.55   | 1047.02  | 0.0481         |

### Business Insights
- Smoker status and profession are major risk indicators.
- Certain demographic groups are either overcharged or undercharged based on current flat premium rates.
- Hosein’s method helps explain premiums to customers in a transparent manner.
