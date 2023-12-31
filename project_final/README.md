# Дипломный проект на тему «Модель прогнозирования стоимости жилья для агентства недвижимости»
<img src="data/dom.jpg" width=50% height=50%>

## Оглавление
[1. Описание проекта](#описание-проекта)  

[2. Какой кейс решаем?](#Какой-кейс-решаем)

[3. Краткая информация о данных](#Краткая-информация-о-данных)

[4. Этапы работы над проектом](#Этапы-работы-над-проектом)

[5. Результаты](#Результаты)


### Описание проекта

Построение моделей прогнозирования стоимости жилья, поиск наилучшей модели. Запуск лучшей модели в Docker. 

<br>

### Какой кейс решаем?

Необходимо построить оптимальную модель прогнозирования с возможностью использования в продакшене - в контейнере Docker.

<br>

Задачи проекта:

1. Провести разведывательный анализ и очистку исходных данных.

2. Выделить наиболее значимые факторы, влияющие на стоимость недвижимости.

3. Построить модель для прогнозирования стоимости недвижимости.

4. Разработать небольшой веб-сервис, на вход которому поступают данные о некоторой выставленной на продажу недвижимости, а сервис прогнозирует его стоимость.


:arrow_up:[к оглавлению](#Оглавление)

<br>

### Краткая информация о данных

В данном проекте данные представлены в виде датасета размером свыше 377 тыс. строк, присутствуют дублирующиеся категории, ошибки ввода, жаргонные сокращения и т .д.. 

<br>

:arrow_up:[к оглавлению](#Оглавление)

<br>

### Этапы работы над проектом
- Знакомство с данными;
- Изучение датасета на предмет наличия пропусков и типов данных;
- Обработка данных;
- Отбор значемых признаков;
- Нормализация числовых признаков;
- Кодировка категориальных признаков;
- Построение моделей с использованием подбора гиперпараметров. (Baseline(LR), Best features(LR), DecisionTreeRegressor, DecisionTreeRegressor(optimal), ElasticNetCV(optimal), RandomForestRegressor, RandomForestRegressor(best), GradientBoostingRegressor, CatBoostRegressor(Optimal))
- Подготовлен сервер с сериализованной моделью и докер.

<br>

### Результаты:

В результате выполнения проекта построена модель CatBoostRegressor, оптимально подходящая под решение поставленной задачи.

<br>

:arrow_up:[к оглавлению](#Оглавление)

<br>

Если информация по этому проекту покажется вам интересной или полезной, то я буду очень вам благодарен, если отметите репозиторий и профиль ⭐️⭐️⭐️.