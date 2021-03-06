# Изучение закономерностей, определяющих успешность игр

![python](https://img.shields.io/pypi/pyversions/pandas)
![pandas](https://img.shields.io/pypi/v/pandas?label=pandas)
![numpy](https://img.shields.io/pypi/v/numpy?label=NumPy)
![matplotlib](https://img.shields.io/pypi/v/matplotlib?label=matplotlib)
![seaborn](https://img.shields.io/pypi/v/seaborn?label=seaborn)
![scipy](https://img.shields.io/pypi/v/scipy?label=SciPy)

## Цель проекта

Выявить определяющие успешность игры закономерности, чтобы сделать ставку на потенциально популярный продукт и спланировать рекламные кампании. Для этого:

- Проведем исследовательский анализ данных;
- Составим портерет пользователя каждого региона;
- Проверим гипотезы:
    1. Средние пользовательские рейтинги платформ Xbox One и PC одинаковые;
    2. Средние пользовательские рейтинги жанров Action (англ. «действие», экшен-игры) и Sports (англ. «спортивные соревнования») разные.


## Данные 

**В качестве входных данных используются исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы полученные из открытых источников за 2016.**

> **Примечание:**  
>В наборе данных попадается аббревиатура ESRB (Entertainment Software Rating Board) — это ассоциация, определяющая возрастной рейтинг компьютерных игр. ESRB оценивает игровой контент и присваивает ему подходящую возрастную категорию, например, «Для взрослых», «Для детей младшего возраста» или «Для подростков».


## Общий вывод

**По результатам исследования рынка игр было выявлено:**

- Подъем выпуска игр начинается с 1992 года и достигает пика в 2009, после идет спад и момент стабилизации с 2013;
- В качестве актуального периода был выбран промежуток с 2013 по 2016 года;
- Характерный средний срок жизни платформы 9.5 лет;
- Самыми прибыльными оказались PS4, PS3, Xbox One, 3DS, X360, подкачали продажи у PC;
- Рост наблюдался только у PS4 и Xbox One, так как это самые новые консоли в представленном наборе данных, но в 2016 году они так же показали снижение, все остальные платформы падают от года к году;
- В качестве потенциально прибыльных платформ были выбраны PS4, Xbox One, 3DS, WiiU, PC, они являются самыми актуальными на 2016 год, у остальных платформ заканчивается срок поддержки;
- Зависимость продаж от оценки пользователей у потенциально прибыльных платформ либо отстутствовала, либо была очень слабой положительной, как у WiiU;
- Зависимость продаж от оценки критиков у 3DS и PC очень слабая положительная, WiiU, Xbox One имеют слабую зависимость как и PS4;
- У PS4, как у самой прибыльной из выбранных, больше всего продаж в жанрах Platform, Shooter и Sports, меньше всего игр с жанром Puzzle. У симуляторов среднее и медиана продаж практически одинаковые.

**Составление портрета пользователя для Северной Америки показал:**

- Самые популярные платформы это PS4, Xbox One, X360, PS3, 3DS;
- Большую долю рынка занимают самые новые консоли PS4, Xbox One, не отстает и консоль прошлого поколения X360;
- На продажи для X360 и Xbox One в Северной Америке приходится больше половины от мировых продаж;
- Самые популярные жанры - это action, shooter, sports, rpg, misc, это объясняется тем что в данные жанры удобно играть на консоле через геймпад, популярные платформы это подтверждают.

**Составление портрета пользователя для Европы показал:**

- Самые популярные платформы - это PS4, PS3, Xbox One, X360, 3DS;
- PS4 занимет целых 42.2% рынка Европы, за ним идет PS3 и уже потом все остальные;
- Продажи игр под PS4 в Европе занимают 45% от мировых, затем рынок почти поровну разделили остальные платформы;
- Самые популярные жанры - это action, shooter, sports, rpg, racing, это объясняется так же как и в Северной Америке, тем что в данные жанры удобно играть на консоле через геймпад.

**Составление портрета пользователя для Японии показал:**

- Самые популярные в Японии оказались отечественные платформы 3DS, PS3, PSV, PS4, WiiU;
- Портативная консоль 3DS занимает половину рынка, остальные платформы делять рынок практически в равных долях;
- Так как 3DS самая популярная платформа в Японии, на нее приходится половина от мировых продаж игр под нее, следом с еще большим размахом идет psv;
- Самые популярные жанры в JP это rpg, action, misc, fighting, shooter, во все эти жанры удобно играть на портативных консолях, которые так популярны в Японии.

*Рейтинг ESRB скорее не влияет чем влияет, больше всего продаж игр с рейтингом M - Mature, но так как игры в жанре action и shooter чаще всего получают именно его, то в этом нет ничего удивительного.*

**Проверка гипотез выявила, что:**

- Средние пользовательские рейтинги платформ Xbox One и PC одинаковые;
- Средние пользовательские рейтинги жанров Action и Sports разные.

**Исходя из всего выше перечиленного можно сделать вывод:** 

1. Если планировать рекламную кампанию всего под одну платформу, то во всех регионах это будет PS4;
2. Если планирвоать кампании под разные регионы: 
 - В Северной Америке нужно сделать акцент на PS4 и Xbox One, так как это самые актуальные платформы на текущий момент, консоли предыдущего поколения со временем будут отходить№
 - В Европе акцентировать нужно на тоже, что и в Северной Америке;
 - В Японии кроме популярной PS4, нужно акцентировать так же и на портативные платформы 3DS и PSV.
3. В Качестве жанров во всех случаях нужно выбрать action, shooter, rpg.

**Так же хотелось бы отметить что в представленном наборе данных были пропуски и неправильные типы данных, большинство этих проблем удалось решить. Причины их появления скорее всего ошибка выгрузки или сбора данных.**