## Учебный проект - Исследование объявлений о продаже квартир

### Описание проекта

У нас имеются данные сервиса Яндекс.Недвижимость - архив объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет.

Для дальнейшего построения автоматизированной системы, которая позволит отследит аномалии и мошенническую деятельность, нам на основании данных необходимо установить: 
1. Сколько обычно занимает продажа квартиры (когда можно считать, что продажи прошли очень быстро, а когда долго);
2. Какие факторы больше всего влияют на стоимость квартиры в Санкт-Петербурге и соседних населённых пунктах и стоимость квартиры в центре Санкт-Петербурга.

### Выводы исследования:

* В ходе исследования было получено, что быстрая продажа - до 45 дней, а долгая продажа более 420 дней;
* На определение рыночной стоимости квартиры больше всего влияют следующие параметры: общая площадь квартиры, число комнат, расстояние до центра, этаж квартиры, срок продажи квартиры.

### Используемые библиотеки:

* Pandas
* Matplotlib
* NumPy
* Seaborn

### Данные

Для анализа были доступны следующие данные:
* Расстояние до ближайшего аэропорта в метрах (м)
* Число балконов
* Высота потолков (м)
* Расстояние до центра города (м)
* Сколько дней было размещено объявление (от публикации до снятия)
* Дата публикации
* Этаж
* Всего этажей в доме
* Апартаменты (булев тип)
* Площадь кухни в квадратных метрах (м²)
* Цена на момент снятия с публикации
* Жилая площадь в квадратных метрах (м²)
* Название населённого пункта
* Свободная планировка (булев тип)
* Число парков в радиусе 3 км
* Расстояние до ближайшего парка (м)
* Число водоёмов в радиусе 3 км
* Расстояние до ближайшего водоёма (м)
* Число комнат
* Квартира-студия (булев тип)
* Площадь квартиры в квадратных метрах (м²)
* Число фотографий квартиры в объявлении