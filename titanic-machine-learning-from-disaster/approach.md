## 문제 접근

### ✅ ML vs DL 선택 기준 (일반적 가이드라인)

| 조건              | ML 적합             | DL 적합                        |
| ----------------- | ------------------- | ------------------------------ |
| **데이터 수 (n)** | n < **10,000**      | n > **50,000~100,000**         |
| **피처 수 (d)**   | 수십~수백           | 수천 이상 (고차원)             |
| **데이터 형태**   | 표(tabular), 수치형 | 이미지, 텍스트, 음성 등 비정형 |
| **해석 필요성**   | 높음                | 낮음                           |
| **훈련 자원**     | 적음 (CPU도 OK)     | 많음 (GPU 필요)                |

---

- Titanic처럼 **n=891, 정형 데이터**인 경우 → **ML이 정답** ✅
- 다양한 ML 모델들을 적용해 보면서 가장 정확도가 높은 ML 모델을 찾아보자.

### ML 모델 시도 순서

1. Logistic Regression → baseline
2. Random Forest
3. XGBoost
4. SVM
5. kNN / Naive Bayes (optional)
6. 위의 모든 방법을 종합하여 결정하는 voting_ensemble

### 모델별 Public Score 정리

| 모델                | Public Score |
| ------------------- | ------------ |
| Logistic Regression | 0.76555      |
| Random Forest       | 0.77033      |
| XGBoost             | 0.76555      |
| SVM                 | 0.77990      |
| k-NN                | 0.76555      |
| Naive Bayes         | 0.74401      |
| Voting Ensemble     | 0.77990      |
