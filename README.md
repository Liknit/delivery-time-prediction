# Прогнозирование времени доставки заказов

## Описание:

- Сбор и хранение данных. Подключился к базе данных MySQL и извлёк необходимые данные. Для облегчения дальнейшего анализа я сохранил эти данные в виде файла sql.csv.

- Разработка функций: Отобрал и описал соответствующие признаки для каждого заказа. Этот шаг заложил основу для построения прогнозной модели.

- Определение целевой переменной: Определил целевую переменную как «время доставки в днях», которое представляет собой разницу во времени между датой заказа и фактической датой доставки.

- Предварительная обработка данных: Применил основные методы предварительной обработки данных, включая кодирование категориальных признаков, нормализацию данных и обработку пропущенных значений. Эти шаги обеспечили готовность набора данных к моделированию.

- Тип проблемы и выбор показателя: Определил тип проблемы прогнозирования, которая представляла собой задачу регрессии, поскольку мы стремились спрогнозировать непрерывное числовое значение (время доставки). Чтобы оценить производительность модели, я выбрал среднеквадратическую ошибку (RMSE).

- Построение и оценка модели: Построил и сравнил различные алгоритмы прогнозирования, используя перекрестную проверку. Модели, которые я исследовал, включали линейные модели и древовидные модели, такие как классические деревья решений и случайный лес. Путем перекрестной проверки я оценил их производительность и определил наиболее подходящий для поставленной задачи алгоритм.

- Дизайн A/B-теста: Чтобы спланировать эксперимент, я сформулировал основную гипотезу, определил ключевые показатели для оценки и рассмотрел последствия результатов.
