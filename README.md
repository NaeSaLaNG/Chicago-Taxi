# Проект по Прогнозированию Количества Такси в Чикаго

## Введение

В современном мире такси стало неотъемлемой частью повседневной жизни. Оно предоставляет удобный и доступный способ перемещения по городу, и его спрос подвержен различным внешним и внутренним факторам. Прогнозирование количества такси, необходимого для удовлетворения спроса, играет важную роль в обеспечении качественных услуг клиентам и оптимизации бизнес-процессов такси-компаний.

## Цель проекта

Цель нашего проекта заключается в разработке модели прогнозирования количества заказов такси в городе Чикаго. Мы стремимся предсказывать спрос на такси с высокой точностью, основываясь на исторических данных. Нашей целью также является оптимизация управления ресурсами такси-компаний и повышение уровня обслуживания клиентов.

## Описание данных

Данные для проекта были получены из открытого источника в интернете и содержат информацию о заказах такси в городе Чикаго. Набор данных включает в себя следующие столбцы:

| Column Name                | Description                                                                | Type        |
| -------------------------- | -------------------------------------------------------------------------- | ----------- |
| Trip ID                    | A unique identifier for the trip.                                          | Plain Text  |
| Taxi ID                    | A unique identifier for the taxi.                                          | Plain Text  |
| Trip Start Timestamp       | When the trip started, rounded to the nearest 15 minutes.                  | Date & Time |
| Trip End Timestamp         | When the trip ended, rounded to the nearest 15 minutes.                    | Date & Time |
| Trip Seconds               | Time of the trip in seconds.                                               | Number      |
| Trip Miles                 | Distance of the trip in miles.                                             | Number      |
| Pickup Census Tract        | The Census Tract where the trip began.                                     | Plain Text  |
| Dropoff Census Tract       | The Census Tract where the trip ended.                                     | Plain Text  |
| Pickup Community Area      | The Community Area where the trip began.                                   | Number      |
| Dropoff Community Area     | The Community Area where the trip ended.                                   | Number      |
| Fare                       | The fare for the trip.                                                     | Number      |
| Tips                       | The tip for the trip. Cash tips generally will not be recorded.            | Number      |
| Tolls                      | The tolls for the trip.                                                    | Number      |
| Extras                     | Extra charges for the trip.                                                | Number      |
| Trip Total                 | Total cost of the trip, the total of the previous columns.                 | Number      |
| Payment Type               | Type of payment for the trip.                                              | Plain Text  |
| Company                    | The taxi company.                                                          | Plain Text  |
| Pickup Centroid Latitude   | The latitude of the center of the pickup census tract or community area.   | Number      |
| Pickup Centroid Longitude  | The longitude of the center of the pickup census tract or community area.  | Number      |
| Pickup Centroid Location   | The location of the center of the pickup census tract or community area.   | Point       |
| Dropoff Centroid Latitude  | The latitude of the center of the dropoff census tract or community area.  | Number      |
| Dropoff Centroid Longitude | The longitude of the center of the dropoff census tract or community area. | Number      |
| Dropoff Centroid Location  | The location of the center of the dropoff census tract or community area.  | Point       |

Эти данные позволяют нам анализировать и предсказывать паттерны в спросе на такси в разные моменты времени и в разных районах города Чикаго.

Прогнозирование спроса на такси является важной задачей для оптимизации бизнес-процессов такси-компаний и повышения уровня обслуживания клиентов. Данные за 2022 год доступны [здесь](https://data.cityofchicago.org/Transportation/Taxi-Trips-2022/npd7-ywjz), а данные за 2023 год - [здесь](https://data.cityofchicago.org/Transportation/Taxi-Trips-2023/e55j-2ewb).

## В ходе этого проекта были выполнены следующие шаги:

1. **Проведение анализа данных:**

   - Мы подготовили данные, обработали их и провели визуальный.
   - Идентифицировали временные паттерны, влияющие на спрос на такси.

2. **Моделирование:**

   - Подготовили данные для моделирования и разделили их на обучающую и тестовую выборки.
   - Обучили модель, оценили ее производительность.
   - Проверили модель на тестовых данных.

3. **Заключение:**
   - Наша модель способна предсказывать спрос на такси.
