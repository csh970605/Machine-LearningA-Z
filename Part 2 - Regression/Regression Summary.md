# 1. 각 회귀모델의 장단점
| Regression Model | Pros | Cons |
| --- | --- | --- |
| Linear Regression | 데이터 셋의 크기에 구애받지 않음<br>feature들의 관련성에 대한 정보를 제공함 | The Linear Regression Assumptions |
| Polynomial Regression | 데이터 셋의 크기에 구애받지 않음<br>비선형 구조에 잘 작동함 | 좋은 bias(편향)/variance(분산) 절충을 위해 올바른 polynomial degree(다항식 차수)를 선택해야함 |
| SVR | 쉽게 적응함<br>비선형 구조에 잘 작동함<br> outlier에 편향되지 않는다. | feature scaling을 해야함<br>잘 알려지지 않음<br>이해하기 어려움 |
| Decision Tree Regression | 이상적임<br>feature scaling이 필요하지 않음<br>선형, 비선형 구조에서 잘 작동함 | 작은 데이터셋에서 안좋은 결과를 냄<br>과적합이 쉬움 |
| Random Forest Regression | 강력하고 정확함<br>많은 데이터 셋에서 좋은 결과를 냄 | 이상적이지 않음<br>과적합이 쉬움<br>나무 수를 정해야함 |
# 2. 회귀 모델을 개선하는 방법
    Parameter를 tuning함으로써 개선할 수 있는데, 이는 Part 10에서 답변을 찾을 수 있다.
