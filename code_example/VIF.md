## 문제
다중 공선성을 피하기 위해 VIF(Variance Inflation Factors) 를 이용하여 변수를 제거하려고 한다.
이 때 절편 Intercept) 은 VIF 계산에 포함하여 계산하도록 한다
 
## 예제 코드

```python
from statsmodels.stats.outliers_influence import variance_inflation_factor
df2_1 = df2.iloc[:,1:-1]
df2_1['const'] = 1

vif = pd.DataFrame()
vif['VIF Factor'] = [variance_inflation_factor(df2_1.values, i) for i in range(df2_1.shape[1])]
```
