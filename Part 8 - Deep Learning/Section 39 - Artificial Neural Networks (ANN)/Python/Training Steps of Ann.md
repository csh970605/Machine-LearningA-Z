# 확률적 경사하강법(Stochastic Gradient Descent)으로 Ann 훈련

1. 0에 근접한 작은 수로 weight을 무작위로 초기화한다.
2. input layer에 첫번째 observation을 넣는다. (하나의 feature당 하나의 input node가 존재한다.)
3. Forward-Porgataion: 왼쪽에서 오른쪽으로 각 뉴런의 활성화 영향이 가중치에 의해 제한되는 방식으로 뉴런이 활성화된다.<br>
  예측된 결과 y를 얻을때 까지 반복한다.
4. 실제 값과 예측 값을 비교한다.
5. Back-Propagtion : 오른쪽에서 왼쪽으로 오류가 역전파된다.<br>
  오류에 대한 책임이 있는 정도에 따라 가중치를 업데이트한다.<br>
  학습률은 가중치를 업데이트하는 정도에 따라 결정된다.
6. 1 ~ 5를 반복하고 관측 후 가중치를 업데이트한다.(강화학습)
  Or, 1 ~ 5를 반복하지만 관측을 여러번 하고 가중치를 업데이트 한다.(Batch Learning)
7. training set이 ANN을 통과 한 후 epoch를 만든다.
