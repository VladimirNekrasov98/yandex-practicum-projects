## Описание проекта

Оператор мобильной связи «Мегалайн» выяснил: многие клиенты пользуются архивными тарифами. Они хотят построить систему, способную проанализировать поведение клиентов и предложить пользователям новый тариф: «Смарт» или «Ультра».

**Описание данных**

- сalls — количество звонков;
- minutes — суммарная длительность звонков в минутах;
- messages — количество sms-сообщений;
- mb_used — израсходованный интернет-трафик в Мб;
- is_ultra — каким тарифом пользовался в течение месяца («Ультра» — 1, «Смарт» — 0).

## Цель и задачи проекта

Целью данной работы является подбор модели с accuracy > 0.75, а также её параметров для решения задачи бинарной классификации - подбора одного из двух тарифов для пользователей на основе информации о звонках. 
Для этого необходимо:

- [x] Загрузить данные и изучить их;
- [x] Подготовить исходную выборку для дальнейшего обучения и проверки точности модели на валидационных и тестовых данных;
- [x] Провести подбор гиперпараметров модели с целью нахождения модели с максимальной точностью;
- [x] Выбрать модель с максимальной точностью на тестовых данных.

## Стек технологий

`python`, `pandas`, `matplotlib`, `seaborn`, `scipy`, `tqdm`, `sklearn`.

## Итоги

По результатам работы по сравнению моделей для решения задачи бинарной классификации можно сделать следующие основные выводы:

- Проведен анализ входных данных, выделены обучающая, валидационная и тестовая выборки;
- Рассмотрены модели: дерево решений, случайный лес и логистическая регрессия;
- Для подбора гиперпараметров использовались перебор в цикле и функции рандомизированного и сеточного поиска. Перебор эффективен для 1-2 параметров, в ином случае лучше рандомизированный поиск;
- Лучшие результаты показали случайный лес и дерево решений (accuracy > 0.79);
- Случайный лес с 27 деревьями и макс. глубиной 7 превзошёл остальные модели;
- Для дерева решений оптимальная макс. глубина - 4;
- Логистическая регрессия показала наименьшую точность (accuracy < 0.75);
- Все модели прошли валидацию и превзошли базовую модель.

## Статус проекта

Завершён.