### Project: Kaggle Credit Card Fraud Detection

### Highlights:

 - This is a **highly skewed binary classification** problem.
 - The purpose of this project is to **detect fraud credit card transactions**. 
 - The model was built with **Random Forest Classifier** on top of **Scikit Learn**.

### Data: [Kaggle Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud/data)

### Train:

```
from sklearn.ensemble import RandomForestClassifier
from sklearn import metrics

rf = RandomForestClassifier(max_depth=10, random_state=42)
rf.fit(X_train, y_train)
```

### Predict:

```
y_pred = rf.predict(X_test)
```

### Evaluate:

```
from sklearn.metrics import roc_auc_score
roc_auc = roc_auc_score(y_test, y_pred)
```
![roc_auc_curve](https://github.com/jiegzhan/kaggle/blob/master/Credit%20Card%20Fraud%20Detection/roc_auc.png)

### Reference:
 - [sklearn.ensemble.RandomForestClassifier](http://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html#sklearn.ensemble.RandomForestClassifier)
