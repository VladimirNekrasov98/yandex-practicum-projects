## Описание проекта

Из «Бета-Банка» стали уходить клиенты. Каждый месяц. Немного, но заметно. Банковские маркетологи посчитали: сохранять текущих клиентов дешевле, чем привлекать новых.

**Описание данных:**

 - RowNumber — индекс строки в данных;
 - CustomerId — уникальный идентификатор клиента;
 - Surname — фамилия;
 - CreditScore — кредитный рейтинг;
 - Geography — страна проживания;
 - Gender — пол;
 - Age — возраст;
 - Tenure — сколько лет человек является клиентом банка;
 - Balance — баланс на счёте;
 - NumOfProducts — количество продуктов банка, используемых клиентом;
 - HasCrCard — наличие кредитной карты;
 - IsActiveMember — активность клиента;
 - EstimatedSalary — предполагаемая зарплата;
 - Exited — факт ухода клиента.

## Цель и задачи проекта

Целью данной работы является нахождение и обучение модели со значением метрики F1 > 0.59 для решения задачи бинарной классификации - прогноза ухода клиента из банка.
Для её реализации необходимо выполнить следующие шаги:

- [x] Ознакомиться с данными для обучения и проанализировать их;
- [x] Провести предварительную подготовку данных для дальнейшего обучения;
- [x] Определить лучшие параметры модели по валидационной выборке;
- [x] Изучить влияние сбалансированных и несбалансированных данных на конечный результат моделирования.
- [x] Выбрать модель с наилучшей метрикой на тестовых данных.

## Стек технологий

`python`, `pandas`, `numpy`, `scipy`, `matplotlib`, `seaborn`, `sklearn`.

## Итоги

По результатам работы по созданию модели для предсказания ухода клиентов банка можно сделать следующие основные выводы:

- Данные клиентов были изучены и приведены к стандартному формату;
- Признаки были преобразованы и масштабированы, данные разделены на обучающую и тестовую выборки;
- Рассмотрены модели: дерево решений, случайный лес и логистическая регрессия;
- Исследованы различные способы борьбы с дисбалансом классов - стратификация и oversampling;
- Распределение значений в Exited и способы обработки и разделения данных оказывает весомое влияние на качество модели;
- Лучшие результаты (F1 > 0.6) показал случайный лес с использованием stratify при разбиении данных;
- Логистическая регрессия оказалась неэффективной для данной задачи;
- Случайный лес с макс. глубиной 15 - наилучшая модель для предсказания ухода клиентов.

## Статус проекта

Завершён.