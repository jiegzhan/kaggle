### Project: House Prices Advanced Regression Techniques

### Highlights:

 - This is a **Regression** problem.
 - The purpose of this project is to **predict house prices**. 
 - The model was built with **Linear Regression** on top of **Scikit Learn**.

### Data: [Kaggle House Price Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)

### Train:

```
from sklearn.ensemble import RandomForestRegressor
lr = RandomForestRegressor(n_estimators=80, max_depth=100, random_state=42)
lr.fit(X_train, y_train)
```

### Predict:

```
y_pred = rf.predict(X_test)
```

### Evaluate:

```
from sklearn.metrics import mean_squared_error, r2_score
print(mean_squared_error(y_test, y_pred))
print(r2_score(y_test, y_pred))
```

### Reference:
 - [sklearn.linear_model.LinearRegression](http://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
