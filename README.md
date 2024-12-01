# machine_learning
- 머신러닝_Task<br>
- **<학습내용>** <br>
  - **House_Price_Prediction_homework_v2:** 집 가격 예측을 위해서 각 컬럼별 상관 계수를 분석한 후 Regression Model등을 활용하여 가장 적합할 model을 MSE로 판단
  - **ML_homework_2:** 주고객이 구매하지 않은 상품에 대해 요금이 청구되지 않도록 신용카드 회사가 신용카드 사기 거래를 식별하는 것. <br>
    본 Task에선 한 데이터 처럼 클래스 간 데이터가 불균형 할 경우, 어떤 성능 지표를 가지고 모델의 학습정도를 파악하는 것이 목표.
    - **ML_homework_2 -> answer :** Recall(재현율)은 분류 모델의 성능을 평가하기 위한 지표 중 하나로, 실제로 양성인 샘플 중에서 모델이 양성으로 정확히 예측한 샘플의 비율을 나타냅니다. Precision(정밀도)는 분류 모델의 성능을 평가하기 위한         지표 중 하나로, 모델이 양성으로 예측한 샘플 중에서 실제로 양성인 샘플의 비율을 나타냅니다. Precision은 모델이 분류한 양성 예측 중에서 실제로 양성인 비율을 나타내며, Recall은 실제 양성 중에서 모델이 양성으로 예측한 비율입니다. F1 score       는 이 두 평가 지표를 모두 고려하여 수식은 2 * (Precision * Recall) / (Precision + Recall)이며 모델의 예측 성능을 평가하기 때문에, 정확한 예측과 재현율의 평균을 동시에 고려할 수 있는 장점이 있습니다.
  - **ML_homework_3:** 본 Task에선 ML_homework_2에서 Randomforest와 GridSearch를 이용해서 예측을 수행해보려 합니다.
      - 위의 결과를 보고 신용카드 사기 거래 탐지를 더 잘하기 위해서는 어떤 모델을 사용해야하는지 파악하는 것이 목표
      - **ML_homework_3 -> answer :** 예를 들어 1개의 거래만 ‘사기’라고 예측해서 실제로 맞히면 Precision은 1(100%) 입니다. 반면에 전체 거래가 ‘사기’라고 예측하면 Recall은 무조건 1(100%) 입니다. 이 각각의 지표가 갖는 바가 중요합니다.
      Precision을 높이면 Recall이 낮아지고, 반대로 Recall을 높이면 Precision이 낮아질 수 밖에 없는 관계다.
      그래서 Precision, Recall 중 어느 하나에 치우친 지표가 아니라 Precision과 Recall의 조화평균인 F1-score를 가장 중요한 평가지표로 다룰 것입니다. 이 때 밑에 코드에서 보듯 F1-score가 가장 높은 RandomForest2를 사용할 것이다.
