## 문제 접근

### 목표

- feature들이 주어질 때, 주택 가격을 예측하는 문제

### 데이터 특징

- feature 개수가 79개
- 회귀 문제
- logistic regression이 가장 먼저 떠오름

### 결과

| 모델                   | 제출 파일명                | Public Score   |
| ---------------------- | -------------------------- | -------------- |
| Linear Regression      | lr_submission.csv          | 15394.27816    |
| Ridge Regression       | ridge_submission.csv       | 15678.23869    |
| Lasso Regression       | lasso_submission.csv       | 15424.11532    |
| XGBoost                | xgboost_submission.csv     | 14988.92630    |
| LightGBM               | lgbm_submission.csv        | 14949.66777 ✅ |
| LightGBM (Optuna 튜닝) | lgbm_optuna_submission.csv | 14957.33372    |
| Stacking Ensemble      | stacking_submission.csv    | 14986.39778    |
