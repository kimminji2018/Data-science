## 문제
K Means 군집화를 수행하시오 이때 , 군집의 수를 각각 4 , 5 , 6 개로 설정하여 총 3 개의 군집 모형을 생성한다
 
## 예제 코드

```python
  model3 = KMeans(n_clusters = idx, random_state=1234, n_init=50, max_iter=300).fit(df3_dummy[input_list3])
  model3.labels_
```
- n_clusters : 군집의 수
- .labels : 분류 결과를 확인 할 수 있다
