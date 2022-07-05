# Анализ товарного ассортимента интернет-магазина товаров для дома и быта

![python](https://img.shields.io/pypi/pyversions/pandas)
![pandas](https://img.shields.io/pypi/v/pandas?label=pandas)
![numpy](https://img.shields.io/pypi/v/numpy?label=NumPy)
![sqlalchemy](https://img.shields.io/pypi/v/sqlalchemy?label=SQLAlchemy)
![plotly](https://img.shields.io/pypi/v/plotly?label=plotly)
![scipy](https://img.shields.io/pypi/v/scipy?label=SciPy)

**В данном проекте используются интерактивные графики:**

[Ссылка на nbviewer для проекта по анализу товарного ассортимента интернет-магазина]()

[Ссылка на nbviewer для проекта по оценке A/B-теста]()

---

## Цель проекта по анализу товарного ассортимента интернет-магазина

Проанализировать ассортимент товаров, определить какие товары входят в основной и дополнительный ассортимент, чтобы грамотно предлагать покупателям дополнительные товары и оптимизировать закупки, для этого:
- Проведем исследовательский анализ данных; 
- Проанализируем торговый ассортимент; 
- Сформулируем и проверим статистические гипотезы.

## Данные 

*В качестве входных данных используется датасет описывающий транзакции интернет-магазина товаров для дома и быта.*

[Презентация проекта](https://disk.yandex.ru/i/T6h0U-2-ByQtLw)  
[Дашборд](https://public.tableau.com/app/profile/ljhl/viz/EcommerceDashboard_16554073462910/Dashboard1)

## Общий вывод

**В результате анализа было выяснено:**

- Среднее количество товаров в заказе 2.8;
- Основной ассортимент товаров в магазине представлен категорией "Сад и огород";
- Товаров, которые покупают как отдельную единицу и тех, что предпочитают как дополнительный, в товарном ассортименте поровну;
- Весной количество товаров категории "Сад и огород" продается больше, чем в остальные сезоны;
- Во все сезоны, кроме весны, по количеству проданных товаров, лидирует категория "Товары для дома";
- Больше всего заказов делается в будние дни;
- Пик заказов приходится на промежуток с 10 до 13 часов;
- Самую большую выручку магазин сделал в последние месяцы 2018 года;
- Самый большой средний чек достигнут в январе;
- Самым продаваемым товаром оказался товар из категории "Интерьер";
- Самые дешевые товары, которые покупают по одной штуке, в категории "Сад и огород";

**Были проверены статистические гипотезы:**

- Средний чек по будням такой же, как и по выходным;
- Средний чек днем такой же, как и ночью;
- Средний чек в разные сезоны не отличается. Мы располагаем данными с 1 октября 2018 по 31 октября 2019, поэтому для проверки будут взяты только данные с 1 декабря 2018 по 31 августа 2019 (зима, весна, лето).

**Ни один тест не показал статистически значимого результата. Средний чек в разные временные промежутки не отличается.**

**Были расчитаны бизнес-показатели:**

- DAU (по месяцам)
- WAU (по месяцам)
- MAU (по месяцам)
- AOV - средний чек (по месяцам)

**На основе них было выяснено, что количество активных пользователей стабильно, но есть прирост в феврале, марте, апреле 2019 года. Средний чек, меньше всего в весенние месяцы.**

*Хотелось бы отметить, что был создан класс и метод в нем, для рекомендации дополнительного товара, но основе товаров из заказа.*

**Рекомендации:** 

- Расширить ассортимент в категории "Товары для дома", хоть и по количеству категория "Сад и огород" лидирует, но именно "Товары для дома" делают основную выручку, сопоставимую с совокупной суммой продаж в других категориях;
- Стимулировать покупателей скидками и акциями, чтобы они делали заказы в выходные и в ночное время, увеличив количество заказов в это время, увеличим и выручку;
- Делать основные закупки семян и рассады к весне, в остальное время они не пользуются популярностью;
- В августе и сентябре, традиционно сезон отпусков, предложить скидки в эти месяцы, тем самым увеличим количество заказов.

---

## Цель проекта по оценке A/B-теста
Провести оценку результатов A/B-теста. 

## Данные

*В качестве входных данных используется датасет с действиями пользователей и несколько вспомогательных датасетов.*

## Общий вывод

**По результатам воронки продаж, а так же результатам A/B-тестирования, можно сделать вывод:**

**Тест был выполнен некорректно, он не соответствует ни правилам проведения A/B-тестирования, ни техническому заданию, были выявлены следующие недостатки:**

- Аудитория для теста набрана неправильно, вместо ожидаемых 15% из EU было всего 5.6%;
- Распределение пользователей между тестами осуществленно неверно, 23% попали в конкурирующий тест;
- Разделение на контрольную и тестовую так же выполнено неверно, преобладание одной над другой;
- Количество пользователей для теста меньше чем предполагалось, из-за пересечения с конкурирующим тестом;
- Много пользователей, которые не совершили ни одного действия.
- Последнее событие было 30 декабря 2020, хотя тест предполагался до 4 января 2021;
- Ни на одном из этапов не видно увеличения конверсии на 10%.

**Рекомендации:** учесть недочеты и доработать механизм разделения на группы.

---

## Цель проекта по анализу базы данных сервиса для чтения книг

Проанализировать базу данных сервиса для чтения книг по подписке.

## Данные

**В качестве входных данных используется база данных, содержащая:**

- Информацию о книгах; 
- Издательствах; 
- Авторах; 
- Пользовательские обзоры книг.

## Необходимо

1. Сделать обзор данных;
2. Посчитать, сколько книг вышло после 1 января 2000 года;
3. Для каждой книги посчитать количество обзоров и среднюю оценку;
4. Определить издательство, которое выпустило наибольшее число книг толще 50 страниц, чтобы исключить из анализа брошюры;
5. Определить автора с самой высокой средней оценкой книг, учитывая только книги с 50 и более оценками;
6. Посчитать среднее количество обзоров от пользователей, которые поставили больше 50 оценок.

## Общий вывод

- База данных представляет из себя 5 таблиц:
  - `books` - содержит данные о книгах;
  - `authors` - содержит данные об авторах;
  - `publishers` - содержит данные об издательствах;
  - `rating` - содержит данные о пользовательских обзорах;
  - `reviews` - содержит данные о пользовательских обзорах$
- В ходе анализа были получены ответы на следующие вопросы:
  - Количество книг вышедших после 1 января 2000 года – `819`;
  - Количество обзоров и средняя оценка для каждой книги:
    1. Место – `Twilight`, количество обзоров `7`, средний рейтинг `3.66`;
    2. Место – `Harry Potter and the Prisoner of Azkaban`, количество обзоров	`6`, средний рейтинг	`4.41`;
    3. Место – `Harry Potter and the Chamber of Secrets`, количество обзоров	`6`, средний рейтинг	`4.29`;
  - Издательство, которое выпустило наибольшее число книг толще 50 страниц – `Penguin Books`;
  - Автор с самой высокой средней оценкой книг, с количеством оценок более 50 – `J.K. Rowling/Mary GrandPré`;
  - Среднее количество обзоров от пользователей, которые поставили больше 50 оценок – `24.33`. 