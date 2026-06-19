# House Price Prediction

ML проект на классических алгоритмах: предсказание цен на жильё по датасету Ames Housing (Kaggle).
## Описание

Полный пайплайн: разведочный анализ данных (EDA), обработка пропусков, кодирование категориальных признаков, обучение и подбор гиперпараметров для нескольких моделей регрессии.
## Результаты

| Модель | RMSE (log price) |
|---|---|
| Linear Regression | 0.130 |
| Random Forest | 0.145 |
| Ridge | 0.1245 |
| Gradient Boosting (tuned) | 0.1235 |
Финальная модель: Gradient Boosting с подбором гиперпараметров (`learning_rate=0.05`, `max_depth=3`, `n_estimators=300`).
## Структура проекта

data/raw/          — исходные данные (train.csv, test.csv)
data/processed/    — submission.csv
notebooks/         — Jupyter ноутбук с полным анализом
models/            — сохранённая обученная модель
## Датасет

[House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)

## Технологии

Python, pandas, numpy, matplotlib, seaborn, scikit-learn