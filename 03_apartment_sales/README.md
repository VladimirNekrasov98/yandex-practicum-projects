## Описание проекта

В вашем распоряжении данные сервиса Яндекс Недвижимость — архив объявлений за несколько лет о продаже квартир в Санкт-Петербурге и соседних населённых пунктах.
Ваша задача — выполнить предобработку данных и изучить их, чтобы найти интересные особенности и зависимости, которые существуют на рынке недвижимости.
Это позволит построить автоматизированную систему: она отследит аномалии и мошенническую деятельность. 

**Описание данных**

- airports_nearest — расстояние до ближайшего аэропорта в метрах (м);
- balcony — число балконов;
- ceiling_height — высота потолков (м);
- cityCenters_nearest — расстояние до центра города (м);
- days_exposition — сколько дней было размещено объявление (от публикации до снятия);
- first_day_exposition — дата публикации;
- floor — этаж;
- floors_total — всего этажей в доме;
- is_apartment — апартаменты (булев тип);
- kitchen_area — площадь кухни в квадратных метрах (м²);
- last_price — цена на момент снятия с публикации;
- living_area — жилая площадь в квадратных метрах (м²);
- locality_name — название населённого пункта;
- open_plan — свободная планировка (булев тип);
- parks_around3000 — число парков в радиусе 3 км;
- parks_nearest — расстояние до ближайшего парка (м);
- ponds_around3000 — число водоёмов в радиусе 3 км;
- ponds_nearest — расстояние до ближайшего водоёма (м);
- rooms — число комнат;
- studio — квартира-студия (булев тип);
- total_area — общая площадь квартиры в квадратных метрах (м²);
- total_images — число фотографий квартиры в объявлении.

## Цель и задачи проекта

Цель исследования - провести исследовательский анализ данных, который поможет установить параметры, влияющие на цену объектов недвижимости:

- [x] Загрузить и изучить представленные данные;
- [x] Провести предобработку данных;
- [x] Создать новые признаки из имеющихся;
- [x] Провести исследовательский анализ данных(EDA);
- [x] Сделать выводы по работе.

## Стек технологий

`python`, `pandas`, `matplotlib`.

## Итоги

По результатам анализа данных о продаже недвижимости в Санкт-Петербурге можно сделать следующие основные выводы:

- Обработаны и изучены данные: заполнены пропуски, исправлены аномалии, преобразованы типы данных, удалены дубликаты;
- Самая часто встречаемая жилая площадь порядка 17-18 и 30 м², а кухни порядка 6-10 м². Общая площадь чаще находится около 42 +- 3 м², а также часто попадается 60 м²;
- В объявлениях больше всего 1-3 комнатных квартир стоимостью порядка 3.5-4.5 млн. руб., чаще продаются квартиры до 5 этажа включительно;
- Достаточно много квартир в пяти и девятиэтажках, расположенных на достаточном удалении как от центра города, так и от аэропортов. Тем не менее, зачастую в пешей доступности находится парк;
- В будние дни публикуется больше объявлений, чем в выходные. Больше всего объявлений публикуется с февраля по апрель, меньше всего объявлений в январе, декабре и мае;
- Чаще всего квартиры продаются за 45 или 60 дней, при этом более половины квартир продаются в первые 100 дней после появления объявления. Менее удачными можно считать объявления, которые продавались более 200 дней;
- Прямое влияние на стоимость квартиры больше всего оказывают следующие параметры(у в порядке убывания влияния): общая площадь, жилая площадь, площадь кухни, количество комнат. Остальные переменные влияния не оказывают или оно нелинейно;
- Наибольшей выгодой обладают объявления о продаже квартиры на первом или последнем этаже за 2017 год. Также лучше рассматривать предложения, опубликованные с пятницы по воскресенье в мае или июле;
- Максимальная удельная стоимость квадратного метра в Зеленогорске, минимальная - в Старополье;
- Чем дальше квартира находится от центра Санкт-Петербурга, тем меньше она будет стоить, пороговое значение - 8 км.

## Статус проекта

Завершён.