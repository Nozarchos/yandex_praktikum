# Описание проекта
  На данных о заказах такси за год нужно обучить модель предсказывающую количетсво заказов в будущем.
  Данные без пропусков.
  
# Интересное
  Написал функцию которая одновременно перебирает значения гиперпарметров и количество создаваемых признаков (скользящее среднее и lag).
  
# Инструментарий
```python
import pandas as pd
import numpy as np
from statsmodels.tsa.seasonal import seasonal_decompose
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split, TimeSeriesSplit, RandomizedSearchCV, cross_val_score
from sklearn.linear_model import LinearRegression
from sklearn.tree import DecisionTreeRegressor
from sklearn.ensemble import RandomForestRegressor
import xgboost as xgb
from sklearn.metrics import mean_squared_error
```
