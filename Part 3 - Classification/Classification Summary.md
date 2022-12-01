# 1. 각 모델의 장단점은?
| Classification Model | Pros | Cons |
| -------------------- | ---- | ---- |
| Logistic Regression  | 확률적 접근 방식<br> features의 statistical significance에 대한 정보를 제공한다.| Logistic Regression Assumption|
| K-NN | 이해하기 쉬움<br> 빠르고 효과적임 | neighbours k의 수를 정해야 함 |
| SVM | 이상적<br> Outlier(이상값)에 편향되지 않음<br> 과적합에 민감하지 않음 | 비선형 데이터 셋에는 적합하지 않음<br> feature가 많은 데이터 셋에 효과적이지 않음 |
| Kernel SVM | 비선형 데이터셋에 높은 성능<br> Outlier에 편항되지 않음<br> 과적합에 민감하지 않음 | feature가 많은 데이터 셋에 효과적이지 않음<br>복잡함 |
| Naive Bayes | 효과적임<br>Outlier에 편향되지 않음<br>비선형 데이터셋에 적합<br>확률적 접근 | feature들이 같은 통계적 관련성을 갖는다는 것을 기반으로 해야함 |
| Decision Tree Classification | Interpretability(해석 가능성)<br>feature scaling이 필요하지 않음<br>선형, 비선형 데이터 셋에서 모두 작동함 | 작은 dataset에서 최악의 결과를 나타냄<br> 과적합이 자주 발생함 |
| Random Forest Classification | 강력하고 정확함<br>비선형 데이터 셋에서 우수한 성능을 나타냄 | 해석 불가능<br>과적합이 쉽게 발생함<br>나무의 수를 선택해야함. |

# 2. 내 데이터 셋에 맞는 모델을 고르는 방법은?
    1. 회귀 모델과 마찬가지로 먼저 문제가 선형인지 비선형인지 파악해야 한다.


    이를 수행 하는 법은 Part 10에서 다루고 있다.
  
    데이터 셋이 선형이면 SVM 또는 Logistic Regression으로 해결한다.
  
    데이터 셋이 비선형이면 KNN, Naive Bayes, Random Forest, Decision Tree를 사용하여 해결한다.

    2. 비지니스 관점에서 다음을 선택한다.

    - Logistic Regression이나 Naive Bayes를 확률에 따라 예측 순위를 지정하는 모델이다.

    예를 들어, 고객이 특정 제품을 구매할 확률이 가장 높은 것부터 가장 낮은 것까지 순위를 매기려는 경우에 사용할 수 있다.
    이를 통해, 마케팅 캠페인을 타켓팅 할 수 있다.

    - SVM은 고객이 속한 세그먼트를 예측하려는 경우 사용 한다. 세그먼트의 경우 모든 종류가 상관 없다.
    - Decision Tree는 결과에 대한 명확한 해석을 원할 때 사용한다.
    - Random Forest는 해석의 필요성이 적고, 고성능을 원할 때 사용한다.

# 3. 이 모델들을 어떻게 개선할수 있는가?
    Parameter를 tuning함으로써 개선할 수 있는데, 이는 Part 10에서 답변을 찾을 수 있다.
