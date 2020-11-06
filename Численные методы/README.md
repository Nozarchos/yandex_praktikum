# Описание проекта
  На исторических данных об объявлений машин нужно обучить модель для оценки рыночной стоимости автомобиля.
  Данные с пропусками и выбросами.
  
  
# Инструментарий
```python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt; sns.set()
from sklearn.linear_model import LinearRegression
from sklearn.tree import DecisionTreeRegressor
from sklearn.ensemble import RandomForestRegressor
from catboost import CatBoostRegressor
from sklearn.model_selection import cross_validate
import lightgbm as lgb
from sklearn.metrics import mean_squared_error
from sklearn.model_selection import train_test_split, RandomizedSearchCV
```

# Произведена оценка различных моделей

Property   | LinearRegr    | DecisionTree  | RandomForest  | CatBoost  | LightGBM |
---------- | -------------:|--------------:| -------------:| ---------:| --------:|
Quality    |2794.5         |2069.80        |1758.5         |1646       |1631.9    |
Pred_speed |0.011          |236            |0.007          |0.007      |5         |
Fit_speed  |32.2           |8.74           |349            |3852       |358       |
