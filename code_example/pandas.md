## rank
```python
df['rank_by_average'] = df['score'].rank(ascending=False)
```
- 평균(method='average') : 동점 관측치 간의 그룹 내 평균 순위 부여 (default 설정)
- 최소값(method='min') : 동점 관측치 그룹 내 최소 순위 부여
- 최대값(method='max') : 동점 관측치 그룹 내 최대 순위 부여
- 첫번째 값 (method='first') : 동점 관측치 중에서 데이터 상에서 먼저 나타나는 관측치부터 순위 부여
- 조밀하게 (method='dense') : 최소값('min')과 같은 방법으로 순위부여하나, 'min'과는 다르게 그룹 간 순위가 '1'씩 증가함 (like ‘min’, but rank always increases by 1 between groups)
