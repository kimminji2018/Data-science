## 문제
TrainSet 5 를 학습 데이터셋으로 활용하여 아래 가이드에 따라 조종키 방향 LABEL) 을
예측하는 **KNN 분류 모형을 학습한 후 TestSet5** 에 대한 예측을 수행하시오 이때 학습 시 참조
할 **이웃의 수는 2, 3, 4** 개로 설정하여 총 3 개의 모형 학습을 학습하고 각 모형에 대한 예측을 수행 하시오
- 입력 변수 총 24 개 표준화된 24 개의 센서값 SENSOR1 S ~ SENSOR24 _S
- 학습 시 , 유클리드 거리를 데이터간 거리로 사용하시오
 
## 예제 코드

```python
model2 = KNeighborsClassifier(n_neighbors=2).fit(train2.iloc[:,2:27], train2['LABEL'])
```


