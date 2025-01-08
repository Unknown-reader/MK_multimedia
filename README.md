# Лабораторные работы по курсу "Методы, средства и технологии мультимедиа"

## Студент

|             |                            |
|-------------|----------------------------|
| **Группа**  | М8О-406Б-21                |
| **ФИО**     | Медведев Кирилл Викторович |


## Датасеты

- ![MONEY](/img/header_img.jpg) В качестве датасета для задачи классификации будем использовать [Salary Prediction Classification](https://www.kaggle.com/datasets/ayessa/salary-prediction-classification/data), содержащем данные 1994 года. Датасет содержит информацию о возрасте, поле, расе, образовании, семейном положении, происхождении, значении заработной платы (<=50'000$ or >50'000$ в год) и др. Будем определять <ins>больше ли 50'000$ заработная плата человека или нет</ins>. <br /> **Обоснование:** Социо-научное изыскание для отслеживания факторов, влияющих на финансовый успех в экономически-развитом обществе на стыке веков.

<br />

- ![BUILDING](/img/header_img2.jpg) В качестве датасета для задачи регрессии будем использовать [Energy Efficiency Dataset](https://www.kaggle.com/datasets/elikplim/eergy-efficiency-dataset/data). Датасет содержит информацию о параметрах зданий: площади, высоте, ориентации, энергетических потребностях. Будем определять значения <ins>нагрузки на отопление и охлаждение</ins>. <br /> **Обоснование:** Предсказание энергетических потребностей здания по его характеристикам.


## Метрики

Для оценки обученных моделей, решающих <ins>задачу классификации</ins>, будем использовать следующие метрики:

| Метрика     |         Описание                                          |
|-------------|-----------------------------------------------------------|
| Accuracy    | Доля правильных предсказаний от общего числа предсказаний |
| Precision   | Отношение верно положительных предсказаний ко всем положительным предсказаниям |
| Recall      | Отношение верно положительных предсказаний к числу всех настоящих положительных примеров |
| F1-Score    | Гармоническое среднее между Precision и Recall |

<br />
<br />

Для оценки обученных моделей, решающих <ins>задачу регрессии</ins>, будем использовать следующие метрики:

| Метрика     |         Описание                                          |
|-------------|-----------------------------------------------------------|
| MAE         | Среднее абсолютное отклонение предсказанных значений от фактических |
| R^2         | Метрика, отражающая насколько хорошо модель объясняет вариацию в целевой переменной |


## Результаты

### ЛР 1 (KNN)

| Задача      | Модель   | Accuracy | Precision | Recall | F1-Score | MAE | R^2 |
|-------------|----------|----------|-----------|--------|----------|--|--|
|Классификация| Бейзлайн            | 0.84204 | 0.6866 | 0.6335 | 0.6590 |  |  |
|             | Улучшенный бейзлайн | 0.8191 | 0.5805 | 0.8996 | 0.7056 |  |  |
|             | Самостоятельная имплементация | 0.8155 | 0.5731 | 0.9179 | 0.7056 |  |  |
|Регрессия    | Бейзлайн            |  |  |  |  | 1.6515 | 0.9464 |
|             | Улучшенный бейзлайн |  |  |  |  | 1.5880 | 0.9561 |
|             | Самостоятельная имплементация |  |  |  |  | 1.5606 | 0.9569 |
<br />
<br />

### ЛР 2 (Линейные модели)

| Задача      | Модель   | Accuracy | Precision | Recall | F1-Score | MAE | R^2 |
|-------------|----------|----------|-----------|--------|----------|--|--|
|Классификация| Бейзлайн            | 0.7946 | 0.6423 | 0.3329 | 0.4385 |  |  |
|             | Улучшенный бейзлайн | 0.7045 | 0.4393 | 0.8193 | 0.5719 |  |  |
|             | Самостоятельная имплементация | 0.7402 | 0.4699 | 0.6126 | 0.5319 |  |  |
|Регрессия    | Бейзлайн            |  |  |  |  | 2.2066 | 0.8994 |
|             | Улучшенный бейзлайн |  |  |  |  | 1.2047 | 0.9723 |
|             | Самостоятельная имплементация |  |  |  |  | 3.9283 | 0.6715 |
<br />
<br />

### ЛР 3 (Решающее дерево)

| Задача      | Модель   | Accuracy | Precision | Recall | F1-Score | MAE | R^2 |
|-------------|----------|----------|-----------|--------|----------|--|--|
|Классификация| Бейзлайн            | 0.8202 | 0.6290 | 0.6186 | 0.6237 |  |  |
|             | Улучшенный бейзлайн | 0.8590 | 0.6539 | 0.8813 | 0.7508 |  |  |
|             | Самостоятельная имплементация | 0.7863 | 0.5344 | 0.8771 | 0.6641 |  |  |
|Регрессия    | Бейзлайн            |  |  |  |  | 0.7462 | 0.9744 |
|             | Улучшенный бейзлайн |  |  |  |  | 0.8340 | 0.9752 |
|             | Самостоятельная имплементация |  |  |  |  | 1.0218 | 0.9728 |
<br />
<br />

### ЛР 4 (Случайный лес)

| Задача      | Модель   | Accuracy | Precision | Recall | F1-Score | MAE | R^2 |
|-------------|----------|----------|-----------|--------|----------|--|--|
|Классификация| Бейзлайн            | 0.8519 | 0.7217 | 0.6275 | 0.6713 |  |  |
|             | Улучшенный бейзлайн | 0.8686 | 0.6714 | 0.8907 | 0.7657 |  |  |
|             | Самостоятельная имплементация | 0.8440 | 0.6955 | 0.6275 | 0.6598 |  |  |
|Регрессия    | Бейзлайн            |  |  |  |  | 0.7099 | 0.9811 |
|             | Улучшенный бейзлайн |  |  |  |  | 0.6953 | 0.9844 |
|             | Самостоятельная имплементация |  |  |  |  | 0.7668 | 0.9793 |
<br />
<br />

### ЛР 5 (Градиентный бустинг)

| Задача      | Модель   | Accuracy | Precision | Recall | F1-Score | MAE | R^2 |
|-------------|----------|----------|-----------|--------|----------|--|--|
|Классификация| Бейзлайн            | 0.8700 | 0.8033 | 0.6096 | 0.6932 |  |  |
|             | Улучшенный бейзлайн | 0.8631 | 0.6689 | 0.85744 | 0.7515 |  |  |
|             | Самостоятельная имплементация | 0.8244 | 0.9650 | 0.2814 | 0.4358 |  |  |
|Регрессия    | Бейзлайн            |  |  |  |  |  |  |
|             | Улучшенный бейзлайн |  |  |  |  |  |  |
|             | Самостоятельная имплементация |  |  |  |  |  |  |