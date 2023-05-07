# Final project
## UFC-Fight historical data from 1993 to 2021
За основу своего проекта я взял именно эту тему, потому что являюсь большим поклонником смешанных единоборств. UFC - это крупнейшая в мире промоутерская компания ММА, в которой выступают одни из самых высококлассных бойцов в этом виде спорта. По состоянию на 2020 год UFC провела более 500 мероприятий с участием бойцов в 12 различных весовых категориях. Набор данных представляет собой коллекцию из более чем 5000 боев за период с 1993 по 2019 год.

Я хотел разработать несколько моделей машинного обучения, чтобы поэкспериментировать с имеющимися данными. Цель - создать модель для прогнозирования исходов боев и посмотреть, будет ли она полезна в реальном мире.

В этом блокноте я использую следующие алгоритмы для построения модели:
* Gaussian Naive Bayes
* Logistic Regression
* Decision Tree
* KNN
* Random Forest
* Support Vector Classifier
* XGBoost

Модели с наивысшим показателем точности (с использованием k-кратной перекрестной валидации) на обучающих данных затем используются на тестовых данных.

|index|Model|Score Average|
|---|---|---|
|0|Gaussian Naive Bayes|0\.5772849102117396|
|1|Logistic Regression|0\.6422175385590021|
|2|Random Forest|0\.6303611023123218|
|3|Decision Tree|0\.5675434321775785|
|4|K-Nearest Neighbor|0\.5881167612874931|
|5|Support Vector Classifier|0\.6216417728612851|
|6|XGBoost|0\.6104395604395605|

Наконец, модели, показавшие хорошие результаты, применяются к событию UFC 259 (6 марта 2021 года), чтобы сделать прогнозы относительно победителей боев.
(https://ufc.ru/event/ufc-259?ysclid=lhd3svxqaa247913782)

Лучший результат успешно предсказал 4 из 5 боев.
