# Прогнозирование уровня сложности фильмов на английском.

**Цель работы**: разработать модель для прогнозирования уровня сложности фильмов на английском языке на основе файлов с субтитрами.

**Ход работы:**

- Сбор данные: Фильмы и их оценки уровня сложности представлены в файле "movies_labels.xlsx". Каждые субтитры представлены в отдельных файлах в формате SRT. Необходимо объединить данные в один датафрейм для последующего анализа.

- Предобработка данных и исследовательский анализ: Проведем предобработку данных, включающую очистку текста от нежелательных символов, удаление стоп-слов, лемматизацию и т.д. Эти шаги помогут улучшить качество моделирования. Изучим распределение уровней сложности фильмов. Также в выборке слишком мало наблюдений, это может стать проблемой при обучении модели. В целевом признаке присутствуют смежные классы, которые необходимо обработать или преобразовать.

- Обучение моделей: На предобработанных данных обучим модели случайного леса и градиентного бустинга с использованием библиотеки CatBoost, сравним их точность и выберем наиболее подходящую.
