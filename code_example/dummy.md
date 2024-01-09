## 문제
졸업대학교 등급 (UNIV_ 변수의 범주 수준 Category Level) 을 가리키는 더미 변수
들을 생성하시오 이 때 **생성되는 더미 변수의 개수는 범주 수준의 수보다 하나 적은 4 개**로 하며
범주 수준을 사전 순으로 배열했을 때의 **가장 첫 번째 수준을 제거**하시오 예 : ‘Apple’, ‘Banana’,
‘Calamansi’ 세가지 범주를 가진 변수 FRUIT’ 를 더미 변수 화 할 경우 사전 순으로 배열했을 때
가장 첫 번째 수준인 ‘ 에 대한 더미 변수는 생성되지 않고 Banana’ 및 ‘ 에 대한
2 개의 더미 변수 만 생성된다
 
## 예제 코드

```python
  df3_dummy = pd.get_dummies(df3, columns=['UNIV_RATING'], drop_first = True)

```
- columns : dummy를 생성할 colums을 list로 입력
- drop_first : 맨 처음 범주에 대해서는 별도로 dummy variable를 할당하지 않음
