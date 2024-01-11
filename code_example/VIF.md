## 문제
다중 공선성을 피하기 위해 VIF(Variance Inflation Factors) 를 이용하여 변수를 제거하려고 한다.
이 때 절편 Intercept) 은 VIF 계산에 포함하여 계산하도록 한다
 
## 예제 코드

```python
from statsmodels.stats.outliers_influence import variance_inflation_factor
from patsy import dmatrices
formula_like = "SATISFACTION ~ " + " + ".join(df.columns[1:-1])
y, x = dmatrices(formula_like, df, return_type='dataframe')
v = []
for i in range(0,12):
    v = v + [vif(x.values, i)]
v
```
