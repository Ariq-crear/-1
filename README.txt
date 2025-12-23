README - Машинное обучение: Bank Marketing

Проект: Анализ банковского датасета 

Участники:
- Кульмагамбетов Бий 
- Испанов Ермек

Дата: 2025

------------------------------------------
1. Цель проекта

- Линейная регрессия: предсказание баланса клиента (balance)
- Классификация: предсказание депозита (deposit)
- Сравнение логистической регрессии с нуля и Random Forest
- Проведение экспериментов с learning rate, epochs и визуализация результатов
- Интерактивный интерфейс для Colab

------------------------------------------
2. Датасет

Источник: Kaggle
Ссылка: https://www.kaggle.com/datasets/janiobachmann/bank-marketing-dataset?resource=download&select=bank.csv
Описание:
- Количество строк: 45211
- Признаки (17): age, job, marital, education, default, balance, housing, loan, contact, day, month, duration, campaign, pdays, previous, poutcome, deposit
- Целевая переменная для регрессии: balance
- Целевая переменная для классификации: deposit

------------------------------------------
3. Структура проекта

- notebook.ipynb / colab: содержит все реализации моделей, эксперименты и интерфейс
- README.txt: инструкция по запуску
- requirements.txt: список необходимых библиотек

------------------------------------------
4. Модели и реализации

1. Linear Regression (с нуля, numpy)
   - Batch Gradient Descent
   - MSE
   - Влияние learning rate и epochs
   - График сходимости и scatter plot с линией регрессии

2. Logistic Regression (с нуля, numpy)
   - Сигмоида
   - Log Loss
   - Batch Gradient Descent
   - Метрики: Accuracy, Precision, Recall, F1-score, ROC AUC
   - Confusion Matrix
   - Влияние learning rate и epochs

3. Random Forest (sklearn)
   - n_estimators=100, max_depth=5
   - Метрики: Accuracy, Precision, Recall, F1-score, ROC AUC
   - Confusion Matrix

------------------------------------------
5. Интерактивный интерфейс (Colab)

- Выбор модели: Linear Regression / Logistic Regression / Random Forest
- Настройка learning rate и epochs для регрессий
- Автоматическая генерация графиков потерь и метрик
- Confusion matrix для классификации
- Сравнение LogReg и Random Forest в интерактивном режиме

------------------------------------------
6. Установка и запуск

1. Клонировать репозиторий:
   git clone <ссылка на GitHub>

2. Установить зависимости:
   pip install -r requirements.txt

3. Открыть notebook.ipynb в Google Colab

4. Запустить ячейки по порядку

------------------------------------------
7. Требуемые библиотеки

- numpy
- pandas
- matplotlib
- sklearn
- ipywidgets
- seaborn (опционально)

------------------------------------------
8. Особенности реализации

- Линейная и логистическая регрессии реализованы с нуля (без sklearn)
- Random Forest использован для сравнения
- Метрики считаются с использованием sklearn (разрешено ТЗ)
- Эксперименты с learning rate и epochs показаны в интерактивном интерфейсе
- Интерфейс полностью рабочий в Google Colab