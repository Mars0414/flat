# Прогнозирование цен на недвижимость / Real Estate Price Prediction

## Описание / Description

**RU:**  
Этот проект направлен на построение модели машинного обучения для предсказания стоимости объектов недвижимости в Бишкеке на основе различных характеристик квартир.

**EN:**  
This project aims to build a machine learning model to predict real estate prices in Bishkek based on various apartment features.

---

## Структура проекта / Project Structure

- `flat.ipynb` — Jupyter-ноутбук с анализом, визуализацией и обучением модели  
- Notebook contains: data cleaning, feature visualization, model training (CatBoost), and evaluation.

---

## Используемые библиотеки / Libraries Used

| Библиотека / Library | Назначение / Purpose        |
|----------------------|-----------------------------|
| `pandas`             | таблицы / data manipulation |
| `numpy`              | численные операции / math   |
| `matplotlib`, `seaborn` | визуализация / visualization |
| `catboost`           | ML-модель / ML model        |
| `sklearn`            | метрики / metrics           |

---

## Этапы / Steps

### 1. Анализ данных / Data Analysis
- Пропуски / Missing values
- Распределения / Distributions
- Выбросы / Outliers

### 2. Предобработка / Preprocessing
- Кодирование категориальных признаков / Categorical encoding
- Масштабирование / Feature scaling

### 3. Модель / Model
- `CatBoostRegressor`
- Признаки / Features: `square`, `rooms_num`, `condition`, `floor`, etc.
- Целевая / Target: `price_per_sq`

### 4. Оценка / Evaluation

| Метрика / Metric | Значение / Example |
|------------------|---------------------|
| MAPE             | 19.8 %              |
| MAE              | 24,600              |
| R²               | 0.71                |

---

## Запуск / How to Run

```bash
pip install pandas numpy matplotlib seaborn catboost scikit-learn
