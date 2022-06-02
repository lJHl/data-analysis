# Анализ поведения пользователей мобильного приложения по продаже продуктов питания

![python](https://img.shields.io/pypi/pyversions/pandas)
![pandas](https://img.shields.io/pypi/v/pandas?label=pandas)
![numpy](https://img.shields.io/pypi/v/numpy?label=NumPy)
![matplotlib](https://img.shields.io/pypi/v/matplotlib?label=matplotlib)
![seaborn](https://img.shields.io/pypi/v/seaborn?label=seaborn)
![plotly](https://img.shields.io/pypi/v/plotly?label=plotly)
![scipy](https://img.shields.io/pypi/v/scipy?label=SciPy)

**В данном проекте используются интерактивные графики,** [ссылка на nbviewer для просмотра](https://nbviewer.org/github/lJHl/data-analysis/blob/e96b89f8664b2bf0c557939f030358c85310572e/food_app_project/food_app_analysis_project.ipynb)

---

## Цель проекта

Изучить воронку продаж, а так же исследовать результаты A/A/B-эксперимента по изменению шрифта во всём приложении.

## Данные 

*В качестве входных данных используются логи мобильного приложения.*

## Общий вывод

**По результатам изучения воронки продаж, а так же результатов A/A/B-эксперимента по изменению шрифта во всём приложении, можно сделать вывод:**

- Представленные данные имеют актуальный период с 1 августа, а не с 25 июля;
- Инструкцией к приложению пользуются всего 11% пользователей, но 98% остается даже не изучив ее, значит в приложении хороший и понятный интерфейс;
- Больше всего просадка на моменте показа экрана с товаром, скорее всего это те кто решил просто из интереса попользоваться приложением, либо же пользователя не удовлетворил представленный ассортимент или стоимость товара;
- 95% из тех кто добавил товар в корзину, оплатили его, а это значит система оплаты и ее наглядность на очень хорошем уровне;
- Доля пользователей, которые доходят от первого события до оплаты составляет 47%;
- Статистические критерии разницу между контрольными группами не находят, группы были разделены корректно;
- Самым популярным событием во всех группах является показ основного экрана;
- Статистической разницы между контрольными, а так же объединенной контрольной и экспериментальной (с измененным шрифтом) не выявлено по всем событиям.

**Исходя из этого всего: изменение шрифта никак не скажется на поведение пользователей, можно его поменять на радость дизайнерам, либо же оставить как есть.**