# [Рекомендация тарифов.](https://github.com/Viktoriy-Petrova/Yandex.Practicum.Data_Scientist/blob/main/Project_%E2%84%962/project_%E2%84%962.ipynb)
## Описание проекта

Необходимо построить модель для задачи классификации, которая выберет подходящий тариф. В нашем распоряжении данные о поведении клиентов, которые уже перешли на эти тарифы.

## Описание данных
- сalls — количество звонков,
- minutes — суммарная длительность звонков в минутах,
- messages — количество sms-сообщений,
- mb_used — израсходованный интернет-трафик в Мб,
- is_ultra — каким тарифом пользовался в течение месяца («Ультра» — 1, «Смарт» — 0).

## Структура проекта
1. Изучение общей информации:
	- 1.1. Загрузка библиотек, изученеие файлов с данными, получение общей информации.
	- 1.2. Подготовка данных.
2. Разбиение данных на выборки:
	- 2.1. Извлеченние в отдельные переменные признаки и целевой признак.
	- 2.2. Разделение набора данных на обучающую, валидационную, и тестовую выборку.
3. Исследование моделей:
	- 3.1. Оценим качество трех моделей по умолчанию.
	- 3.2. Оценим качество моделей на тренировочной выборке.
	- 3.3. Улучшим модели.
		- Случайный лес (RandomForestClassifier).
		- Дерево решений (DecisionTreeClassifier).
		- Логистическая регрессия (LogisticRegression).
	- 3.4. Добавим получившиеся метрики в таблицу modl, и выберем лучшую модель.
4. Проверка модели на тестовой выборке:
	- 4.1. Объединим тренировачную и валидационную выборки.
	- 4.2. Обучим модель на полных данных.
	- 4.3. Получим предсказания и посчитаем качество модели на тестовой выборке.
5. Проверка модели на адекватность:
	- 5.1. Создадим константную модель.
	- 5.2. Сравним показатель точности константной модели и финальной.
6. Общий вывод:
	- 6.1. Формулировка общего вывода.

## Используемые библиотеки и модули
`numpy` `pandas` `seaborn` `sklearn`
