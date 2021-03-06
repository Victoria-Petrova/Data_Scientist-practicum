# [Определение потенциально популярного продукта для компании компьютерных игр.](https://github.com/Viktoriy-Petrova/-1/blob/main/Identifying_a_potentially_popular_product%20.ipynb)

## Описание проекта

Необходимо выявить определяющие успешность игры закономерности. Это позволит сделать ставку на потенциально популярный продукт и спланировать рекламные кампании.
## Описание данных
- Name — название игры
- Platform — платформа
- Year_of_Release — год выпуска
- Genre — жанр игры
- NA_sales — продажи в Северной Америке (миллионы проданных копий)
- EU_sales — продажи в Европе (миллионы проданных копий)
- JP_sales — продажи в Японии (миллионы проданных копий)
- Other_sales — продажи в других странах (миллионы проданных копий)
- Critic_Score — оценка критиков (максимум 100)
- User_Score — оценка пользователей (максимум 10)
- Rating — рейтинг от организации ESRB (англ. Entertainment Software Rating Board). Эта ассоциация определяет рейтинг компьютерных игр и присваивает им подходящую возрастную категорию.

## Структура проекта
1. Изучение общей информации:
	- 1.1.  Загрузка библиотек, изученеие файлов с данными, получение общей информации.
2. Подготовка данных
	- 2.1.  Обработаем дубликаты.
	- 2.2. Приведем названия столбцов к нижнему регистру.
	- 2.3. Обработаем пропуски.
	- 2.4. Заменим тип данных.
	- 2.5. Посчитаем суммарные продажи во всех регионах и запишем их в отдельный столбец.
3. Исследовательский анализ данных
	- 3.1. Построим график кол-ва выпущенных игр по годам.
	- 3.2. Узнаем, как менялись продажи по платформам и выберем платформы с наибольшими суммарными продажами.
	- 3.3. Определим какие платформы лидируют по продажам и выберем несколько потенциально прибыльных платформ.
	- 3.4. Построим график по глобальным продажам игр в разбивке по платформам.
	- 3.5. Посмотрим, как влияют на продажи внутри одной популярной платформы отзывы пользователей и критиков.
	- 3.6. Посмотрим на общее распределение игр и суммы продаж по жанрам.
4. Портрет пользователя каждого региона (NA, EU, JP)
	- 4.1. Самые популярные платформы (топ-5).
	- 4.2. Самые популярные жанры (топ-5).
	- 4.3. Определим влияние рейтинга ESRB на продажи в отдельном регионе.
5. Проверка гипотез
	- 5.1. Проверка гипотезы: Средние пользовательские рейтинги платформ Xbox One и PC одинаковые.
	- 5.2. Проверка гипотезы: Средние пользовательские рейтинги жанров Action и Sports разные.
6. Общий вывод
	- 6.1. Формулировка общего вывода.

## Используемые библиотеки и модули
`matplotlib` `numpy` `pandas` `seaborn` `scipy`
