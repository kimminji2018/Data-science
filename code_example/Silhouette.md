## 문제
생성된 군집 모형 별로 Silhouette 계수를 계산하 시오
 
## 예제 코드

```python
from sklearn.metrics import silhouette_score
silhouette_score(df3_dummy[input_list3],model3.labels_)
```
data와 label를 넘겨주면 sillhouette 계수를 계산해준다.

## Sillhouette 계수란?
- 클러스터링(군집화) 결과를 평가하느 지표로써 각 데이터별로 그 데이터가 속한 군 내의 (거리 기반) 유사도와 인접한 군의 유사도를 비교하는 지표
### 장점
- 클러스터의 개수를 판단하는데 활용할 수 있다.
### 단점
- 계산량이 많다
