# Лабораторные работы по курсу "Методы, средства и технологии мультимедиа"

## Студент

|         |                            |
|---------|----------------------------|
| Группа  | М8О-406Б-21                |
| ФИО     | Медведев Кирилл Викторович |


## Датасеты

- ![MONEY](/img/header_img.jpg) В качестве датасета для задачи классификации будем использовать [Salary Prediction Classification](https://www.kaggle.com/datasets/ayessa/salary-prediction-classification/data). Датасет содержит информацию о возрасте, поле, расе, образовании, семейном положении,стране, значении заработной платы (<=50'000$ or >50'000$) и др. Будем определять <ins>больше ли 50'000$ заработная плата человека или нет</ins>.

- ![POSSUM](/img/header_img2.jpg) В качестве датасета для задачи регрессии будем использовать [Possum Regression](https://www.kaggle.com/datasets/abrambeyer/openintro-possum/data). Датасет содержит информацию о породе, поле, длине тела, длине хвоста, размере головы, размере лап и возрасте и др. Будем определять <ins>возраст опоссума</ins>.


## Метрики

Для оценки обученных моделей, решающих задачу классификации, будем использовать следующие метрики:

| Метрика     |         Описание                                          |
|-------------|-----------------------------------------------------------|
| Accuracy    | Доля правильных предсказаний от общего числа предсказаний |
| Precision   | Отношение верно положительных предсказаний ко всем положительным предсказаниям |
| Recall      | Отношение верно положительных предсказаний к числу всех настоящих положительных примеров |
| F1-Score    | Гармоническое среднее между Precision и Recall |