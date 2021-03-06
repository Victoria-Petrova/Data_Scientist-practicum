# [Выбор региона для разработки новых нефтяных скважин.]( https://github.com/Viktoriy-Petrova/Yandex.Practicum.Data_Scientist/blob/main/Project_%E2%84%964/project_04.ipynb)

## Описание проекта

Добывающей нефтекомпании необходимо решить, где бурить новую скважину.
Нам предоставлены пробы нефти в трёх регионах: в каждом 10 000 месторождений, где измерили качество нефти и объём её запасов. Нам предстоит построить модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль. Проанализируем возможную прибыль и риски техникой Bootstrap.

Шаги для выбора локации:
- В избранном регионе ищут месторождения, для каждого определяют значения признаков;
- Строят модель и оценивают объём запасов;
- Выбирают месторождения с самым высокими оценками значений. Количество месторождений зависит от бюджета компании и стоимости разработки одной скважины;
- Прибыль равна суммарной прибыли отобранных месторождений.


## Описание данных
признаки:
- id — уникальный идентификатор скважины
- f0, f1, f2 — три признака точек

целевой признак:
- product — объём запасов в скважине (тыс. баррелей).

## Структура проекта
1. Загрузка и подготовка данных:
    - 1.1. Загрузка библиотек, изучение файлов с данными, получение общей информации.
    - 1.2. Изучение коэффициентов корреляции.
2. Обучение и проверка модели:
    - 2.1. Разбиение данных на выборки.
    - 2.2. Обучение и предсказания модели на валидационной выборке.
    - 2.3. Получение среднего запаса предсказанного сырья, r2 и RMSE.
3. Подготовка к расчёту прибыли:
    - 3.1. Сохранение значений для расчётов в отдельные переменные.
    - 3.2. Рассчет достаточного объема сырья для безубыточной разработки новой скважины.
4. Расчёт прибыли и рисков :
    - 4.1. Написание функции для расчёта прибыли по выбранным скважинам и предсказаниям модели.
    - 4.2. Нахождение средней прибыли, 95%-ого доверительного интервала и риска убытков.
5. Общий вывод:
    - 5.1. Формулировка общего вывода.

## Используемые библиотеки и модули
`numpy` `pandas`  `sklearn` 
