Приведенный набор данных представляет из себя описание астероидов. Каждый астероид имееет метку "опасности": "опасен", "не опасен". Таким образом, данная задача представляет из себя задачу бинарной классификации. Весь набор данных находиться в файле `neo.csv`.

### Признаки:
`id`: уникальные идентификатор астероида;
`name`: наименование астероида, выданное NASA;
`est_diameter_min`: минимальный наблюдаемый диаметр в километрах;
`est_diameter_max`: максимальный наблюдаемый диаметр в километрах;
`relative_velocity`: скорость относительно Земли;
`miss_distance`: расстояние в километрах;
`orbiting_body`: планета, вокруг которой вращается астероид
`sentry_object`: входит в состав sentry - автоматизированной системы мониторинга столкновений;
`absolute_magnitude`: светимость;
`hazardous`: целевая переменная - описывает опасен астероид или нет.



Доп. файлы:
* train.csv - обучающая выборка, после предварительного анализа и предварительной обрабатки данных. Выборка включает в себя целевую переменную;
* test.csv - тестовая выборка, после предварительного анализа и предварительной обрабатки данных. Выборка включает в себя целевую переменную;
* cat_boost_model.pickle - обученная модель CatBoostVlassifier;
* X_test_save.parquet.gzip - результат скоринга модели, сохраненный в формате parquet и заархивированный.