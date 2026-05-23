# Прогнозирование заказов такси

Учебный проект: по историческим данным о заказах такси в аэропортах построить модель, предсказывающую число заказов на следующий час.

## Установка

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Запуск

```bash
jupyter notebook taxi_forecast.ipynb
```

Либо выполнить целиком из консоли:

```bash
jupyter nbconvert --to notebook --execute taxi_forecast.ipynb
```

## Результат

Лучшая модель по валидации - LightGBM с параметрами `learning_rate=0.05, n_estimators=200, max_depth=10`. RMSE на тестовой выборке: 40.6.
