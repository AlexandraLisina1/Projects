## Учебный проект - Проверка гипотез по увеличению выручки в интернет-магазине

### Описание проекта

Вместе с отделом маркетинга крупного интернет-магазина мы подготовили список гипотез для увеличения выручки. Приоритизируем гипотезы, запустим A/B-тест и проанализируем результаты.

**Задачи:**
* Приоритизировать гипотезы для увеличения выручки;
* Запустить A/B-тест;
* Проанализировать результаты.

**Проект состоит из двух частей**

**Часть 1 (приоритизация гипотез):**
* Применим фреймворк ICE для приоритизации гипотез. Отсортируем их по убыванию приоритета;
* Применим фреймворк RICE для приоритизации гипотез. Отсортируем их по убыванию приоритета;
* Укажем как изменилась приоритизация гипотез при применении RICE вместо ICE и объяснить почему так произошло.

**Часть 2 (анализ A/B-теста):**
* Построим график кумулятивной выручки по группам;
* Построим график кумулятивного среднего чека по группам;
* Построим график относительного изменения кумулятивного среднего чека группы B к группе A;
* Построим график кумулятивной конверсии по группам;
* Построим график относительного изменения кумулятивной конверсии группы B к группе A;
* Построим точечный график количества заказов по пользователям;
* Посчитаем 95-й и 99-й перцентили количества заказов на пользователя. Выберем границу для определения аномальных пользователей;
* Построим точечный график стоимостей заказов;
* Посчитаем 95-й и 99-й перцентили стоимости заказов. Выберем границу для определения аномальных заказов;
* Посчитаем статистическую значимость различий в конверсии между группами по «сырым» данным;
* Посчитаем статистическую значимость различий в среднем чеке заказа между группами по «сырым» данным;
* Посчитаем статистическую значимость различий в конверсии между группами по «очищенным» данным;
* Посчитаем статистическую значимость различий в среднем чеке заказа между группами по «очищенным» данным;
* Примем решение по результатам теста.

### Выводы исследования:

1. Гипотезы были приоритезированы по фреймворкам ICE и RICE. Проведен анализ результатов A/B-теста, построены графики кумулятивной выручки, среднего чека, конверсии по группам. Посчитана статистическая значимость различий конверсий и средних чеков по сырым и очищенным данным.
2. Затем были даны следующие рекомендации:
* остановить тест и признавать его успешным, зафиксировав победу группы В, если для нас важно только повышение конверсии;
* продолжить тест до установления отношения средних чеков по группам и подтверждения с помощью статистических тестов значимости в превышении среднего чека группы В над средним чеком группы А, если мы ожидали повышение среднего чека.

### Используемые библиотеки:

* Pandas
* Matplotlib
* NumPy
* Seaborn

### Данные

**Данные для первой части**

Структура hypothesis.csv:
* Краткое описание гипотезы
* Охват пользователей по 10-балльной шкале
* Влияние на пользователей по 10-балльной шкале
* Уверенность в гипотезе по 10-балльной шкале
* Затраты ресурсов на проверку гипотезы по 10-балльной шкале. Чем больше значение Efforts, тем дороже проверка гипотезы

**Данные для второй части**

Структура orders.csv:
* Идентификатор заказа
* Идентификатор пользователя, совершившего заказ
* Дата, когда был совершён заказ
* Выручка заказа
* Группа A/B-теста, в которую попал заказ

Структура visitors.csv:
* Дата
* Группа A/B-теста
* Количество пользователей в указанную дату в указанной группе A/B-теста
